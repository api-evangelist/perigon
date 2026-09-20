---
name: perigon-semantic-search-and-summarize
description: Run natural-language vector search over news or Wikipedia and synthesize an answer with citations. Use when keywords are unknown or a summary is wanted.
api: openapi/perigon-openapi.yml
operations:
- vector-search-articles
- vector-search-wikipedia
- search-summarizer
generated: '2026-09-20'
method: generated
---

# Semantic search and AI summary

Base URL `https://api.perigon.io`. Auth: `Authorization: Bearer <api key>` (also `x-api-key` header or `apiKey` query). See ../authentication/perigon-authentication.yml.

## Steps
1. POST `vector-search-articles` with a natural-language `prompt` and optional filters.
2. Optionally ground entities with POST `vector-search-wikipedia`.
3. POST `search-summarizer` (/v1/summarize) with the same query filters to get a synthesized summary of matching coverage.

## Rules
- No idempotency keys on writes: do not blind-retry POSTs; list first to check whether the resource was created (../conventions/perigon-conventions.yml).
- Errors use `{status, message, timestamp}`; a 500 is often a malformed query or date, a 403 is a plan restriction (../errors/perigon-problem-types.yml).
- Provider-published skills are saved verbatim in skills/provider/.
