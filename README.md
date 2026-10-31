# Perigon

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

Perigon is a real-time global news data and intelligence platform. It provides structured, enriched news data from 200,000+ sources worldwide through REST APIs — articles, clustered stories, AI search summaries, semantic vector search, sources, companies, people, journalists, topics and Wikipedia — plus Signals, an AI-driven monitoring product with monitors, watchlists, contact points and signed webhooks. Perigon publishes an OpenAPI description, a hosted remote MCP server, official TypeScript, Python and Go SDKs, Agent Skills, and an API versioning and deprecation policy.

**Areas:** Company · News · Media Monitoring · Search · Artificial Intelligence · Data · MCP · Webhook

## Perigon on APIs.io

Everything profiled for Perigon is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/perigon/](https://apis.io/providers/perigon/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Perigon MCP Server](https://apis.io/apis/perigon/perigon-mcp/) — Hosted remote Model Context Protocol server (Streamable HTTP, with an SSE variant) exposing Perigon news search, analytics and monitor tools to AI clients.…
- [Perigon AI & Advanced Search API](https://apis.io/apis/perigon/perigon-ai-advanced-search-api/) — These endpoints enable semantic search beyond traditional keyword matching, content summarization, and advanced information retrieval across articles
- [Perigon Contact Points API](https://apis.io/apis/perigon/perigon-contact-points-api/) — Manage contact points used to deliver monitor notifications. Contact points define where and how monitor events are delivered (e.g. webhooks). Only WEBHOOK…
- [Perigon Monitors API](https://apis.io/apis/perigon/perigon-monitors-api/) — Manage AI Monitors — configurable monitors that continuously scan news content for topics, entities, and events of interest. Monitors run asynchronously and…
- [Perigon News & Stories API](https://apis.io/apis/perigon/perigon-news-stories-api/) — Endpoints for accessing news articles and stories
- [Perigon Source Groups API](https://apis.io/apis/perigon/perigon-source-groups-api/) — Manage custom source groups for organizing and filtering news sources. Source groups allow grouping domains together for use in search queries and monitors.
- [Perigon Supplemental Endpoints API](https://apis.io/apis/perigon/perigon-supplemental-endpoints-api/) — Additional endpoints for metadata and related information
- [Perigon Utilities API](https://apis.io/apis/perigon/perigon-utilities-api/) — The Utilities API from Perigon — 1 operation(s) for utilities.
- [Perigon Watchlists API](https://apis.io/apis/perigon/perigon-watchlists-api/) — Manage watchlists of people and companies for use with monitors. Watchlists can contain up to 100 combined entities and are used to track mentions across…
- [Perigon Wikipedia API](https://apis.io/apis/perigon/perigon-wikipedia-api/) — Endpoints for searching ingested Wikipedia content. Provides keyword and filtered search capabilities along with vector-based semantic search across…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Perigon Webhooks](https://apis.io/asyncapis/perigon/perigon-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Perigon MCP](https://apis.io/servers/perigon/io-perigon-mcp/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Perigon Agentic Access](https://apis.io/agentic-access/perigon/perigon-agentic-access/)

#### Overlays (10)

OpenAPI overlays, including conversational phrasing for each operation.

- [Perigon Ai Advanced Search Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-ai-advanced-search-api-phrasing-overlay/)
- [Perigon Contact Points Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-contact-points-api-phrasing-overlay/)
- [Perigon Monitors Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-monitors-api-phrasing-overlay/)
- [Perigon News Stories Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-news-stories-api-phrasing-overlay/)
- [Perigon Openapi Overlay](https://apis.io/overlays/perigon/perigon-openapi-overlay/)
- [Perigon Source Groups Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-source-groups-api-phrasing-overlay/)
- [Perigon Supplemental Endpoints Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-supplemental-endpoints-api-phrasing-overlay/)
- [Perigon Utilities Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-utilities-api-phrasing-overlay/)
- [Perigon Watchlists Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-watchlists-api-phrasing-overlay/)
- [Perigon Wikipedia Api Phrasing Overlay](https://apis.io/overlays/perigon/perigon-wikipedia-api-phrasing-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Perigon Authentication](https://apis.io/security/perigon/perigon-authentication/)
- [Perigon Domain Security](https://apis.io/security/perigon/perigon-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Perigon Plans Pricing](https://apis.io/plans/perigon/perigon-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Perigon Rate Limits](https://apis.io/rate-limits/perigon/perigon-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://perigon.io/)
- [Documentation](https://perigon.io/docs/api/intro)
- [Getting started](https://perigon.io/docs/api/getting-started)
- [API reference](https://perigon.io/reference)
- [Pricing](https://perigon.io/products/pricing/apis)
- [Sign up](https://perigon.io/sign-up)
- [Support](https://perigon.io/contact)
- [Blog](https://perigon.io/blog)
- [Terms of service](https://perigon.io/terms)
- [Privacy policy](https://perigon.io/privacy)
- [GitHub](https://github.com/goperigon)
- [Status](https://status.perigon.io/)

## API Evangelist rating

**Kin Score 67.2** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 65.0 |
| Contract governance | 18.2 |
| Operational transparency | 84.2 |
| Developer ergonomics | 73.2 |
| Access clarity | 76.3 |

**Agent readiness 53.8** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly (partial credit) |

**Regulatory alignment 22.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/perigon/](https://apis.io/providers/perigon/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Perigon: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/perigon/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
