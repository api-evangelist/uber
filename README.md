# Uber

Uber is a global technology platform offering transportation, food delivery, and logistics services. Its developer platform provides APIs for integrating ride requests, food ordering, on-demand delivery, voucher programs, and business travel management into third-party applications. APIs use OAuth 2.0 authentication with scope-based access controls and support both production and sandbox environments.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/uber/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Ride-Sharing, Rides, Taxis, Transportation, Food Delivery, Delivery, Logistics

## Timestamps

- **Created:** 2025-02-06
- **Modified:** 2026-06-03

## APIs

### Uber Riders API

The Uber Riders API enables applications to interact with the Uber platform on behalf of riders. It allows requesting rides, getting product listings, price and time estimates, viewing trip history, and managing saved places. Authentication uses OAuth 2.0 bearer tokens.

**Human URL:** [https://developer.uber.com/docs/riders/introduction](https://developer.uber.com/docs/riders/introduction)

#### Tags:

 - Ride-Sharing, Rides, Products, Estimates, Transportation

#### Properties

- [Documentation](https://developer.uber.com/docs/riders/references/api)
- [Documentation](https://developer.uber.com/docs/riders/ride-requests/introduction)
- [OpenAPI](openapi/uber-riders-openapi.yml)
- [SDK - Android SDK](https://github.com/uber/rides-android-sdk)
- [SDK - iOS SDK](https://github.com/uber/uber-ios-sdk)
- [SDK - Python SDK](https://pypi.org/project/uber-rides/)
- [SDK - Java SDK](https://github.com/uber/rides-java-sdk)
- [CodeExamples - Python Sample Application](https://github.com/uber/Python-Sample-Application)
- [Example](examples/uber-riders-list-products-example.json)
- [Example](examples/uber-riders-create-ride-request-example.json)
- [JSONSchema](json-schema/uber-ride-request-schema.json)
- [NaftikoCapability](capabilities/riders-estimates.yaml)
- [NaftikoCapability](capabilities/riders-places.yaml)
- [NaftikoCapability](capabilities/riders-products.yaml)
- [NaftikoCapability](capabilities/riders-requests.yaml)
- [NaftikoCapability](capabilities/riders-riders.yaml)
- [JSONSchema](json-schema/uber-product-schema.json)
- [JSONSchema](json-schema/uber-priceestimate-schema.json)
- [JSONSchema](json-schema/uber-timeestimate-schema.json)
- [JSONSchema](json-schema/uber-rideestimate-schema.json)
- [JSONSchema](json-schema/uber-riderprofile-schema.json)
- [JSONSchema](json-schema/uber-ridedetails-schema.json)
- [JSONSchema](json-schema/uber-riderequest-schema.json)
- [JSONSchema](json-schema/uber-place-schema.json)
- [JSONSchema](json-schema/uber-placeupdate-schema.json)
- [JSONSchema](json-schema/uber-activities-schema.json)
- [JSONStructure](json-structure/uber-riders-structure.json)

### Uber Drivers API

The Uber Drivers API allows partners to access driver profile information, payment history, and trip records. It provides access to driver earnings, completed trips, and partner program data via OAuth 2.0 bearer tokens.

**Human URL:** [https://developer.uber.com/docs/drivers/introduction](https://developer.uber.com/docs/drivers/introduction)

#### Tags:

 - Drivers, Ride-Sharing, Payments, Trips, Transportation

#### Properties

- [Documentation](https://developer.uber.com/docs/drivers/references/api)
- [OpenAPI](openapi/uber-drivers-openapi.yml)
- [NaftikoCapability](capabilities/drivers-partners.yaml)
- [JSONSchema](json-schema/uber-driverprofile-schema.json)
- [JSONSchema](json-schema/uber-drivertrip-schema.json)
- [JSONSchema](json-schema/uber-payment-schema.json)
- [JSONSchema](json-schema/uber-paymentsresponse-schema.json)

### Uber Eats API

The Uber Eats Marketplace API enables partners to programmatically manage stores, menus, and orders on the Uber Eats platform. It supports real-time menu synchronization, order processing, store operations, promotional campaigns, and analytics reporting. Access requires written approval from Uber.

**Human URL:** [https://developer.uber.com/docs/eats/introduction](https://developer.uber.com/docs/eats/introduction)

#### Tags:

 - Food Delivery, Restaurants, Orders, Menus, Delivery

#### Properties

- [Documentation](https://developer.uber.com/docs/eats/introduction)
- [ChangeLog](https://developer.uber.com/docs/eats/api-change-log)
- [OpenAPI](openapi/uber-eats-openapi.yml)
- [Example](examples/uber-eats-get-order-example.json)
- [NaftikoCapability](capabilities/eats-menus.yaml)
- [NaftikoCapability](capabilities/eats-orders.yaml)
- [NaftikoCapability](capabilities/eats-reporting.yaml)
- [NaftikoCapability](capabilities/eats-stores.yaml)
- [JSONSchema](json-schema/uber-store-schema.json)
- [JSONSchema](json-schema/uber-storeupdate-schema.json)
- [JSONSchema](json-schema/uber-menu-schema.json)
- [JSONSchema](json-schema/uber-menucategory-schema.json)
- [JSONSchema](json-schema/uber-menuitem-schema.json)
- [JSONSchema](json-schema/uber-order-schema.json)
- [JSONSchema](json-schema/uber-orderreceipt-schema.json)
- [JSONSchema](json-schema/uber-reportrequest-schema.json)

### Uber Direct API

The Uber Direct API allows merchants to leverage Uber's courier network to deliver their orders. It supports on-demand delivery creation, courier tracking, refunds, and location management. Webhooks provide real-time delivery status, courier updates, and shopping progress notifications.

**Human URL:** [https://developer.uber.com/docs/deliveries/overview](https://developer.uber.com/docs/deliveries/overview)

#### Tags:

 - Delivery, Courier, Logistics, Fulfillment

#### Properties

- [Documentation](https://developer.uber.com/docs/deliveries/overview)
- [OpenAPI](openapi/uber-direct-openapi.yml)
- [SDK - JavaScript SDK](https://www.npmjs.com/package/uber-direct)
- [SDK - JavaScript SDK Source](https://github.com/uber/uber-direct-sdk)
- [CodeExamples - JavaScript SDK Samples](https://github.com/uber/uber-direct-sdk-samples)
- [Authentication](https://developer.uber.com/docs/deliveries/authentication)
- [Example](examples/uber-direct-create-delivery-example.json)
- [JSONSchema](json-schema/uber-delivery-schema.json)
- [NaftikoCapability](capabilities/direct-deliveries.yaml)
- [NaftikoCapability](capabilities/direct-locations.yaml)
- [NaftikoCapability](capabilities/direct-organizations.yaml)
- [NaftikoCapability](capabilities/direct-refunds.yaml)
- [JSONSchema](json-schema/uber-deliveryquote-schema.json)
- [JSONSchema](json-schema/uber-deliveryrequest-schema.json)
- [JSONSchema](json-schema/uber-organization-schema.json)
- [JSONSchema](json-schema/uber-refund-schema.json)
- [JSONSchema](json-schema/uber-refundrequest-schema.json)
- [JSONSchema](json-schema/uber-businesslocation-schema.json)
- [JSONSchema](json-schema/uber-businesslocationrequest-schema.json)

### Uber Guest Rides API

The Uber Guest Rides API enables businesses to allow their users to request rides from Uber without requiring an Uber account. Uses OAuth 2.0 with the guest.rides scope for authentication.

**Human URL:** [https://developer.uber.com/docs/guest-rides/introduction](https://developer.uber.com/docs/guest-rides/introduction)

#### Tags:

 - Ride-Sharing, Guest, Trips, Transportation

#### Properties

- [Documentation](https://developer.uber.com/docs/guest-rides/introduction)
- [Documentation](https://developer.uber.com/docs/guest-rides/about/u4b-api-introduction)

### Uber Vouchers API

The Uber Vouchers API allows businesses to create and manage voucher programs and codes for rides and meals. It supports program creation, code generation, bulk distribution, guest management, and code redemption workflows.

**Human URL:** [https://developer.uber.com/docs/vouchers/introduction](https://developer.uber.com/docs/vouchers/introduction)

#### Tags:

 - Vouchers, Promotions, Incentives, Codes

#### Properties

- [Documentation](https://developer.uber.com/docs/vouchers/introduction)
- [OpenAPI](openapi/uber-vouchers-openapi.yml)
- [NaftikoCapability](capabilities/vouchers-codes.yaml)
- [NaftikoCapability](capabilities/vouchers-programs.yaml)
- [NaftikoCapability](capabilities/vouchers-redemption.yaml)
- [NaftikoCapability](capabilities/vouchers-templates.yaml)
- [JSONSchema](json-schema/uber-vouchercode-schema.json)
- [JSONSchema](json-schema/uber-voucherprogram-schema.json)
- [JSONSchema](json-schema/uber-voucherprogramrequest-schema.json)
- [JSONSchema](json-schema/uber-voucherprogramupdate-schema.json)
- [JSONSchema](json-schema/uber-vouchertemplate-schema.json)

### Uber for Business API

The Uber for Business API enables organizations to automate workflows within their enterprise Uber accounts. Provides access to trip invoices, receipts, and business travel data for expense management and reporting.

**Human URL:** [https://developer.uber.com/docs/businesses/introduction](https://developer.uber.com/docs/businesses/introduction)

#### Tags:

 - Business, Enterprise, Receipts, Trips, Expenses

#### Properties

- [Documentation](https://developer.uber.com/docs/businesses/introduction)
- [Documentation](https://developer.uber.com/docs/businesses/receipts/references/api)
- [OpenAPI](openapi/uber-businesses-openapi.yml)
- [NaftikoCapability](capabilities/businesses-orders.yaml)
- [NaftikoCapability](capabilities/businesses-trips.yaml)
- [JSONSchema](json-schema/uber-receipt-schema.json)
- [JSONSchema](json-schema/uber-tripreceipt-schema.json)
- [JSONSchema](json-schema/uber-tripsresponse-schema.json)

## Common Properties

- [GitHubOrganization](https://github.com/uber)
- [LinkedIn](https://www.linkedin.com/company/uber-com)
- [Portal](https://developer.uber.com/)
- [Documentation](https://developer.uber.com/docs)
- [Console](https://developer.uber.com/dashboard)
- [SignUp](https://developer.uber.com/dashboard)
- [GettingStarted](https://developer.uber.com/docs/riders/getting-started/introduction)
- [Authentication](https://developer.uber.com/docs/riders/guides/authentication/introduction)
- [Pricing](https://www.uber.com/us/en/business/api/)
- [TermsOfService](https://developer.uber.com/docs/riders/policies/license-and-terms-of-use)
- [PrivacyPolicy](https://www.uber.com/legal/en/document/?name=privacy-notice)
- [Blog](https://www.uber.com/blog/engineering/)
- [GitHubRepository](https://github.com/uber/uber-direct-sdk)
- [JSONStructure](json-structure/uber-structure.json)
- [Plans](plans/uber-plans-pricing.yml)
- [RateLimits](rate-limits/uber-rate-limits.yml)
- [FinOps](finops/uber-finops.yml)

## Features

| Name | Description |
|------|-------------|
| OAuth 2.0 Authorization | All Uber developer APIs authenticate with OAuth 2.0 bearer tokens using scope-based access controls for both client-credentials (server-to-server) and authorization-code (on behalf of a user) flows. |
| Sandbox Environment | Most APIs offer a sandbox for simulating rides, deliveries, and orders without dispatching real couriers or charging real payment methods. |
| Webhooks | Uber Direct and Uber Eats publish real-time event webhooks for delivery status, courier updates, shopping progress, refunds, and order lifecycle changes. |
| Courier Delivery Network | Uber Direct exposes Uber's on-demand courier network so merchants can quote, create, track, and manage last-mile deliveries from their own storefronts. |
| Marketplace Integration | Uber Eats Marketplace APIs let restaurants and POS partners synchronize stores, menus, and orders with the Uber Eats consumer marketplace in real time. |

## Use Cases

| Name | Description |
|------|-------------|
| Restaurant Delivery Fulfillment | Restaurants and food brands use Uber Direct to dispatch couriers for delivery of orders placed on their own websites and apps, bypassing the Uber Eats marketplace fee structure. |
| Menu And Order Synchronization | POS and online-ordering platforms integrate Uber Eats APIs to keep store hours, menus, pricing, and order status in sync between their systems and the Uber Eats marketplace. |
| Corporate Travel And Meals | Enterprises use Uber for Business and Vouchers to provision rides and meals for employees and guests with centralized billing, expense reporting, and policy controls. |
| Guest Ride Provisioning | Healthcare, hospitality, and service businesses use Guest Rides to request trips on behalf of customers who do not have an Uber account. |

## Integrations

| Name | Description |
|------|-------------|
| Point Of Sale Systems | Uber Eats integrates with restaurant POS platforms for automated order injection and menu management. |
| E-Commerce And Ordering Platforms | Uber Direct integrates with online ordering and e-commerce checkout flows to add same-day local delivery. |
| Expense And Travel Management | Uber for Business integrates with expense management and corporate travel platforms via receipts and invoices. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [uber-businesses-openapi.yml](openapi/uber-businesses-openapi.yml)
- [uber-direct-openapi.yml](openapi/uber-direct-openapi.yml)
- [uber-drivers-openapi.yml](openapi/uber-drivers-openapi.yml)
- [uber-eats-openapi.yml](openapi/uber-eats-openapi.yml)
- [uber-riders-openapi.yml](openapi/uber-riders-openapi.yml)
- [uber-vouchers-openapi.yml](openapi/uber-vouchers-openapi.yml)

### JSON Schema

- [uber-activities-schema.json](json-schema/uber-activities-schema.json)
- [uber-businesslocation-schema.json](json-schema/uber-businesslocation-schema.json)
- [uber-businesslocationrequest-schema.json](json-schema/uber-businesslocationrequest-schema.json)
- [uber-delivery-schema.json](json-schema/uber-delivery-schema.json)
- [uber-deliveryquote-schema.json](json-schema/uber-deliveryquote-schema.json)
- [uber-deliveryrequest-schema.json](json-schema/uber-deliveryrequest-schema.json)
- [uber-driverprofile-schema.json](json-schema/uber-driverprofile-schema.json)
- [uber-drivertrip-schema.json](json-schema/uber-drivertrip-schema.json)
- [uber-menu-schema.json](json-schema/uber-menu-schema.json)
- [uber-menucategory-schema.json](json-schema/uber-menucategory-schema.json)
- [uber-menuitem-schema.json](json-schema/uber-menuitem-schema.json)
- [uber-order-schema.json](json-schema/uber-order-schema.json)
- [uber-orderreceipt-schema.json](json-schema/uber-orderreceipt-schema.json)
- [uber-organization-schema.json](json-schema/uber-organization-schema.json)
- [uber-payment-schema.json](json-schema/uber-payment-schema.json)
- [uber-paymentsresponse-schema.json](json-schema/uber-paymentsresponse-schema.json)
- [uber-place-schema.json](json-schema/uber-place-schema.json)
- [uber-placeupdate-schema.json](json-schema/uber-placeupdate-schema.json)
- [uber-priceestimate-schema.json](json-schema/uber-priceestimate-schema.json)
- [uber-product-schema.json](json-schema/uber-product-schema.json)
- [uber-receipt-schema.json](json-schema/uber-receipt-schema.json)
- [uber-refund-schema.json](json-schema/uber-refund-schema.json)
- [uber-refundrequest-schema.json](json-schema/uber-refundrequest-schema.json)
- [uber-reportrequest-schema.json](json-schema/uber-reportrequest-schema.json)
- [uber-ride-request-schema.json](json-schema/uber-ride-request-schema.json)
- [uber-ridedetails-schema.json](json-schema/uber-ridedetails-schema.json)
- [uber-rideestimate-schema.json](json-schema/uber-rideestimate-schema.json)
- [uber-riderequest-schema.json](json-schema/uber-riderequest-schema.json)
- [uber-riderprofile-schema.json](json-schema/uber-riderprofile-schema.json)
- [uber-store-schema.json](json-schema/uber-store-schema.json)
- [uber-storeupdate-schema.json](json-schema/uber-storeupdate-schema.json)
- [uber-timeestimate-schema.json](json-schema/uber-timeestimate-schema.json)
- [uber-tripreceipt-schema.json](json-schema/uber-tripreceipt-schema.json)
- [uber-tripsresponse-schema.json](json-schema/uber-tripsresponse-schema.json)
- [uber-vouchercode-schema.json](json-schema/uber-vouchercode-schema.json)
- [uber-voucherprogram-schema.json](json-schema/uber-voucherprogram-schema.json)
- [uber-voucherprogramrequest-schema.json](json-schema/uber-voucherprogramrequest-schema.json)
- [uber-voucherprogramupdate-schema.json](json-schema/uber-voucherprogramupdate-schema.json)
- [uber-vouchertemplate-schema.json](json-schema/uber-vouchertemplate-schema.json)

### JSON Structure

- [uber-riders-structure.json](json-structure/uber-riders-structure.json)
- [uber-structure.json](json-structure/uber-structure.json)

### JSON-LD

- [uber-context.jsonld](json-ld/uber-context.jsonld)

### Examples

- [uber-direct-create-delivery-example.json](examples/uber-direct-create-delivery-example.json)
- [uber-eats-get-order-example.json](examples/uber-eats-get-order-example.json)
- [uber-riders-create-ride-request-example.json](examples/uber-riders-create-ride-request-example.json)
- [uber-riders-list-products-example.json](examples/uber-riders-list-products-example.json)

### Plans & Pricing

- [uber-plans-pricing.yml](plans/uber-plans-pricing.yml)

### Rate Limits

- [uber-rate-limits.yml](rate-limits/uber-rate-limits.yml)

### FinOps

- [uber-finops.yml](finops/uber-finops.yml)

## Capabilities

Self-contained Naftiko capabilities (one per business surface), each exposing both a REST and an MCP adapter. Grouped by owning API.

### Uber Riders API

- [Uber Riders API — Estimates](capabilities/riders-estimates.yaml) — 2 operations (REST + MCP)
- [Uber Riders API — Places](capabilities/riders-places.yaml) — 2 operations (REST + MCP)
- [Uber Riders API — Products](capabilities/riders-products.yaml) — 2 operations (REST + MCP)
- [Uber Riders API — Requests](capabilities/riders-requests.yaml) — 7 operations (REST + MCP)
- [Uber Riders API — Riders](capabilities/riders-riders.yaml) — 3 operations (REST + MCP)

### Uber Drivers API

- [Uber Drivers API — Partners](capabilities/drivers-partners.yaml) — 3 operations (REST + MCP)

### Uber Eats API

- [Uber Eats API — Menus](capabilities/eats-menus.yaml) — 2 operations (REST + MCP)
- [Uber Eats API — Orders](capabilities/eats-orders.yaml) — 4 operations (REST + MCP)
- [Uber Eats API — Reporting](capabilities/eats-reporting.yaml) — 1 operations (REST + MCP)
- [Uber Eats API — Stores](capabilities/eats-stores.yaml) — 4 operations (REST + MCP)

### Uber Direct API

- [Uber Direct API — Deliveries](capabilities/direct-deliveries.yaml) — 4 operations (REST + MCP)
- [Uber Direct API — Locations](capabilities/direct-locations.yaml) — 4 operations (REST + MCP)
- [Uber Direct API — Organizations](capabilities/direct-organizations.yaml) — 2 operations (REST + MCP)
- [Uber Direct API — Refunds](capabilities/direct-refunds.yaml) — 1 operations (REST + MCP)

### Uber Vouchers API

- [Uber Vouchers API — Codes](capabilities/vouchers-codes.yaml) — 3 operations (REST + MCP)
- [Uber Vouchers API — Programs](capabilities/vouchers-programs.yaml) — 6 operations (REST + MCP)
- [Uber Vouchers API — Redemption](capabilities/vouchers-redemption.yaml) — 1 operations (REST + MCP)
- [Uber Vouchers API — Templates](capabilities/vouchers-templates.yaml) — 2 operations (REST + MCP)

### Uber for Business API

- [Uber for Business API — Orders](capabilities/businesses-orders.yaml) — 1 operations (REST + MCP)
- [Uber for Business API — Trips](capabilities/businesses-trips.yaml) — 3 operations (REST + MCP)

## Vocabulary

- [Uber Vocabulary](vocabulary/uber-vocabulary.yml) — Controlled taxonomy spanning 5 domains and 10 categories across the Uber developer platform

## Rules

- [Uber Spectral Ruleset](rules/uber-rules.yml) — 11 rules enforcing Uber API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
