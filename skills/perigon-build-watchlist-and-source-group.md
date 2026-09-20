---
name: perigon-build-watchlist-and-source-group
description: Create reusable entity watchlists and source groups, then filter searches with them.
api: openapi/perigon-openapi.yml
operations:
- create-watchlist
- resolve-watchlists
- create-source-group
- resolve-source-groups
- search-companies
- search-people
- search-sources
- search-articles
generated: '2026-09-20'
method: generated
---

# Build a watchlist and a source group

Base URL `https://api.perigon.io`. Auth: `Authorization: Bearer <api key>` (also `x-api-key` header or `apiKey` query). See ../authentication/perigon-authentication.yml.

## Steps
1. Resolve entity ids with `search-companies` / `search-people` and domains with `search-sources`.
2. POST `create-watchlist` and `create-source-group`; check membership with `resolve-watchlists` / `resolve-source-groups`.
3. Filter `search-articles` by the saved source group. Deletes have no restore operation — confirm before calling delete.

## Rules
- No idempotency keys on writes: do not blind-retry POSTs; list first to check whether the resource was created (../conventions/perigon-conventions.yml).
- Errors use `{status, message, timestamp}`; a 500 is often a malformed query or date, a 403 is a plan restriction (../errors/perigon-problem-types.yml).
- Provider-published skills are saved verbatim in skills/provider/.
