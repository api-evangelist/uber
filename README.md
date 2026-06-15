# Uber (uber)

Uber is a global technology platform offering transportation, food delivery, and logistics services. Its developer platform provides APIs for integrating ride requests, food ordering, on-demand delivery, voucher programs, and business travel management into third-party applications. APIs use OAuth 2.0 authentication with scope-based access controls and support both production and sandbox environments.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Ride-Sharing
- Rides
- Taxis
- Transportation
- Food Delivery
- Delivery
- Logistics

## Timestamps

- **Created:** 2025-02-06
- **Modified:** 2026-06-03

## APIs

### Uber Riders API

The Uber Riders API enables applications to interact with the Uber platform on behalf of riders. It allows requesting rides, getting product listings, price and time estimates, viewing trip history, and managing saved places. Authentication uses OAuth 2.0 bearer tokens.

- **Human URL:** [https://developer.uber.com/docs/riders/introduction](https://developer.uber.com/docs/riders/introduction)
- **Base URL:** `https://api.uber.com/v1.2`

#### Tags

- Ride-Sharing
- Rides
- Products
- Estimates
- Transportation

#### Properties

- [Documentation](https://developer.uber.com/docs/riders/references/api)
- [Documentation](https://developer.uber.com/docs/riders/ride-requests/introduction)
- [OpenAPI](openapi/uber-riders-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-riders.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-riders.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [SDK](https://github.com/uber/rides-android-sdk)
- [SDK](https://github.com/uber/uber-ios-sdk)
- [SDK](https://pypi.org/project/uber-rides/)
- [SDK](https://github.com/uber/rides-java-sdk)
- [Code Examples](https://github.com/uber/Python-Sample-Application)
- [Example](examples/uber-riders-list-products-example.json)
- [Example](examples/uber-riders-create-ride-request-example.json)
- [JSON Schema](json-schema/uber-ride-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-product-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-priceestimate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-timeestimate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-rideestimate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-riderprofile-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-ridedetails-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-riderequest-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-place-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-placeupdate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-activities-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/uber-riders-structure.json)

### Uber Drivers API

The Uber Drivers API allows partners to access driver profile information, payment history, and trip records. It provides access to driver earnings, completed trips, and partner program data via OAuth 2.0 bearer tokens.

- **Human URL:** [https://developer.uber.com/docs/drivers/introduction](https://developer.uber.com/docs/drivers/introduction)
- **Base URL:** `https://api.uber.com/v1`

#### Tags

- Drivers
- Ride-Sharing
- Payments
- Trips
- Transportation

#### Properties

- [Documentation](https://developer.uber.com/docs/drivers/references/api)
- [OpenAPI](openapi/uber-drivers-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-drivers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-drivers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/uber-driverprofile-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-drivertrip-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-payment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-paymentsresponse-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Uber Eats API

The Uber Eats Marketplace API enables partners to programmatically manage stores, menus, and orders on the Uber Eats platform. It supports real-time menu synchronization, order processing, store operations, promotional campaigns, and analytics reporting. Access requires written approval from Uber.

- **Human URL:** [https://developer.uber.com/docs/eats/introduction](https://developer.uber.com/docs/eats/introduction)
- **Base URL:** `https://api.uber.com/v1`

#### Tags

- Food Delivery
- Restaurants
- Orders
- Menus
- Delivery

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/introduction)
- [Changelog](https://developer.uber.com/docs/eats/api-change-log)
- [OpenAPI](openapi/uber-eats-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/uber-eats-get-order-example.json)
- [JSON Schema](json-schema/uber-store-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-storeupdate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-menu-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-menucategory-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-menuitem-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-orderreceipt-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-reportrequest-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Uber Direct API

The Uber Direct API allows merchants to leverage Uber's courier network to deliver their orders. It supports on-demand delivery creation, courier tracking, refunds, and location management. Webhooks provide real-time delivery status, courier updates, and shopping progress notifications.

- **Human URL:** [https://developer.uber.com/docs/deliveries/overview](https://developer.uber.com/docs/deliveries/overview)
- **Base URL:** `https://api.uber.com/v1`

#### Tags

- Delivery
- Courier
- Logistics
- Fulfillment

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/overview)
- [OpenAPI](openapi/uber-direct-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [SDK](https://www.npmjs.com/package/uber-direct)
- [SDK](https://github.com/uber/uber-direct-sdk)
- [Code Examples](https://github.com/uber/uber-direct-sdk-samples)
- [Authentication](https://developer.uber.com/docs/deliveries/authentication)
- [Example](examples/uber-direct-create-delivery-example.json)
- [JSON Schema](json-schema/uber-delivery-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-deliveryquote-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-deliveryrequest-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-organization-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-refund-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-refundrequest-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-businesslocation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-businesslocationrequest-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Uber Guest Rides API

The Uber Guest Rides API enables businesses to allow their users to request rides from Uber without requiring an Uber account. Uses OAuth 2.0 with the guest.rides scope for authentication.

- **Human URL:** [https://developer.uber.com/docs/guest-rides/introduction](https://developer.uber.com/docs/guest-rides/introduction)
- **Base URL:** `https://api.uber.com/v1`

#### Tags

- Ride-Sharing
- Guest
- Trips
- Transportation

#### Properties

- [Documentation](https://developer.uber.com/docs/guest-rides/introduction)
- [Documentation](https://developer.uber.com/docs/guest-rides/about/u4b-api-introduction)
- [Postman Collection](collections/uber-businesses.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-businesses.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-direct.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-direct.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-drivers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-drivers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-eats.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-eats.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-riders.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-riders.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uber-vouchers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-vouchers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Uber Vouchers API

The Uber Vouchers API allows businesses to create and manage voucher programs and codes for rides and meals. It supports program creation, code generation, bulk distribution, guest management, and code redemption workflows.

- **Human URL:** [https://developer.uber.com/docs/vouchers/introduction](https://developer.uber.com/docs/vouchers/introduction)
- **Base URL:** `https://api.uber.com/v1`

#### Tags

- Vouchers
- Promotions
- Incentives
- Codes

#### Properties

- [Documentation](https://developer.uber.com/docs/vouchers/introduction)
- [OpenAPI](openapi/uber-vouchers-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-vouchers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-vouchers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/uber-vouchercode-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-voucherprogram-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-voucherprogramrequest-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-voucherprogramupdate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-vouchertemplate-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Uber for Business API

The Uber for Business API enables organizations to automate workflows within their enterprise Uber accounts. Provides access to trip invoices, receipts, and business travel data for expense management and reporting.

- **Human URL:** [https://developer.uber.com/docs/businesses/introduction](https://developer.uber.com/docs/businesses/introduction)
- **Base URL:** `https://api.uber.com/v1.2`

#### Tags

- Business
- Enterprise
- Receipts
- Trips
- Expenses

#### Properties

- [Documentation](https://developer.uber.com/docs/businesses/introduction)
- [Documentation](https://developer.uber.com/docs/businesses/receipts/references/api)
- [OpenAPI](openapi/uber-businesses-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/uber-businesses.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uber-businesses.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/uber-receipt-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-tripreceipt-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/uber-tripsresponse-schema.json) — [JSON Schema](https://json-schema.org/specification)

## Common Properties

- [GitHub Organization](https://github.com/uber)
- [LinkedIn](https://www.linkedin.com/company/uber-com)
- [Portal](https://developer.uber.com/)
- [Documentation](https://developer.uber.com/docs)
- [Console](https://developer.uber.com/dashboard)
- [Sign Up](https://developer.uber.com/dashboard)
- [Getting Started](https://developer.uber.com/docs/riders/getting-started/introduction)
- [Authentication](https://developer.uber.com/docs/riders/guides/authentication/introduction)
- [Pricing](https://www.uber.com/us/en/business/api/)
- [Terms of Service](https://developer.uber.com/docs/riders/policies/license-and-terms-of-use)
- [Privacy Policy](https://www.uber.com/legal/en/document/?name=privacy-notice)
- [Blog](https://www.uber.com/blog/engineering/)
- [GitHub Repository](https://github.com/uber/uber-direct-sdk)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [JSON Structure](json-structure/uber-structure.json)
- [Plans](plans/uber-plans-pricing.yml)
- [Rate Limits](rate-limits/uber-rate-limits.yml)
- [Fin Ops](finops/uber-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
