---
name: Send a Request to Pay with Ordo Smart Requests
description: Create a Pay.UK Request to Pay ("Smart Request") as a Biller Delivery Request link, track its state, grant or decline due-date extensions, and withdraw it.
api: openapi/ordo-smart-request-manager.yml
operations: [PostSmartRequestBDRAsync, GetSmartRequestAsync, GetSmartRequestsAsync, PostSmartRequestMessagesGrantDueDateAsync, PostSmartRequestMessagesDeclineDueDateAsync, PostWithdrawSmartRequestBDRAsync]
---

# Send a Request to Pay (Smart Request)

Ordo Smart Requests implement Pay.UK **Request to Pay** — a flexible ask-for-payment
message the payer can pay, decline, or ask to extend. Discontinued surface; reference only.

## Auth
Azure APIM subscription key (`Ocp-Apim-Subscription-Key`). Base host
`https://test.api.ordopay.com/smartrequestmanager/v1`.

## Steps
1. **Create the request** — `PostSmartRequestBDRAsync` (newSmartRequestBDRLink) with the
   amount, due date and biller reference; the response returns a `SmartRequestUrls` link
   to deliver to the payer.
2. **Track it** — `GetSmartRequestAsync` by `smartRequestId`, or list messages with
   `GetSmartRequestsAsync` (page with `PageNumber`/`PageSize`).
3. **Handle an extension request** — `PostSmartRequestMessagesGrantDueDateAsync` to grant
   a new due date or `PostSmartRequestMessagesDeclineDueDateAsync` to decline it.
4. **Withdraw** — `PostWithdrawSmartRequestBDRAsync` to cancel the request.

## Conventions & errors
- List endpoints paginate with `PageNumber` / `PageSize` (`conventions/ordo-conventions.yml`).
- RFC 7807 error envelope (`errors/ordo-problem-types.yml`).
