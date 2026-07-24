# Ordo (ordo)

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
