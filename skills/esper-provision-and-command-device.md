---
name: Find a device and run a command on it
description: Locate a device in an Esper enterprise and issue a Commands V2 command, then track its status.
api: openapi/esper-manage-openapi-original.yml
operations: [getAllDevices, getDeviceById, createCommand, getCommandRequestStatus, getDeviceCommandHistory]
---

# Find a device and run a command on it

Use the Esper Manage API to locate a dedicated device and run a remote command.

## Auth
- Base URL: `https://<domain>-api.esper.cloud/api`, scoped to `/enterprise/<enterprise_id>/`.
- Send `Authorization: Bearer <ACCESS_TOKEN>` (tenant API key from the Esper Dev Console) and `Content-Type: application/json`.

## Steps
1. **Find the device** — call `getAllDevices` with filters (`name`, `serial`, `imei`, `group`, `search`) and `limit`/`offset` paging. Read `results[]`, `count`, `next`.
2. **Confirm details** — call `getDeviceById` with the device UUID to verify state before acting.
3. **Issue the command** — call `createCommand` (Commands V2) with the target device set and command payload. Prefer V2 over the deprecated V0/V1 Commands surface.
4. **Track status** — poll `getCommandRequestStatus` for the command request; use `getDeviceCommandHistory` for the device's past commands.

## Conventions & errors
- Pagination: `limit`/`offset` → `count`/`next`/`previous`/`results` (see `conventions/esper-conventions.yml`).
- No idempotency-key contract — do not blindly retry `createCommand`; check status first.
- Errors return `{ errors:[], message, status }`; 401 = bad/missing key, 404 = unknown device (see `errors/esper-problem-types.yml`).
