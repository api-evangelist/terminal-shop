# Terminal (terminal-shop)

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

Terminal is a developer-focused coffee company with an API-first, SSH-first ordering experience. The Terminal Shop API is a public REST API (Bearer token) for browsing coffee products, managing carts, placing orders, running subscriptions, and handling addresses, cards, and profiles - the same surface that powers the famous `ssh terminal.shop` storefront.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/terminal-shop/refs/heads/main/apis.yml)

## The `ssh terminal.shop` Experience

Terminal is best known for letting you buy coffee straight from your terminal: run `ssh terminal.shop` and a full TUI storefront opens over SSH. That same storefront is backed by the public Terminal Shop REST API documented here, along with official Stainless-generated SDKs (Go, JavaScript/TypeScript, Python, Java, Kotlin, Ruby) and a Terraform provider. The API serves a production environment at `https://api.terminal.shop` and a dev sandbox at `https://api.dev.terminal.shop` that places test orders without real charges.

## Tags

- Coffee
- E-Commerce
- Developer
- SSH
- Ordering

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Terminal Products API

Lists Terminal's coffee products and their purchasable variants, with pricing (in cents), market availability, and subscription eligibility.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Products
- Catalog
- Coffee

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [API Reference](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Terminal Cart API

Manages the current user's cart - set item quantities, attach a shipping address and card, clear the cart, and convert it into an order at checkout.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Cart
- Checkout

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Terminal Orders API

Creates orders directly (bypassing the cart), lists past orders, and retrieves a single order with amounts, line items, shipping, and carrier tracking.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Orders
- Fulfillment
- Tracking

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Terminal Subscriptions API

Creates and manages recurring coffee subscriptions on fixed or weekly schedules, tied to a product variant, address, and card.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Subscriptions
- Recurring

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Terminal Addresses & Cards API

Manages saved shipping addresses and Stripe-tokenized payment cards for the current user, including a hosted card-collection flow.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Addresses
- Cards
- Payment

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Terminal Profile API

Reads and updates the current user's profile (name and email) and surfaces a single aggregate view of all account state via `/view/init`.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Profile
- User
- Account

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Terminal Tokens & Apps API

Manages personal access tokens used as Bearer credentials and registers OAuth apps (client ID/secret and redirect URI) for third-party integrations.

- **Human URL:** [https://www.terminal.shop/api](https://www.terminal.shop/api)
- **Base URL:** `https://api.terminal.shop`

#### Tags

- Tokens
- OAuth
- Apps

#### Properties

- [Documentation](https://www.terminal.shop/api)
- [OpenAPI](openapi/terminal-shop-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/terminal-shop.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/terminal-shop.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/terminaldotshop)
- [LinkedIn](https://www.linkedin.com/company/terminalshop)
- [Website](https://www.terminal.shop)
- [Documentation](https://www.terminal.shop/api)
- [Plans](plans/terminal-shop-plans-pricing.yml)
- [Rate Limits](rate-limits/terminal-shop-rate-limits.yml)
- [Fin Ops](finops/terminal-shop-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
