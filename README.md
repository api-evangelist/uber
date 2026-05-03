# Uber

Uber is a global technology platform offering transportation, food delivery, and logistics services. Its developer platform provides APIs for integrating ride requests, food ordering, on-demand delivery, voucher programs, and business travel management into third-party applications. APIs use OAuth 2.0 authentication with scope-based access controls and support both production and sandbox environments.

**URL:** [https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Transportation, Ride-Sharing, Rides, Taxis, Food Delivery, Delivery, Logistics

## Timestamps

- **Created:** 2025-02-06
- **Modified:** 2026-05-03

## APIs

### Uber Riders API
REST API for requesting rides, getting product listings, price and time estimates, viewing trip history, and managing saved places on behalf of Uber riders.

**Human URL:** [https://developer.uber.com/docs/riders/introduction](https://developer.uber.com/docs/riders/introduction)

#### Tags
Ride-Sharing, Rides, Products, Estimates, Transportation

#### Properties
- [Documentation](https://developer.uber.com/docs/riders/references/api)
- [OpenAPI](openapi/uber-riders-openapi.yml)
- [Example](examples/uber-riders-list-products-example.json)
- [Example](examples/uber-riders-create-ride-request-example.json)
- [JSONSchema](json-schema/uber-ride-request-schema.json)

---

### Uber Drivers API
API for accessing driver partner profiles, payment history, and trip records.

**Human URL:** [https://developer.uber.com/docs/drivers/introduction](https://developer.uber.com/docs/drivers/introduction)

#### Tags
Drivers, Ride-Sharing, Payments, Trips, Transportation

#### Properties
- [Documentation](https://developer.uber.com/docs/drivers/references/api)
- [OpenAPI](openapi/uber-drivers-openapi.yml)

---

### Uber Eats API
Marketplace API for managing stores, menus, and orders on the Uber Eats platform, supporting real-time menu sync, order processing, and analytics.

**Human URL:** [https://developer.uber.com/docs/eats/introduction](https://developer.uber.com/docs/eats/introduction)

#### Tags
Food Delivery, Restaurants, Orders, Menus, Delivery

#### Properties
- [Documentation](https://developer.uber.com/docs/eats/introduction)
- [ChangeLog](https://developer.uber.com/docs/eats/api-change-log)
- [OpenAPI](openapi/uber-eats-openapi.yml)
- [Example](examples/uber-eats-get-order-example.json)

---

### Uber Direct API
On-demand delivery API leveraging Uber's courier network for merchant delivery, with quote, dispatch, tracking, and refund capabilities.

**Human URL:** [https://developer.uber.com/docs/deliveries/overview](https://developer.uber.com/docs/deliveries/overview)

#### Tags
Delivery, Courier, Logistics, Fulfillment

#### Properties
- [Documentation](https://developer.uber.com/docs/deliveries/overview)
- [OpenAPI](openapi/uber-direct-openapi.yml)
- [Example](examples/uber-direct-create-delivery-example.json)
- [JSONSchema](json-schema/uber-delivery-schema.json)

---

### Uber Guest Rides API
Enables businesses to allow users to request rides from Uber without requiring an Uber account.

**Human URL:** [https://developer.uber.com/docs/guest-rides/introduction](https://developer.uber.com/docs/guest-rides/introduction)

#### Tags
Ride-Sharing, Guest, Trips, Transportation

#### Properties
- [Documentation](https://developer.uber.com/docs/guest-rides/introduction)

---

### Uber Vouchers API
API for creating and managing voucher programs and codes for rides and meals, including bulk generation and distribution.

**Human URL:** [https://developer.uber.com/docs/vouchers/introduction](https://developer.uber.com/docs/vouchers/introduction)

#### Tags
Vouchers, Promotions, Incentives, Codes

#### Properties
- [Documentation](https://developer.uber.com/docs/vouchers/introduction)
- [OpenAPI](openapi/uber-vouchers-openapi.yml)

---

### Uber for Business API
Enterprise API for accessing trip invoices, receipts, and business travel data for expense management.

**Human URL:** [https://developer.uber.com/docs/businesses/introduction](https://developer.uber.com/docs/businesses/introduction)

#### Tags
Business, Enterprise, Receipts, Trips, Expenses

#### Properties
- [Documentation](https://developer.uber.com/docs/businesses/introduction)
- [OpenAPI](openapi/uber-businesses-openapi.yml)

---

## Artifacts

### OpenAPI Specifications
| File | Description |
|------|-------------|
| [openapi/uber-riders-openapi.yml](openapi/uber-riders-openapi.yml) | Uber Riders API |
| [openapi/uber-drivers-openapi.yml](openapi/uber-drivers-openapi.yml) | Uber Drivers API |
| [openapi/uber-eats-openapi.yml](openapi/uber-eats-openapi.yml) | Uber Eats API |
| [openapi/uber-direct-openapi.yml](openapi/uber-direct-openapi.yml) | Uber Direct API |
| [openapi/uber-vouchers-openapi.yml](openapi/uber-vouchers-openapi.yml) | Uber Vouchers API |
| [openapi/uber-businesses-openapi.yml](openapi/uber-businesses-openapi.yml) | Uber for Business API |

### Naftiko Capabilities
| File | Description |
|------|-------------|
| [capabilities/ride-management.yaml](capabilities/ride-management.yaml) | Ride lifecycle — Riders + Drivers APIs (11 tools) |
| [capabilities/food-and-delivery.yaml](capabilities/food-and-delivery.yaml) | Food and delivery — Eats + Direct APIs (12 tools) |

**Shared definitions:** `capabilities/shared/riders.yaml`, `capabilities/shared/drivers.yaml`, `capabilities/shared/eats.yaml`, `capabilities/shared/direct.yaml`

### Rules
- [rules/uber-rules.yml](rules/uber-rules.yml) — Spectral linting rules for Uber API conventions.

### JSON Schema
- [json-schema/uber-ride-request-schema.json](json-schema/uber-ride-request-schema.json)
- [json-schema/uber-delivery-schema.json](json-schema/uber-delivery-schema.json)

### JSON Structure
- [json-structure/uber-riders-structure.json](json-structure/uber-riders-structure.json)

### JSON-LD
- [json-ld/uber-context.jsonld](json-ld/uber-context.jsonld)

### Examples
- [examples/uber-riders-list-products-example.json](examples/uber-riders-list-products-example.json)
- [examples/uber-riders-create-ride-request-example.json](examples/uber-riders-create-ride-request-example.json)
- [examples/uber-eats-get-order-example.json](examples/uber-eats-get-order-example.json)
- [examples/uber-direct-create-delivery-example.json](examples/uber-direct-create-delivery-example.json)

### Vocabulary
- [vocabulary/uber-vocabulary.yml](vocabulary/uber-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
