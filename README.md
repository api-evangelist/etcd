# Etcd

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

etcd is a CNCF graduated distributed, reliable key-value store used as the backing store for all Kubernetes cluster data. It provides strong consistency guarantees using the Raft consensus algorithm, supporting watch operations, lease-based TTLs, and atomic compare-and-swap transactions. etcd is designed for high availability and stores critical configuration data for distributed systems.

**Areas:** Cloud-Native · Consensus · Distributed Systems · Graduated · Key-Value Store · Kubernetes

## Etcd on APIs.io

Everything profiled for Etcd is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/etcd/](https://apis.io/providers/etcd/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [etcd gRPC API](https://apis.io/apis/etcd/etcd-grpc-api/) — The etcd v3 API is a gRPC-based interface providing key-value operations (put, get, delete, range), watch streams for change notifications, lease management…
- [etcd Concurrency API](https://apis.io/apis/etcd/etcd-concurrency-api/) — The etcd concurrency API provides distributed primitives built on top of the core key-value store, including distributed mutexes (locks), leader election,…
- [etcd Metrics API](https://apis.io/apis/etcd/etcd-metrics-api/) — etcd exposes a Prometheus-compatible metrics endpoint that provides operational insights into the etcd cluster, including request rates, latency histograms,…
- [etcd v2 HTTP API](https://apis.io/apis/etcd/etcd-v2-api/) — The original etcd v2 API exposed a RESTful HTTP interface for key-value operations using a hierarchical directory structure. This API has been deprecated in…
- [Etcd Auth API](https://apis.io/apis/etcd/etcd-auth-api/) — Authentication and authorization management for users and roles
- [Etcd Cluster API](https://apis.io/apis/etcd/etcd-cluster-api/) — Cluster membership management including member add, remove, and list
- [Etcd KV API](https://apis.io/apis/etcd/etcd-kv-api/) — Key-value store operations including put, get, delete, and range queries
- [Etcd Lease API](https://apis.io/apis/etcd/etcd-lease-api/) — Lease management for TTL-based key expiration
- [Etcd Maintenance API](https://apis.io/apis/etcd/etcd-maintenance-api/) — Maintenance operations including snapshots, defragmentation, and status
- [Etcd Watch API](https://apis.io/apis/etcd/etcd-watch-api/) — Watch operations for streaming key change notifications

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Etcd Agentic Access](https://apis.io/agentic-access/etcd/etcd-agentic-access/)

#### JSON Schema (76)

The data models the API reads and writes.

- [AlarmMember](https://apis.io/schemas/etcd/etcd-alarmmember/)
- [AlarmRequest](https://apis.io/schemas/etcd/etcd-alarmrequest/)
- [AlarmResponse](https://apis.io/schemas/etcd/etcd-alarmresponse/)
- [AuthDisableResponse](https://apis.io/schemas/etcd/etcd-authdisableresponse/)
- [AuthEnableResponse](https://apis.io/schemas/etcd/etcd-authenableresponse/)
- [AuthenticateRequest](https://apis.io/schemas/etcd/etcd-authenticaterequest/)
- [AuthenticateResponse](https://apis.io/schemas/etcd/etcd-authenticateresponse/)
- [AuthRoleAddRequest](https://apis.io/schemas/etcd/etcd-authroleaddrequest/)
- [AuthRoleAddResponse](https://apis.io/schemas/etcd/etcd-authroleaddresponse/)
- [AuthRoleDeleteRequest](https://apis.io/schemas/etcd/etcd-authroledeleterequest/)
- [AuthRoleDeleteResponse](https://apis.io/schemas/etcd/etcd-authroledeleteresponse/)
- [AuthRoleGetRequest](https://apis.io/schemas/etcd/etcd-authrolegetrequest/)
- [AuthRoleGetResponse](https://apis.io/schemas/etcd/etcd-authrolegetresponse/)
- [AuthRoleGrantPermissionRequest](https://apis.io/schemas/etcd/etcd-authrolegrantpermissionrequest/)
- [AuthRoleGrantPermissionResponse](https://apis.io/schemas/etcd/etcd-authrolegrantpermissionresponse/)
- [AuthRoleListResponse](https://apis.io/schemas/etcd/etcd-authrolelistresponse/)
- [AuthRoleRevokePermissionRequest](https://apis.io/schemas/etcd/etcd-authrolerevokepermissionrequest/)
- [AuthRoleRevokePermissionResponse](https://apis.io/schemas/etcd/etcd-authrolerevokepermissionresponse/)
- [AuthUserAddRequest](https://apis.io/schemas/etcd/etcd-authuseraddrequest/)
- [AuthUserAddResponse](https://apis.io/schemas/etcd/etcd-authuseraddresponse/)
- [AuthUserChangePasswordRequest](https://apis.io/schemas/etcd/etcd-authuserchangepasswordrequest/)
- [AuthUserChangePasswordResponse](https://apis.io/schemas/etcd/etcd-authuserchangepasswordresponse/)
- [AuthUserDeleteRequest](https://apis.io/schemas/etcd/etcd-authuserdeleterequest/)
- [AuthUserDeleteResponse](https://apis.io/schemas/etcd/etcd-authuserdeleteresponse/)
- [AuthUserGetRequest](https://apis.io/schemas/etcd/etcd-authusergetrequest/)
- …and 51 more published on APIs.io

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Etcd Structure](https://apis.io/json-structure/etcd/etcd-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Etcd Context](https://apis.io/jsonld/etcd/etcd-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Etcd Domain Vocabulary](https://apis.io/vocabularies/etcd/etcd-vocabulary/)

#### Collections (7)

Postman and Open Collection request collections.

- [etcd HTTP Gateway Auth API](https://apis.io/collections/etcd/open-etcd-auth-api/)
- [etcd HTTP Gateway Auth Cluster API](https://apis.io/collections/etcd/open-etcd-cluster-api/)
- [etcd HTTP Gateway API](https://apis.io/collections/etcd/open-etcd-http-gateway/)
- [etcd HTTP Gateway Auth KV API](https://apis.io/collections/etcd/open-etcd-kv-api/)
- [etcd HTTP Gateway Auth Lease API](https://apis.io/collections/etcd/open-etcd-lease-api/)
- [etcd HTTP Gateway Auth Maintenance API](https://apis.io/collections/etcd/open-etcd-maintenance-api/)
- [etcd HTTP Gateway Auth Watch API](https://apis.io/collections/etcd/open-etcd-watch-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Etcd — jsonschema rules](https://apis.io/rules/etcd/etcd-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Etcd Authentication](https://apis.io/security/etcd/etcd-authentication/)
- [Etcd Domain Security](https://apis.io/security/etcd/etcd-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Etcd Plans Pricing](https://apis.io/plans/etcd/etcd-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Etcd Rate Limits](https://apis.io/rate-limits/etcd/etcd-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Etcd Finops](https://apis.io/finops/etcd/etcd-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://etcd.io)
- [Documentation](https://etcd.io/docs/)
- [Getting started](https://etcd.io/docs/v3.5/quickstart/)
- [Support](https://etcd.io/community/)
- [Changelog](https://github.com/etcd-io/etcd/blob/main/CHANGELOG/)
- [Blog](https://etcd.io/blog/)
- [Security](https://github.com/etcd-io/etcd/blob/main/security/SECURITY.md)
- [GitHub](https://github.com/etcd-io)

## API Evangelist rating

**Kin Score 48.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 53.6 |
| Contract governance | 9.8 |
| Operational transparency | 47.4 |
| Developer ergonomics | 47.6 |
| Access clarity | 5.3 |

**Agent readiness 25.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/etcd/](https://apis.io/providers/etcd/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Etcd: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/etcd/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
