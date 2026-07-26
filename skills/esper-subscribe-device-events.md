---
name: Subscribe to device events
description: Create an Esper event subscription to stream device events to an external (AWS) sink.
api: openapi/esper-manage-openapi-original.yml
operations: [createSubscription, getAllSubscriptions, getSubscription, getDeviceEvent, deleteSubscription]
---

# Subscribe to device events

Esper streams device telemetry/state events to an external sink via event subscriptions.

## Auth
- Base URL `https://<domain>-api.esper.cloud/api` under `/enterprise/<enterprise_id>/`.
- `Authorization: Bearer <ACCESS_TOKEN>`.

## Steps
1. **Create a subscription** — `createSubscription` with an `aws_account_id` (the target AWS account that will receive delivered events).
2. **List / verify** — `getAllSubscriptions` and `getSubscription` to confirm it is active.
3. **Read latest event** — `getDeviceEvent` returns the latest event for a device (useful for polling or reconciliation).
4. **Tear down** — `deleteSubscription` to stop delivery.

## Notes
- Delivery is push to an AWS sink; there is no generic HTTP webhook URL field — see `asyncapi/esper-events-webhooks.yml`.
- Errors return `{ errors:[], message, status }` (see `errors/esper-problem-types.yml`).
