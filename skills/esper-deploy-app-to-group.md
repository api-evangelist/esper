---
name: Upload an app and deploy it to a device group
description: Upload an application to an Esper enterprise and roll it out to a device group.
api: openapi/esper-manage-openapi-original.yml
operations: [upload, getAppVersions, getAllGroups, createGroup, runGroupCommand, getGroupCommand]
---

# Upload an app and deploy it to a device group

## Auth
- Base URL `https://<domain>-api.esper.cloud/api` under `/enterprise/<enterprise_id>/`.
- `Authorization: Bearer <ACCESS_TOKEN>`.

## Steps
1. **Upload the app** — call `upload` with `multipart/form-data` (set the correct `Content-Type`, or you get 415). This creates the application and its first version.
2. **Confirm the version** — call `getAppVersions` for the application to get the `version_id` to deploy.
3. **Pick or create the target group** — call `getAllGroups`; if none fits, `createGroup`.
4. **Deploy to the group** — call `runGroupCommand` with an install command referencing the app version; the command runs on all active devices in the group.
5. **Track rollout** — poll `getGroupCommand` for status.

## Conventions & errors
- Uploads require multipart; JSON bodies for commands.
- Errors: 415 (wrong Content-Type), 404 (unknown app/group), 401 (auth). See `errors/esper-problem-types.yml`.
