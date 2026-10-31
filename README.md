# Ordo

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

> **No longer operating.** This company or product has shut down, been discontinued, or been deprecated. This profile is kept as a historical record and is not maintained or rated.

Ordo (operated by The Smart Request Company Ltd, ordohq.com / ordopay.com) is a United Kingdom open-banking payments provider that lets businesses collect money directly from a customer's bank account over the UK Faster Payments rails, avoiding card fees and chargebacks. Built on PSD2 / Open Banking payment initiation, its fully hosted, white-labelled platform delivers Request to Pay, one-off payment requests, e-commerce, Point of Sale / QR code and contact centre payments, plus Variable Recurring Payments (VRP) for fixed, variable and sweeping collections, and account information (AIS) and account verification services. Ordo is FCA-authorised and an Open Banking regulated provider, with a developer surface historically published as a ReadMe.io portal at docs.myordo.com backed by an Azure API Management gateway (test.api.ordopay.com). Ordo has since ceased trading and been acquired by Neonomics; the marketing site at ordopay.com remains live while the developer portal is now offline. Its API posture is documented here honestly from six OpenAPI 3.0.1 definitions harvested verbatim from the archived developer portal.

**Areas:** Payments · United Kingdom · Open Banking · Account-to-Account · Payment Initiation · Variable Recurring Payments · Request to Pay · Real-Time Payments · Faster Payments · PSD2 · Account Information · Defunct

## Ordo on APIs.io (historical record)

Everything profiled for Ordo is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/ordo/](https://apis.io/providers/ordo/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Ordo Account Data - Client Hosted API](https://apis.io/apis/ordo/ordo-account-data-client-hosted-api/) — The Account Data - Client Hosted API from Ordo — 9 operation(s) for account data - client hosted.
- [Ordo Account Verification - Client Hosted API](https://apis.io/apis/ordo/ordo-account-verification-client-hosted-api/) — The Account Verification - Client Hosted API from Ordo — 6 operation(s) for account verification - client hosted.
- [Ordo Bank accounts API](https://apis.io/apis/ordo/ordo-bank-accounts-api/) — The Bank accounts API from Ordo — 3 operation(s) for bank accounts.
- [Ordo Client hosted API](https://apis.io/apis/ordo/ordo-client-hosted-api/) — The Client hosted API from Ordo — 4 operation(s) for client hosted.
- [Ordo Create a mandate API](https://apis.io/apis/ordo/ordo-create-a-mandate-api/) — The Create a mandate API from Ordo — 2 operation(s) for create a mandate.
- [Ordo Hosted API](https://apis.io/apis/ordo/ordo-ordo-hosted-api/) — The Ordo hosted API from Ordo — 8 operation(s) for ordo hosted.
- [Ordo Retrieve mandate details API](https://apis.io/apis/ordo/ordo-retrieve-mandate-details-api/) — The Retrieve mandate details API from Ordo — 4 operation(s) for retrieve mandate details.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [ordo](https://apis.io/servers/ordo/ordo/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Ordo Agentic Access](https://apis.io/agentic-access/ordo/ordo-agentic-access/)

#### Collections (6)

Postman and Open Collection request collections.

- [ACCOUNT DATA - Client Hosted](https://apis.io/collections/ordo/open-ordo-account-data-client-hosted/)
- [ACCOUNT DATA - Ordo Hosted](https://apis.io/collections/ordo/open-ordo-account-data-ordo-hosted/)
- [Recurring Payment Mandates](https://apis.io/collections/ordo/open-ordo-recurring-payment-mandates/)
- [Bank account configuration](https://apis.io/collections/ordo/open-ordo-registry-manager/)
- [Single Payments](https://apis.io/collections/ordo/open-ordo-single-payments/)
- [Single Payments](https://apis.io/collections/ordo/open-ordo-smart-request-manager/)

#### Overlays (6)

OpenAPI overlays, including conversational phrasing for each operation.

- [Ordo Account Data Client Hosted Overlay](https://apis.io/overlays/ordo/ordo-account-data-client-hosted-overlay/)
- [Ordo Account Data Hosted Overlay](https://apis.io/overlays/ordo/ordo-account-data-hosted-overlay/)
- [Ordo Recurring Payment Mandates Overlay](https://apis.io/overlays/ordo/ordo-recurring-payment-mandates-overlay/)
- [Ordo Registry Manager Overlay](https://apis.io/overlays/ordo/ordo-registry-manager-overlay/)
- [Ordo Single Payments Overlay](https://apis.io/overlays/ordo/ordo-single-payments-overlay/)
- [Ordo Smart Request Manager Overlay](https://apis.io/overlays/ordo/ordo-smart-request-manager-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Ordo Authentication](https://apis.io/security/ordo/ordo-authentication/)
- [Ordo Domain Security](https://apis.io/security/ordo/ordo-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://ordopay.com/)
- [Getting started](https://docs.myordo.com/docs/get-started)
- [API reference](https://docs.myordo.com/reference)
- [Support](https://ordopay.com/contact)
- [Terms of service](https://ordopay.com/legal/merchant-terms)
- [Privacy policy](https://ordopay.com/legal/privacy-policy)
- [GitHub](https://github.com/ordohq)

## API Evangelist rating

**Not rated** — this company is recorded as no longer operating, so no score is published. If it is in fact operating, say so on this repository and it will be re-profiled.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Ordo: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/ordo/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
