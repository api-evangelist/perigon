---
name: perigon-check-usage-and-keys
description: Read plan limits and remaining quota before a bulk job. Use as a pre-flight and health check.
api: openapi/perigon-openapi.yml
operations:
- get-limits
generated: '2026-09-20'
method: generated
---

# Check usage, limits and key validity

Base URL `https://api.perigon.io`. Auth: `Authorization: Bearer <api key>` (also `x-api-key` header or `apiKey` query). See ../authentication/perigon-authentication.yml.

## Steps
1. GET `get-limits` (/v1/limits) — quota-exempt and not rate-limited. Read `requestsUsed`, `requestLimit`, `maxPageSize`, `paginationLimit`, `resetAt`.
2. Pass `apiKeys` (up to 50) to verify keys are valid and active.
3. Size the job to the remaining quota and the plan req/sec limit; on 429 honor `Retry-After` and read `RateLimit` / `RateLimit-Policy`.

## Rules
- No idempotency keys on writes: do not blind-retry POSTs; list first to check whether the resource was created (../conventions/perigon-conventions.yml).
- Errors use `{status, message, timestamp}`; a 500 is often a malformed query or date, a 403 is a plan restriction (../errors/perigon-problem-types.yml).
- Provider-published skills are saved verbatim in skills/provider/.
