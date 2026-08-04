# Bored API (bored)

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

The Bored API is a free, open-source, no-authentication public API that serves suggestions for things to do when you are bored. The canonical reference implementation is an MEVN (MongoDB / Express / Vue / Node) project maintained by Drew Thoennes at github.com/drewthoennes/Bored-API (MIT licensed). The historically hosted instance at https://www.boredapi.com/ has been intermittently or fully unreachable since June 2024 (originally hosted on Heroku); a community fork maintained by The App Brewery at https://bored-api.appbrewery.com remains actively available for students and consumers. This profile documents the v1 surface (legacy activities-only), the v2 surface (activities + facts + riddles + websites + suggestions), and the App Brewery community mirror, so the API contract is preserved as a historical, self-hostable artifact.

**APIs.json:** [https://github.com/drewthoennes/Bored-API](https://github.com/drewthoennes/Bored-API)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Activities
- Boredom
- Community
- Development
- Discovery
- Education
- Facts
- Free
- MEVN
- No Auth
- Open Source
- Public APIs
- Recreation
- Riddles
- Suggestions
- Websites

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Bored API (Canonical)

Canonical Drew Thoennes Bored API surface, covering v1 (legacy activities) and v2 (activities + facts + riddles + websites + suggestions). No authentication. The hosted instance at www.boredapi.com has been unreliable since 2024; the spec is preserved for self-hosting.

- **Human URL:** [https://github.com/drewthoennes/Bored-API](https://github.com/drewthoennes/Bored-API)
- **Base URL:** `https://www.boredapi.com`

#### Tags

- Activities
- Facts
- Riddles
- Websites
- Suggestions
- REST
- No Auth

#### Properties

- [Documentation](https://github.com/drewthoennes/Bored-API#readme)
- [Source Code](https://github.com/drewthoennes/Bored-API)
- [OpenAPI](openapi/bored-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bored-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bored-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bored-activity-v1-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bored-activity-v2-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bored-fact-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bored-riddle-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bored-website-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bored-suggestion-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/bored-activity-v1-structure.json)
- [JSON Structure](json-structure/bored-activity-v2-structure.json)
- [JSON Structure](json-structure/bored-fact-structure.json)
- [JSON Structure](json-structure/bored-riddle-structure.json)
- [JSON Structure](json-structure/bored-website-structure.json)
- [Example](examples/bored-api-get-random-activity-v1-example.json)
- [Example](examples/bored-api-get-random-activity-v1-filtered-example.json)
- [Example](examples/bored-api-get-random-activity-v2-example.json)
- [Example](examples/bored-api-get-activity-by-key-v2-example.json)
- [Example](examples/bored-api-get-random-fact-example.json)
- [Example](examples/bored-api-get-random-riddle-example.json)
- [Example](examples/bored-api-get-random-website-example.json)
- [Example](examples/bored-api-submit-suggestion-example.json)

### Bored API (App Brewery Community Fork)

Community-hosted mirror of the Bored API maintained by The App Brewery for their web development course. Provides a flattened path scheme (/random, /filter, /activity/{key}) on bored-api.appbrewery.com and is rate-limited to 100 requests per 15 minutes. No authentication.

- **Human URL:** [https://bored-api.appbrewery.com/](https://bored-api.appbrewery.com/)
- **Base URL:** `https://bored-api.appbrewery.com`

#### Tags

- Activities
- Community Fork
- Education
- REST
- No Auth

#### Properties

- [Documentation](https://bored-api.appbrewery.com/)
- [OpenAPI](openapi/bored-appbrewery-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bored-appbrewery.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bored-appbrewery.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Rate Limits](https://bored-api.appbrewery.com/)
- [Example](examples/bored-appbrewery-get-random-example.json)
- [Example](examples/bored-appbrewery-filter-example.json)

## Common Properties

- [Website](https://www.boredapi.com/)
- [Portal](https://bored-api.appbrewery.com/)
- [Git Hub](https://github.com/drewthoennes/Bored-API)
- [Source Code](https://github.com/drewthoennes/Bored-API)
- [Documentation](https://github.com/drewthoennes/Bored-API#readme)
- [License](https://github.com/drewthoennes/Bored-API/blob/master/license)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [SDK](https://pypi.org/project/bored/)
- [SDK](https://pypi.org/project/bored-api/)
- [SDK](https://gitlab.com/CMDR_Tvis/bored-api)
- [JSON-LD](json-ld/bored-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/bored-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)
- [Vocabulary](vocabulary/bored-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
