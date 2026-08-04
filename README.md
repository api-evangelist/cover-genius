# Cover Genius (cover-genius)

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

Cover Genius is an insurtech company providing embedded insurance and protection at the point of sale. The XCover distribution API lets partners create insurance offers, confirm bookings, modify and cancel policies, and receive policy lifecycle webhooks, while the XClaim API handles claims intake and instant payments.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/apis.yml)

## Tags

- Insurance
- Insurtech
- Embedded Insurance
- Protection
- Claims

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### XCover Offers API

Creates real-time, context-aware insurance offers (quotes) for a partner's customers at the point of sale, returning priced products, localized content, and product disclosure documents.

- **Human URL:** [https://partner-docs.covergenius.com/offers/api/reference](https://partner-docs.covergenius.com/offers/api/reference)
- **Base URL:** `https://api.xcover.com/x`

#### Tags

- Offers
- Quotes
- Embedded Insurance

#### Properties

- [Documentation](https://partner-docs.covergenius.com/offers/guides/purchase-workflow-overview/create-offer)
- [API Reference](https://partner-docs.covergenius.com/offers/api/reference/create-offer)
- [OpenAPI](openapi/cover-genius-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cover-genius.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cover-genius.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### XCover Bookings and Policies API

Confirms offers into bound policies and retrieves, modifies (quote-for-update then confirm-update), and cancels bookings, with idempotency-key support on purchase operations.

- **Human URL:** [https://partner-docs.covergenius.com/offers/api/reference/confirm-offer](https://partner-docs.covergenius.com/offers/api/reference/confirm-offer)
- **Base URL:** `https://api.xcover.com/x`

#### Tags

- Bookings
- Policies
- Confirmation

#### Properties

- [Documentation](https://partner-docs.covergenius.com/offers/guides/purchase-workflow-overview)
- [API Reference](https://partner-docs.covergenius.com/offers/api/reference/confirm-offer)
- [OpenAPI](openapi/cover-genius-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cover-genius.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cover-genius.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### XClaim Claims API

Files new claims against a partner policy and lists existing claims, driving Cover Genius's automated claims assessment and instant payment experience.

- **Human URL:** [https://partner-docs.covergenius.com/xclaim](https://partner-docs.covergenius.com/xclaim)
- **Base URL:** `https://api.xclaim.xcover.com`

#### Tags

- Claims
- Payments
- Settlement

#### Properties

- [Documentation](https://partner-docs.covergenius.com/xclaim/readme)
- [API Reference](https://partner-docs.covergenius.com/xclaim/claims/create-a-new-claim)
- [OpenAPI](openapi/cover-genius-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### XCover Webhooks and Events

HTTP POST webhook callbacks notifying partner listener URLs of policy lifecycle events (BOOKING_CREATED, BOOKING_UPDATED, BOOKING_CANCELLED, and renewal events), HMAC-SHA256 signed for verification.

- **Human URL:** [https://partner-docs.covergenius.com/offers/api/webhooks](https://partner-docs.covergenius.com/offers/api/webhooks)
- **Base URL:** `https://api.xcover.com/x`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://partner-docs.covergenius.com/offers/api/webhooks)
- [API Reference](https://partner-docs.covergenius.com/xclaim/webhooks)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/cover-genius)
- [Website](https://www.covergenius.com)
- [Documentation](https://partner-docs.covergenius.com)
- [Plans](plans/cover-genius-plans-pricing.yml)
- [Rate Limits](rate-limits/cover-genius-rate-limits.yml)
- [Fin Ops](finops/cover-genius-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
