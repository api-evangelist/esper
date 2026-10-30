# Esper

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

Esper is the DevOps platform for connected devices, providing cloud-based Android (and edge) device management, application deployment, and remote orchestration for dedicated-device fleets. The Esper Manage REST API lets developers programmatically provision, monitor, and control Android-based dedicated devices running the Esper agent: manage devices and device groups, upload and roll out applications and versions, run device and group commands, configure compliance and enterprise policies, set up geofences, manage content, and subscribe to device events via webhooks. APIs are authenticated with a Bearer API key and served per-tenant on a dedicated Esper Cloud environment, with an official Python SDK (esperclient) and CLI.

**Areas:** Device Management · Mobile Device Management · Android · DevOps · IoT · Fleet Management · Enterprise Mobility · Edge Computing · Kiosk

## Esper on APIs.io

Everything profiled for Esper is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/esper/](https://apis.io/providers/esper/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [Esper Application API](https://apis.io/apis/esper/esper-application-api/) — APIs for application management
- [Esper Application V1 API](https://apis.io/apis/esper/esper-application-v1-api/) — APIs for application management
- [Esper Commands API](https://apis.io/apis/esper/esper-commands-api/) — APIs to run device commands. `This version of commands is being deprecated and documentation will be archived soon. Please use Commands V2.`
- [Esper Commands V2 API](https://apis.io/apis/esper/esper-commands-v2-api/) — Commands V2.0 is to provide advanced device commands capabilities like queuing, support for offline devices, dynamic device set for commands and command…
- [Esper Content API](https://apis.io/apis/esper/esper-content-api/) — APIs for Content management
- [Esper Device API](https://apis.io/apis/esper/esper-device-api/) — APIs for device management
- [Esper Device Group API](https://apis.io/apis/esper/esper-device-group-api/) — APIs for device group management
- [Esper Enterprise API](https://apis.io/apis/esper/esper-enterprise-api/) — The Esper Enterprise APIs to manage the account information set up for your company’s account. Read our Esper Manage documentation or use the Esper Manage…
- [Esper Enterprise Policy API](https://apis.io/apis/esper/esper-enterprise-policy-api/) — APIs to Esper Compliance Policy
- [Esper Geofence API](https://apis.io/apis/esper/esper-geofence-api/) — APIs for geofence management
- [Esper Group Commands API](https://apis.io/apis/esper/esper-group-commands-api/) — APIs to run group commands. Command will be run on all the active devices in a group
- [Esper Subscription API](https://apis.io/apis/esper/esper-subscription-api/) — APIs for Subscription management
- [Esper Token API](https://apis.io/apis/esper/esper-token-api/) — Fetch API token information

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Esper Events Webhooks](https://apis.io/asyncapis/esper/esper-events-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [esper-manage](https://apis.io/servers/esper/esper-manage/)

#### Collections (13)

Postman and Open Collection request collections.

- [ESPER API REFERENCE Application API](https://apis.io/collections/esper/open-esper-application-api/)
- [ESPER API REFERENCE Application Application V1 API](https://apis.io/collections/esper/open-esper-application-v1-api/)
- [ESPER API REFERENCE Application Commands API](https://apis.io/collections/esper/open-esper-commands-api/)
- [ESPER API REFERENCE Application Commands V2 API](https://apis.io/collections/esper/open-esper-commands-v2-api/)
- [ESPER API REFERENCE Application Content API](https://apis.io/collections/esper/open-esper-content-api/)
- [ESPER API REFERENCE Application Device API](https://apis.io/collections/esper/open-esper-device-api/)
- [ESPER API REFERENCE Application Device Group API](https://apis.io/collections/esper/open-esper-device-group-api/)
- [ESPER API REFERENCE Application Enterprise API](https://apis.io/collections/esper/open-esper-enterprise-api/)
- [ESPER API REFERENCE Application Enterprise Policy API](https://apis.io/collections/esper/open-esper-enterprise-policy-api/)
- [ESPER API REFERENCE Application Geofence API](https://apis.io/collections/esper/open-esper-geofence-api/)
- [ESPER API REFERENCE Application Group Commands API](https://apis.io/collections/esper/open-esper-group-commands-api/)
- [ESPER API REFERENCE Application Subscription API](https://apis.io/collections/esper/open-esper-subscription-api/)
- [ESPER API REFERENCE Application Token API](https://apis.io/collections/esper/open-esper-token-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Esper Manage Overlay](https://apis.io/overlays/esper/esper-manage-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Esper Authentication](https://apis.io/security/esper/esper-authentication/)
- [Esper Domain Security](https://apis.io/security/esper/esper-domain-security/)
- [Esper Trust Center](https://apis.io/security/esper/esper-trust-center/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://esper.io)
- [Documentation](https://help.esper.io/hc/en-us/categories/11385054747153-Developer-Documentation)
- [Getting started](https://help.esper.io/hc/en-us/articles/14199291792145-Getting-Started-with-APIs)
- [API reference](https://api.esper.io/openapi)
- [Pricing](https://www.esper.io/pricing)
- [Sign up](https://esper.io/signup)
- [Support](https://help.esper.io/)
- [Blog](https://www.esper.io/blog)
- [Compliance](https://trust.esper.io/)
- [Terms of service](https://esper.io/terms-of-service)
- [Privacy policy](https://www.esper.io/privacy-policy)
- [GitHub](https://github.com/esper-io)

## API Evangelist rating

**Kin Score 49.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 58.1 |
| Contract governance | 4.5 |
| Operational transparency | 10.5 |
| Developer ergonomics | 63.7 |
| Access clarity | 60.5 |

**Agent readiness 28.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | mostly |

**Regulatory alignment 29.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/esper/](https://apis.io/providers/esper/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Esper: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/esper/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
