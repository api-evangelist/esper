---
name: Manage device groups
description: Create, read, update and delete Esper device groups used for bulk device operations.
api: openapi/esper-manage-openapi-original.yml
operations: [getAllGroups, createGroup, getGroupById, updateGroup, deleteGroup]
---

# Manage device groups

Device groups are named collections of devices that group commands and policies target in bulk.

## Auth
- Base URL `https://<domain>-api.esper.cloud/api` under `/enterprise/<enterprise_id>/`.
- `Authorization: Bearer <ACCESS_TOKEN>`.

## Steps
1. **List groups** — `getAllGroups` with `limit`/`offset` paging.
2. **Create a group** — `createGroup` with the group name/attributes.
3. **Inspect** — `getGroupById` with the group UUID.
4. **Update** — `updateGroup` (full, PUT) or use the partial-update variant for a subset of fields.
5. **Delete** — `deleteGroup` when the group is no longer needed.

## Conventions & errors
- Pagination and error envelope per `conventions/esper-conventions.yml` and `errors/esper-problem-types.yml`.
- 404 on unknown group id; 403 if the key lacks access to the enterprise.
