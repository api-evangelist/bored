# Bored API

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

> **No longer operating.** This company or product has shut down, been discontinued, or been deprecated. This profile is kept as a historical record and is not maintained or rated.

**Status:** hosted-instance-deprecated

The Bored API is a free, open-source, no-authentication public API that serves suggestions for things to do when you are bored. The canonical reference implementation is an MEVN (MongoDB / Express / Vue / Node) project maintained by Drew Thoennes at github.com/drewthoennes/Bored-API (MIT licensed). The historically hosted instance at https://www.boredapi.com/ has been intermittently or fully unreachable since June 2024 (originally hosted on Heroku); a community fork maintained by The App Brewery at https://bored-api.appbrewery.com remains actively available for students and consumers. This profile documents the v1 surface (legacy activities-only), the v2 surface (activities + facts + riddles + websites + suggestions), and the App Brewery community mirror, so the API contract is preserved as a historical, self-hostable artifact.

**Areas:** Activities · Boredom · Community · Development · Discovery · Education · Facts · Free · MEVN · No Auth · Open Source · Public APIs

## Bored API on APIs.io (historical record)

Everything profiled for Bored API is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/bored/](https://apis.io/providers/bored/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [Bored API Activities API](https://apis.io/apis/bored/bored-activities-api/) — Random and filtered activity suggestions.
- [Bored API Facts API](https://apis.io/apis/bored/bored-facts-api/) — Random or keyed factual snippets (v2 only).
- [Bored API Riddles API](https://apis.io/apis/bored/bored-riddles-api/) — Random or keyed riddles with difficulty filter (v2 only).
- [Bored API Suggestions API](https://apis.io/apis/bored/bored-suggestions-api/) — Community-submitted content suggestions for review (v2 only).
- [Bored API Websites API](https://apis.io/apis/bored/bored-websites-api/) — Random or keyed website recommendations (v2 only).

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Bored Agentic Access](https://apis.io/agentic-access/bored/bored-agentic-access/)

#### JSON Schema (6)

The data models the API reads and writes.

- [BoredActivityV1](https://apis.io/schemas/bored/bored-activity-v1/)
- [BoredActivityV2](https://apis.io/schemas/bored/bored-activity-v2/)
- [BoredFact](https://apis.io/schemas/bored/bored-fact/)
- [BoredRiddle](https://apis.io/schemas/bored/bored-riddle/)
- [BoredSuggestion](https://apis.io/schemas/bored/bored-suggestion/)
- [BoredWebsite](https://apis.io/schemas/bored/bored-website/)

#### JSON Structure (5)

Data models expressed in JSON Structure.

- [Bored Activity V1 Structure](https://apis.io/json-structure/bored/bored-activity-v1-structure/)
- [Bored Activity V2 Structure](https://apis.io/json-structure/bored/bored-activity-v2-structure/)
- [Bored Fact Structure](https://apis.io/json-structure/bored/bored-fact-structure/)
- [Bored Riddle Structure](https://apis.io/json-structure/bored/bored-riddle-structure/)
- [Bored Website Structure](https://apis.io/json-structure/bored/bored-website-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Bored Context](https://apis.io/jsonld/bored/bored-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Bored API Vocabulary](https://apis.io/vocabularies/bored/bored-vocabulary/)

#### Examples (10)

Example requests and responses.

- [Bored Api Get Activity By Key V2 Example](https://apis.io/examples/bored/bored-api-get-activity-by-key-v2-example/)
- [Bored Api Get Random Activity V1 Example](https://apis.io/examples/bored/bored-api-get-random-activity-v1-example/)
- [Bored Api Get Random Activity V1 Filtered Example](https://apis.io/examples/bored/bored-api-get-random-activity-v1-filtered-example/)
- [Bored Api Get Random Activity V2 Example](https://apis.io/examples/bored/bored-api-get-random-activity-v2-example/)
- [Bored Api Get Random Fact Example](https://apis.io/examples/bored/bored-api-get-random-fact-example/)
- [Bored Api Get Random Riddle Example](https://apis.io/examples/bored/bored-api-get-random-riddle-example/)
- [Bored Api Get Random Website Example](https://apis.io/examples/bored/bored-api-get-random-website-example/)
- [Bored Api Submit Suggestion Example](https://apis.io/examples/bored/bored-api-submit-suggestion-example/)
- [Bored Appbrewery Filter Example](https://apis.io/examples/bored/bored-appbrewery-filter-example/)
- [Bored Appbrewery Get Random Example](https://apis.io/examples/bored/bored-appbrewery-get-random-example/)

#### Collections (7)

Postman and Open Collection request collections.

- [Bored Activities API](https://apis.io/collections/bored/open-bored-activities-api/)
- [Bored API](https://apis.io/collections/bored/open-bored-api/)
- [Bored API (App Brewery Fork)](https://apis.io/collections/bored/open-bored-appbrewery/)
- [Bored Activities Facts API](https://apis.io/collections/bored/open-bored-facts-api/)
- [Bored Activities Riddles API](https://apis.io/collections/bored/open-bored-riddles-api/)
- [Bored Activities Suggestions API](https://apis.io/collections/bored/open-bored-suggestions-api/)
- [Bored Activities Websites API](https://apis.io/collections/bored/open-bored-websites-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Bored API — jsonschema rules](https://apis.io/rules/bored/bored-jsonschema-spectral-rules/)
- [Bored API API Rules](https://apis.io/rules/bored/bored-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Bored Domain Security](https://apis.io/security/bored/bored-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.boredapi.com/)
- [Documentation](https://github.com/drewthoennes/Bored-API#readme)

## API Evangelist rating

**Not rated** — this company is recorded as no longer operating, so no score is published. If it is in fact operating, say so on this repository and it will be re-profiled.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Bored API: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/bored/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
