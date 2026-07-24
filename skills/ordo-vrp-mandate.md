---
name: Set up a Variable Recurring Payment mandate with Ordo
description: Create a sweeping or non-sweeping VRP mandate with control parameters, read the mandate back, and read the transactions executed under it.
api: openapi/ordo-recurring-payment-mandates.yml
operations: [post-vrpmandate, get-vrpmandate-mandateid, get-vrpmandates, get-vrptransactions-vrpmandateid, get-vrptransaction-vrptransactionid]
---

# Set up a Variable Recurring Payment (VRP) mandate

Ordo VRP lets a payer authorise recurring account-to-account collections within control
parameters — an Open Banking alternative to Direct Debit and card CPA. Discontinued
surface; reference only.

## Auth
Azure APIM subscription key (`Ocp-Apim-Subscription-Key`). Base host
`https://test.api.ordopay.com/vrp/v1`.

## Steps
1. **Create the mandate** — `post-vrpmandate` (POST `/VRPMandate/sweeping`) for a sweeping
   mandate, supplying `VRPControlParameters` (max amount per payment/period, valid-from/to).
   A non-sweeping mandate is created at POST `/VRPMandate/nonsweeping`.
2. **Read the mandate** — `get-vrpmandate-mandateid` by `mandateId`, or list all with
   `get-vrpmandates`.
3. **Read executed transactions** — `get-vrptransactions-vrpmandateid` for every payment
   under a mandate, or `get-vrptransaction-vrptransactionid` for one.

## Conventions & errors
- Control parameters bound each collection; a payment outside them is rejected (422).
- No idempotency-key contract — check mandate/transaction state before re-issuing.
- RFC 7807 error envelope (`errors/ordo-problem-types.yml`).
