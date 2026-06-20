# Terminal (terminal-shop)

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
