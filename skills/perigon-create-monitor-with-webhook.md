---
name: perigon-create-monitor-with-webhook
description: Create a webhook contact point, create and activate a monitor, then read its events. Use to set up real-time alerting.
api: openapi/perigon-openapi.yml
operations:
- create-contact-point
- get-contact-point
- create-monitor-api
- activate-monitor-api
- list-monitor-events-api
- pause-monitor-api
- archive-monitor-api
generated: '2026-09-20'
method: generated
---

# Create a monitor that delivers to a webhook

Base URL `https://api.perigon.io`. Auth: `Authorization: Bearer <api key>` (also `x-api-key` header or `apiKey` query). See ../authentication/perigon-authentication.yml.

## Steps
1. POST `create-contact-point` with the HTTPS webhook URL; read `webhookSecret` via `get-contact-point` and store it as a secret.
2. POST `create-monitor-api` (DRAFT or ACTIVE) referencing the contact point; `activate-monitor-api` if created as a draft.
3. Verify deliveries with the `Perigon-Signature` header: HMAC_SHA256(secret, "<t>.<raw body>"); dedupe on `signal_notification_id` (stable across the up-to-3 delivery attempts).
4. Poll `list-monitor-events-api` for structured events. `pause-monitor-api` is reversible via `activate-monitor-api`; `archive-monitor-api` is irreversible — confirm with the user first.

## Rules
- No idempotency keys on writes: do not blind-retry POSTs; list first to check whether the resource was created (../conventions/perigon-conventions.yml).
- Errors use `{status, message, timestamp}`; a 500 is often a malformed query or date, a 403 is a plan restriction (../errors/perigon-problem-types.yml).
- Provider-published skills are saved verbatim in skills/provider/.
