# Bored API (bored)

The Bored API is a free, open-source, no-authentication public API that returns suggestions for things to do when you are bored. The canonical reference implementation is an MEVN (MongoDB / Express / Vue / Node) project maintained by Drew Thoennes at [github.com/drewthoennes/Bored-API](https://github.com/drewthoennes/Bored-API) (MIT licensed).

**APIs.yml:** [apis.yml](apis.yml)

## Status

> The historically hosted instance at `https://www.boredapi.com/` has been intermittently or fully unreachable since June 2024 (originally hosted on Heroku). The reference implementation remains open source and can be self-hosted. The community fork maintained by The App Brewery at `https://bored-api.appbrewery.com` is the actively maintained hosted mirror.

| Surface | Host | Status |
|---|---|---|
| Canonical | `https://www.boredapi.com/` | Hosted instance deprecated / unreliable; self-host from source |
| Canonical (source) | [github.com/drewthoennes/Bored-API](https://github.com/drewthoennes/Bored-API) | MIT licensed, actively reachable |
| Community fork | `https://bored-api.appbrewery.com/` | Active, rate-limited to 100 req / 15 min |

## Type
- **x-type:** opensource
- **License:** MIT
- **Stack:** MEVN (MongoDB, Express.js, Vue.js, Node.js)
- **Authentication:** None
- **x-tier:** 3 (bulk-registered from public-apis)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Development

## APIs
- **Bored API (Canonical)** — Drew Thoennes implementation, v1 + v2 surfaces. [OpenAPI](openapi/bored-api-openapi.yml)
- **Bored API (App Brewery Community Fork)** — Hosted mirror with flatter path scheme. [OpenAPI](openapi/bored-appbrewery-openapi.yml)

## Endpoints (Canonical)

**V1 — Activities**
- `GET /api/activity` — Get a random activity (also at `/api/v1/activity`).
  - Query: `type`, `participants`, `minparticipants`, `maxparticipants`, `price`, `minprice`, `maxprice`, `accessibility`, `minaccessibility`, `maxaccessibility`, `key`

**V2 — Activities, Facts, Riddles, Websites, Suggestions**
- `GET /api/v2/activities` and `GET /api/v2/activities/{key}`
- `GET /api/v2/facts` and `GET /api/v2/facts/{key}`
- `GET /api/v2/riddles` (filter: `difficulty=easy|normal|hard`) and `GET /api/v2/riddles/{key}`
- `GET /api/v2/websites` and `GET /api/v2/websites/{key}`
- `POST /api/v2/suggestions` (exactly one of activity, fact, riddle, website)

## Endpoints (App Brewery Fork)
- `GET /random` — Random activity (no params)
- `GET /filter?type=&participants=` — Filtered activity list
- `GET /activity/{key}` — Activity by key

## Entities

- **Activity** — `activity`, `type`, `participants`, `price`, `accessibility`/`availability`, `duration`, `kidFriendly`, `link`, `key`
- **Fact** — `fact`, `source`, `key`
- **Riddle** — `question`, `answer`, `difficulty`, `source`, `key`
- **Website** — `url`, `description`, `key`
- **Suggestion** — community-submitted wrapper for any of the above

Canonical activity types: `charity`, `cooking`, `music`, `diy`, `education`, `social`, `busywork`, `recreational`, `relaxation`.

## Artifacts

| Folder | Files |
|---|---|
| [openapi/](openapi/) | `bored-api-openapi.yml`, `bored-appbrewery-openapi.yml` |
| [json-schema/](json-schema/) | activity-v1, activity-v2, fact, riddle, website, suggestion |
| [json-structure/](json-structure/) | activity-v1, activity-v2, fact, riddle, website |
| [json-ld/](json-ld/) | `bored-context.jsonld` |
| [examples/](examples/) | 10 request/response samples across v1, v2, and App Brewery mirror |
| [capabilities/](capabilities/) | activities, facts, riddles, websites, suggestions, appbrewery-activities |
| [rules/](rules/) | `bored-rules.yml` — Spectral linting rules |
| [vocabulary/](vocabulary/) | `bored-vocabulary.yml` |

## Tags
Activities, Boredom, Community, Development, Discovery, Education, Facts, Free, MEVN, No Auth, Open Source, Public APIs, Recreation, Riddles, Suggestions, Websites

## Notable Integrations and Wrappers

- [Bored — Find What to Do (iOS)](https://apps.apple.com/us/app/bored-find-what-to-do/id1475656469)
- ["I'm Bored" Alexa skill](https://www.amazon.com/gp/product/B07GDL9MP4)
- [bored (PyPI)](https://pypi.org/project/bored/) — Python wrapper
- [bored-api (PyPI)](https://pypi.org/project/bored-api/) — alternate Python wrapper
- [CMDR_Tvis bored-api (Kotlin)](https://gitlab.com/CMDR_Tvis/bored-api)
- [The App Brewery Web Dev course](https://bored-api.appbrewery.com/) — uses this API as teaching surface

## Notes
This entry was bulk-registered as part of a public-apis catalog sweep on 2026-05-28 and fully enriched on 2026-05-30 with OpenAPI specs, JSON Schemas, JSON Structures, JSON-LD context, Spectral rules, vocabulary, examples, and Naftiko capabilities for both the canonical Drew Thoennes implementation and the App Brewery community fork.

## Timestamps
- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## Maintainers
- **Kin Lane** — kin@apievangelist.com
