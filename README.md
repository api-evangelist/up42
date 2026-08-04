# UP42 (up42)

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
