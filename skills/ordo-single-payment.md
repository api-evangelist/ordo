---
name: Collect a one-off open-banking payment with Ordo
description: Initiate a single account-to-account payment over UK Faster Payments — pick the payer's bank, initiate the payment, and hand the payer to their bank's authorisation screen.
api: openapi/ordo-single-payments.yml
operations: [get-institutions, post-initiatepayment, postwithdrawsmartrequestbdrasync]
---

# Collect a one-off open-banking payment

Ordo Single Payments initiates a one-off account-to-account payment (PIS) that settles
over UK Faster Payments. Payments are **discontinued** (Ordo ceased trading; the gateway
is offline) — treat this as reference for the archived contract.

## Auth
All requests carry the Azure APIM subscription key: header `Ocp-Apim-Subscription-Key`
(or `subscription-key` query param). Base host `https://test.api.ordopay.com/payments`.

## Steps
1. **List supported banks** — `get-institutions` returns the open-banking participants
   (`participantId`) the payer can pay from.
2. **Initiate the payment** — `post-initiatepayment` with the amount, payer alias and
   chosen `participantId`. The `initiatePaymentResponse` returns a `SmartRequestUrls`
   object with the redirect URL into the payer's bank / Ordo-hosted authorisation UX.
3. **Redirect the payer** to that URL to authorise the payment at their bank.
4. **Withdraw if needed** — before authorisation completes, cancel with
   `postwithdrawsmartrequestbdrasync`.

## Conventions & errors
- No idempotency-key contract is documented — do not blindly retry a POST; re-check
  state first.
- Errors are RFC 7807 `ProblemDetails` / `OrdoValidationProblemDetails`
  (see `errors/ordo-problem-types.yml`): 400/422 for validation, 401 for a bad
  subscription key, 404 for an unknown payment.
