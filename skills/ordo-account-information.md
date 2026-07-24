---
name: Retrieve bank account data with Ordo AIS
description: Create an Account Information consent, execute a data request against the authorised account, and read the returned accounts, balances and transactions.
api: openapi/ordo-account-data-ordo-hosted.yml
operations: [post-account-information-create, post-account-information-data, get-account-information-data-request-aisdatarequestid, get-account-information-consent-aisconsentid, post-account-information-cancel]
---

# Retrieve bank account data (AIS)

Ordo Account Data implements Open Banking **Account Information Services** — with the
end user authorising via an Ordo-hosted UX (the client-hosted variant mirrors this at
`openapi/ordo-account-data-client-hosted.yml`). Discontinued surface; reference only.

## Auth
Azure APIM subscription key (`Ocp-Apim-Subscription-Key`). Base host
`https://test.api.ordopay.com/hosted`.

## Steps
1. **Create a consent** — `post-account-information-create` returns a `CreateAISConsentResponse`
   with the `aisConsentId` and an authorisation URL to send the customer to their bank.
2. **Check consent status** — `get-account-information-consent-aisconsentid` by `aisConsentId`
   until it is authorised.
3. **Request data** — `post-account-information-data` under the authorised consent to kick
   off an `aisDataRequestId`.
4. **Read the data** — `get-account-information-data-request-aisdatarequestid` returns the
   `OBAccount`s, balances and transactions.
5. **Cancel** — `post-account-information-cancel` to revoke the consent.

## Conventions & errors
- Account data is only returned while the consent is live; a cancelled/expired consent
  yields 403/404.
- RFC 7807 error envelope (`errors/ordo-problem-types.yml`).
