# Etcd (etcd)

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

**APIs.json:** [https://etcd.io](https://etcd.io)

## Scope

- **Type:** Index

## Tags

- Cloud Native
- Consensus
- Distributed Systems
- Graduated
- Key-Value Store
- Kubernetes

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### etcd gRPC API

The etcd v3 API is a gRPC-based interface providing key-value operations (put, get, delete, range), watch streams for change notifications, lease management for TTL-based keys, cluster membership management, maintenance operations including snapshots and defragmentation, and authentication and authorization controls.

- **Human URL:** [https://etcd.io/docs/v3.5/learning/api/](https://etcd.io/docs/v3.5/learning/api/)

#### Tags

- Cluster Management
- gRPC
- Key-Value
- Lease
- Watch

#### Properties

- [Documentation](https://etcd.io/docs/v3.5/learning/api/)
- [Reference](https://etcd.io/docs/v3.5/learning/api_guarantees/)
- [Authentication](https://etcd.io/docs/v3.5/op-guide/authentication/)
- [Getting Started](https://etcd.io/docs/v3.5/dev-guide/interacting_v3/)
- [Client  Libraries](https://etcd.io/docs/v3.5/integrations/)
- [Postman Collection](collections/etcd-http-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/etcd-http-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### etcd HTTP Gateway API

etcd provides an HTTP/JSON gateway that translates HTTP requests into gRPC calls, allowing clients without gRPC support to interact with etcd. The gateway supports the same operations as the gRPC API including key-value operations, watches, and cluster management through a RESTful interface.

- **Human URL:** [https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/](https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/)

#### Tags

- Gateway
- gRPC
- HTTP
- REST

#### Properties

- [Documentation](https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/)
- [Reference](https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/)
- [OpenAPI](openapi/etcd-http-gateway-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/etcd-http-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/etcd-http-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### etcd Concurrency API

The etcd concurrency API provides distributed primitives built on top of the core key-value store, including distributed mutexes (locks), leader election, and software transactional memory (STM). These primitives are used to coordinate between distributed processes and implement consensus patterns in clustered applications.

- **Human URL:** [https://etcd.io/docs/v3.5/dev-guide/api_concurrency_reference_v3/](https://etcd.io/docs/v3.5/dev-guide/api_concurrency_reference_v3/)

#### Tags

- Concurrency
- Coordination
- Distributed Locking
- Leader Election

#### Properties

- [Documentation](https://etcd.io/docs/v3.5/dev-guide/api_concurrency_reference_v3/)
- [Reference](https://etcd.io/docs/v3.5/dev-guide/api_concurrency_reference_v3/)
- [Postman Collection](collections/etcd-http-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/etcd-http-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### etcd Metrics API

etcd exposes a Prometheus-compatible metrics endpoint that provides operational insights into the etcd cluster, including request rates, latency histograms, disk I/O statistics, Raft state, and cluster health indicators. This endpoint is used for monitoring and alerting in production etcd deployments.

- **Human URL:** [https://etcd.io/docs/v3.5/op-guide/monitoring/](https://etcd.io/docs/v3.5/op-guide/monitoring/)

#### Tags

- Metrics
- Monitoring
- Observability
- Prometheus

#### Properties

- [Documentation](https://etcd.io/docs/v3.5/op-guide/monitoring/)
- [Reference](https://etcd.io/docs/v3.5/metrics/)
- [Postman Collection](collections/etcd-http-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/etcd-http-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### etcd v2 HTTP API

The original etcd v2 API exposed a RESTful HTTP interface for key-value operations using a hierarchical directory structure. This API has been deprecated in favor of the v3 gRPC API and was removed from the default etcd build in later versions. Existing users should migrate to the v3 API.

- **Human URL:** [https://etcd.io/docs/v2.3/api/](https://etcd.io/docs/v2.3/api/)

#### Tags

- Deprecated
- HTTP
- Key-Value
- REST

#### Properties

- [Documentation](https://etcd.io/docs/v2.3/api/)
- [Deprecation  Notice](https://etcd.io/docs/v3.5/op-guide/v2-migration/)
- [Migration  Guide](https://etcd.io/docs/v3.5/op-guide/v2-migration/)
- [Postman Collection](collections/etcd-http-gateway.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/etcd-http-gateway.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [JSON Schema](json-schema/etcd-key-value-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/etcd-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Website](https://etcd.io)
- [Documentation](https://etcd.io/docs/)
- [Getting Started](https://etcd.io/docs/v3.5/quickstart/)
- [GitHub Organization](https://github.com/etcd-io)
- [GitHub Repository](https://github.com/etcd-io/etcd)
- [Blog](https://etcd.io/blog/)
- [Community](https://etcd.io/community/)
- [Changelog](https://github.com/etcd-io/etcd/blob/main/CHANGELOG/)
- [Security](https://github.com/etcd-io/etcd/blob/main/security/SECURITY.md)
- [Support](https://etcd.io/community/)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/etcd)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
