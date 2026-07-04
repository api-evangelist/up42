# UP42 (up42)

UP42 is a geospatial marketplace and developer platform for Earth observation (EO) data and analytics, operated by Airbus Defence and Space. It lets you search a global archive of satellite and aerial imagery (Catalog), task new satellite acquisitions on demand (Tasking), place and track Orders, store and download results as cloud-native Assets, and browse everything through a STAC-compliant data management API. Delivery, ordering, and storage are exposed over a documented REST API at `https://api.up42.com`, authenticated with OAuth2 access tokens (obtained from an API key or account credentials), and are also wrapped by an official Python SDK. Storage is powered by STAC and the cloud-native asset model, and job/order status changes can be pushed to consumer endpoints via webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/up42/refs/heads/main/apis.yml)

## Tags

- Geospatial
- Earth Observation
- Satellite Imagery
- Remote Sensing
- STAC
- Tasking
- Catalog
- Airbus

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### UP42 Catalog API

Search the UP42 archive of previously captured satellite and aerial imagery. List geospatial collections, run STAC searches against a host's catalog, and retrieve quicklook and thumbnail previews before placing an order for immediate delivery.

- **Human URL:** [https://docs.up42.com/developers/api-catalog](https://docs.up42.com/developers/api-catalog)
- **Base URL:** `https://api.up42.com`

#### Tags

- Catalog
- Archive
- Search
- STAC

#### Properties

- [Documentation](https://docs.up42.com/developers/api-catalog)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/up42.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/up42.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### UP42 Tasking API

Commission new satellite acquisitions on demand. List tasking collections and opportunities, request feasibility studies, review and accept quotations, and create tasking orders scoped to a workspace and area of interest.

- **Human URL:** [https://docs.up42.com/developers/api-tasking](https://docs.up42.com/developers/api-tasking)
- **Base URL:** `https://api.up42.com`

#### Tags

- Tasking
- Acquisition
- Feasibility
- Quotations

#### Properties

- [Documentation](https://docs.up42.com/developers/api-tasking)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### UP42 Orders API

Estimate, place, and track catalog and tasking orders. Get a JSON schema for an order form, estimate the credit cost, create an order under a workspace, list and retrieve orders, update or cancel an order, and inspect order coverage.

- **Human URL:** [https://docs.up42.com/developers/api](https://docs.up42.com/developers/api)
- **Base URL:** `https://api.up42.com`

#### Tags

- Orders
- Estimate
- Fulfillment

#### Properties

- [Documentation](https://docs.up42.com/developers/api)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### UP42 Storage Assets API

List and retrieve the geospatial assets produced by completed catalog and tasking orders, inspect asset and STAC item metadata, and generate a pre-signed download URL to fetch the underlying files without additional authentication.

- **Human URL:** [https://docs.up42.com/developers/api-assets](https://docs.up42.com/developers/api-assets)
- **Base URL:** `https://api.up42.com`

#### Tags

- Storage
- Assets
- Download

#### Properties

- [Documentation](https://docs.up42.com/developers/api-assets)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### UP42 STAC Data Management API

A STAC-compliant (SpatioTemporal Asset Catalog) view of everything in your UP42 storage. Browse the STAC landing page and conformance, list and get STAC collections and items, update item titles and tags, discover queryables, and run a cross-storage STAC search.

- **Human URL:** [https://docs.up42.com/developers/api-stac](https://docs.up42.com/developers/api-stac)
- **Base URL:** `https://api.up42.com`

#### Tags

- STAC
- Data Management
- Collections
- Items

#### Properties

- [Documentation](https://docs.up42.com/developers/api-stac)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### UP42 Processing API

Run advanced analytics and processing over geospatial assets in storage. List available processes, evaluate the cost and validity of a process against inputs, execute a process, and list and track the resulting processing jobs.

- **Human URL:** [https://docs.up42.com/processing/getting-started](https://docs.up42.com/processing/getting-started)
- **Base URL:** `https://api.up42.com`

#### Tags

- Processing
- Analytics
- Jobs

#### Properties

- [Documentation](https://docs.up42.com/processing/getting-started)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### UP42 Webhooks API

Register HTTPS webhook endpoints that UP42 calls when order and job status changes occur. Create, list, get, update, and delete webhooks, list the available event types, and test a webhook with a sample payload. Server-to-endpoint HTTP callbacks, not a bidirectional WebSocket.

- **Human URL:** [https://docs.up42.com/help/webhooks](https://docs.up42.com/help/webhooks)
- **Base URL:** `https://api.up42.com`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.up42.com/help/webhooks)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### UP42 Workspaces and Account API

Read account and workspace context used across the platform. Retrieve the authenticated account, list workspaces, and (for enterprise accounts) inspect budgets that cap credit spend. Workspace IDs scope ordering, storage, and processing calls.

- **Human URL:** [https://docs.up42.com/developers/api](https://docs.up42.com/developers/api)
- **Base URL:** `https://api.up42.com`

#### Tags

- Workspaces
- Account
- Budgets

#### Properties

- [Documentation](https://docs.up42.com/developers/api)
- [API Reference](https://developer.up42.com/reference/overview)
- [OpenAPI](openapi/up42-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/up42)
- [LinkedIn](https://www.linkedin.com/company/up42)
- [Website](https://up42.com)
- [Documentation](https://docs.up42.com)
- [Plans](plans/up42-plans-pricing.yml)
- [Rate Limits](rate-limits/up42-rate-limits.yml)
- [Fin Ops](finops/up42-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
