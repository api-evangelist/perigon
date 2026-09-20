---
name: perigon-search-news-and-stories
description: Search enriched articles, pivot to the story cluster, and pull its history. Use when an agent needs current or historical news coverage as structured data.
api: openapi/perigon-openapi.yml
operations:
- search-articles
- search-stories
- get-story-history
- get-story-counts
generated: '2026-09-20'
method: generated
---

# Search news articles and clustered stories

Base URL `https://api.perigon.io`. Auth: `Authorization: Bearer <api key>` (also `x-api-key` header or `apiKey` query). See ../authentication/perigon-authentication.yml.

## Steps
1. Call `search-articles` (GET /v1/articles/all) with `q`, `from`/`to` (YYYY-MM-DD) and filters; page with `page` (zero-indexed) and `size` (max 100; 10,000-record ceiling — narrow by date range beyond that).
2. Take a `clusterId` from an article and call `search-stories` (GET /v1/stories/all) to get the cluster summary and counts.
3. Call `get-story-history` for the timeline of a story and `get-story-counts` for volume stats.

## Rules
- No idempotency keys on writes: do not blind-retry POSTs; list first to check whether the resource was created (../conventions/perigon-conventions.yml).
- Errors use `{status, message, timestamp}`; a 500 is often a malformed query or date, a 403 is a plan restriction (../errors/perigon-problem-types.yml).
- Provider-published skills are saved verbatim in skills/provider/.
