# Uber GraphQL Schema

## Overview

This conceptual GraphQL schema covers the full breadth of the Uber developer platform, spanning ride-sharing (Riders API, Drivers API, Guest Rides), food delivery (Uber Eats), on-demand courier logistics (Uber Direct), business/enterprise programs (Uber for Business, Vouchers), and shared supporting types such as payments, receipts, webhooks, and location primitives.

The schema is derived from the REST APIs documented at https://developer.uber.com/docs and existing JSON Schema artifacts in this repository.

## APIs Covered

- **Uber Riders API** — product listings, price/time estimates, ride requests, trip history, saved places
- **Uber Drivers API** — driver profile, trips, payment history
- **Uber Eats API** — stores, menus, menu items, orders, receipts, reporting
- **Uber Direct API** — on-demand delivery, courier tracking, refunds, business locations, webhooks
- **Uber Guest Rides API** — ride provisioning for users without an Uber account
- **Uber Vouchers API** — voucher programs, templates, codes
- **Uber for Business API** — business trips, receipts, invoices

## Design Principles

- All geo-coordinates use a shared `Location` type with `latitude` and `longitude` fields.
- Monetary values use a `Money` type pairing an `amount` (Float) with a `currencyCode` (ISO 4217 string) to avoid integer-cents ambiguity across currencies.
- Enum types reflect the literal string values returned by Uber's REST APIs.
- Mutations represent the write operations available across the REST APIs (create ride request, create delivery, update menu, etc.).
- Subscription types model the webhook event stream that Uber Direct and Uber Eats publish.

## Root Types

### Query

| Field | Return Type | Description |
|---|---|---|
| `products` | `[Product]` | List available ride products at a location |
| `priceEstimates` | `[PriceEstimate]` | Fare estimates for a route |
| `timeEstimates` | `[TimeEstimate]` | ETA estimates by product |
| `ride` | `RideDetails` | Fetch a specific ride request |
| `rideHistory` | `RideHistory` | Paginated trip history for a rider |
| `driverProfile` | `DriverDetails` | Fetch driver profile |
| `driverTrips` | `[DriverTrip]` | Trips completed by a driver |
| `driverPayments` | `[PayoutDetail]` | Payment history for a driver |
| `restaurant` | `UberEatsRestaurant` | Fetch an Eats store |
| `menu` | `Menu` | Fetch menu for a store |
| `order` | `UberEatsOrder` | Fetch an Eats order |
| `delivery` | `Delivery` | Fetch a Direct delivery |
| `deliveryQuote` | `DeliveryQuote` | Quote a Direct delivery |
| `organization` | `Organization` | Fetch a Direct organization |
| `businessLocation` | `BusinessLocation` | Fetch a Direct business location |
| `voucherProgram` | `VoucherProgram` | Fetch a voucher program |
| `voucherCode` | `VoucherCode` | Fetch a voucher code |
| `businessTrips` | `[BusinessTrip]` | Trips for a business account |
| `businessReceipt` | `Receipt` | Fetch a business trip receipt |
| `webhooks` | `[Webhook]` | List registered webhooks |

### Mutation

| Field | Return Type | Description |
|---|---|---|
| `createRideRequest` | `TripRequest` | Request a ride |
| `cancelRideRequest` | `Boolean` | Cancel a pending ride |
| `updatePlace` | `Place` | Update a saved place |
| `createDelivery` | `Delivery` | Create a Direct delivery |
| `cancelDelivery` | `Boolean` | Cancel a delivery |
| `createDeliveryQuote` | `DeliveryQuote` | Create a delivery quote |
| `createRefund` | `Refund` | Request a delivery refund |
| `updateStore` | `UberEatsRestaurant` | Update an Eats store |
| `updateMenu` | `Menu` | Upsert a full menu |
| `acceptOrder` | `UberEatsOrder` | Accept an incoming Eats order |
| `denyOrder` | `UberEatsOrder` | Deny an incoming Eats order |
| `cancelOrder` | `UberEatsOrder` | Cancel an Eats order |
| `createVoucherProgram` | `VoucherProgram` | Create a voucher program |
| `createVoucherCodes` | `[VoucherCode]` | Generate voucher codes |
| `registerWebhook` | `Webhook` | Register a webhook endpoint |
| `deleteWebhook` | `Boolean` | Remove a webhook endpoint |

### Subscription

| Field | Return Type | Description |
|---|---|---|
| `deliveryStatusUpdated` | `DeliveryEvent` | Real-time delivery status changes |
| `courierLocationUpdated` | `CourierLocation` | Courier GPS position stream |
| `orderStatusUpdated` | `OrderEvent` | Eats order lifecycle events |

## Type Summary

See `uber-schema.graphql` for the full SDL. The schema defines 72 named types across the following domains:

| Domain | Types |
|---|---|
| Rides & Products | `Product`, `ProductAvailability`, `PriceEstimate`, `TimeEstimate`, `TripRequest`, `TripDetails`, `TripStatus`, `Ride`, `RideDetails`, `RideHistory`, `RideEstimate`, `Place` |
| Drivers | `Driver`, `DriverDetails`, `DriverRating`, `DriverTrip` |
| Vehicles | `Vehicle`, `VehicleDetails` |
| Routing & Geo | `Route`, `Waypoint`, `Location`, `PolyLine`, `Bearing` |
| Surge Pricing | `Surge`, `SurgeArea`, `SurgeMultiplier` |
| Payments | `PaymentMethod`, `CreditCard`, `PaypalAccount`, `Money`, `Currency`, `Receipt`, `PayoutDetail` |
| Promotions | `PromoCode`, `ReferralCode`, `VoucherProgram`, `VoucherTemplate`, `VoucherCode`, `VoucherProgramRequest` |
| Ratings & Reviews | `Rating`, `Review` |
| Business | `BusinessProfile`, `BusinessMembership`, `Organization`, `BusinessLocation`, `BusinessTrip` |
| Uber Eats | `UberEatsRestaurant`, `Menu`, `MenuCategory`, `MenuItem`, `MenuItemModifierGroup`, `MenuItemModifier`, `UberEatsOrder`, `OrderItem`, `OrderReceipt` |
| Uber Direct | `Delivery`, `DeliveryStatus`, `DeliveryTracking`, `DeliveryQuote`, `CourierLocation`, `PickupDetails`, `DropoffDetails`, `Refund`, `RefundRequest` |
| Uber Freight | `FreightShipment`, `BidRequest`, `Carrier`, `CarrierProfile`, `LoadBoard`, `TruckingSpot` |
| Webhooks & Events | `Webhook`, `WebhookEvent`, `DeliveryEvent`, `OrderEvent` |
| Health Transport | `UberHealthRide`, `UberHealthPatient` |
