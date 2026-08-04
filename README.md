# Ordo (ordo)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Ordo (operated by The Smart Request Company Ltd) is a United Kingdom open-banking payments provider that lets businesses collect money directly from a customer's bank account over the UK Faster Payments rails, avoiding card fees and chargebacks. Built on PSD2 / Open Banking payment initiation, its fully hosted, white-labelled platform delivers Request to Pay, one-off payment requests, e-commerce, Point of Sale / QR code and contact centre payments, plus Variable Recurring Payments (VRP) and account information (AIS) and account verification services.

Ordo has since ceased trading and been acquired by Neonomics. The marketing site at [ordopay.com](https://ordopay.com/) remains live; the ReadMe.io developer portal at `docs.myordo.com` is now offline. The six OpenAPI 3.0.1 definitions in `openapi/` were recovered verbatim from Internet Archive snapshots of the developer portal.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/apis.yml)

## Tags

- Payments
- United Kingdom
- Open Banking
- Account-to-Account
- Payment Initiation
- Variable Recurring Payments
- Request to Pay
- Real-Time Payments
- Faster Payments
- PSD2
- Account Information

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## APIs

All APIs run behind an Azure API Management gateway (`test.api.ordopay.com`) and authenticate with a gateway subscription key (`Ocp-Apim-Subscription-Key` header or `subscription-key` query).

### Ordo Single Payments API

Single, one-off open-banking payment initiation — list institutions, create, initiate and withdraw a payment. 4 operations.

- **Human URL:** [https://ordopay.com/products/payments](https://ordopay.com/products/payments)
- **Base URL:** `https://test.api.ordopay.com/payments`
- [OpenAPI](openapi/ordo-single-payments.yml)

### Ordo Smart Request Manager API

Request to Pay / "Smart Request" management for one-off payment requests, Biller Delivery Request (BDR) links, extensions and withdrawals. 8 operations.

- **Human URL:** [https://ordopay.com/products/payments](https://ordopay.com/products/payments)
- **Base URL:** `https://test.api.ordopay.com/smartrequestmanager/v1`
- [OpenAPI](openapi/ordo-smart-request-manager.yml)

### Ordo Recurring Payment Mandates (VRP) API

Variable Recurring Payments — sweeping and non-sweeping mandates, mandate payments and VRP transactions. 6 operations.

- **Human URL:** [https://ordopay.com/products/vrp](https://ordopay.com/products/vrp)
- **Base URL:** `https://test.api.ordopay.com/vrp/v1`
- [OpenAPI](openapi/ordo-recurring-payment-mandates.yml)

### Ordo Account Data (Ordo Hosted) API

Account Information (AIS) and account verification with Ordo hosting the end-user authorisation UX. 13 operations.

- **Human URL:** [https://ordopay.com/products/account/data](https://ordopay.com/products/account/data)
- **Base URL:** `https://test.api.ordopay.com/hosted`
- [OpenAPI](openapi/ordo-account-data-ordo-hosted.yml)

### Ordo Account Data (Client Hosted) API

The same AIS + verification lifecycle with the integrating client hosting the authorisation UX. 15 operations.

- **Human URL:** [https://ordopay.com/products/account/verify](https://ordopay.com/products/account/verify)
- **Base URL:** `https://test.api.ordopay.com/client`
- [OpenAPI](openapi/ordo-account-data-client-hosted.yml)

### Ordo Registry Manager API

Bank account configuration / registry management for the biller bank accounts into which payments settle. 3 operations.

- **Human URL:** [https://ordopay.com/products/payments](https://ordopay.com/products/payments)
- **Base URL:** `https://test.api.ordopay.com/registrymanager/v1`
- [OpenAPI](openapi/ordo-registry-manager.yml)

## Common Properties

- [Website](https://ordopay.com/)
- [Developer Portal](https://docs.myordo.com/docs) (offline / archived)
- [API Reference](https://docs.myordo.com/reference) (offline / archived)
- [Getting Started](https://docs.myordo.com/docs/get-started) (offline / archived)
- [GitHub Organization](https://github.com/ordohq)
- [LinkedIn](https://www.linkedin.com/company/ordohq)
- [Terms of Service](https://ordopay.com/legal/merchant-terms)
- [Privacy Policy](https://ordopay.com/legal/privacy-policy)
- [Support](https://ordopay.com/contact)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
