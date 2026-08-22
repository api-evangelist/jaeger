# Jaeger (jaeger)

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

Jaeger is an open source, end-to-end distributed tracing system for monitoring and troubleshooting microservices-based architectures. Jaeger provides visibility into distributed system behavior through trace collection, storage, and visualization.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Distributed Tracing
- Microservices
- Monitoring
- Observability

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-05-19

## APIs

### Jaeger Query API

The Jaeger Query API is an HTTP/JSON API exposed by the Jaeger Query service for retrieving distributed traces, listing services and operations, querying service dependency graphs, and accessing performance metrics including latency, call rates, and error rates. A gRPC version of the Query API is also available defined in the jaeger-idl query.proto IDL.

- **Human URL:** [https://www.jaegertracing.io/docs/latest/apis/](https://www.jaegertracing.io/docs/latest/apis/)

#### Tags

- Distributed Tracing
- Observability
- Query
- Traces

#### Properties

- [Documentation](https://www.jaegertracing.io/docs/latest/apis/)
- [OpenAPI](openapi/jaeger-query-api.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/jaeger-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jaeger-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub Repository](https://github.com/jaegertracing/jaeger)
- [Changelog](https://github.com/jaegertracing/jaeger/blob/main/CHANGELOG.md)

### Jaeger Collector API

The Jaeger Collector API receives trace spans from instrumented applications and SDKs. Since Jaeger v1.11 the primary protocol is the jaeger.api_v2.CollectorService gRPC endpoint; the collector also accepts OTLP traces (binary gRPC, Protobuf over HTTP, JSON over HTTP) since v1.35, as well as legacy Thrift over UDP and HTTP formats.

- **Human URL:** [https://www.jaegertracing.io/docs/latest/apis/](https://www.jaegertracing.io/docs/latest/apis/)

#### Tags

- Collector
- Distributed Tracing
- gRPC
- OTLP

#### Properties

- [Documentation](https://www.jaegertracing.io/docs/latest/apis/)
- [Reference](https://github.com/jaegertracing/jaeger-idl/blob/main/proto/api_v2/collector.proto)
- [GitHub Repository](https://github.com/jaegertracing/jaeger)
- [Postman Collection](collections/jaeger-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jaeger-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jaeger Remote Storage API

The Jaeger Remote Storage API is a gRPC-based interface that allows extending Jaeger with custom storage backends. Any backend implementing this API can be deployed as a remote gRPC server and plugged into Jaeger components in place of built-in storage engines (available since v1.30).

- **Human URL:** [https://www.jaegertracing.io/docs/latest/apis/](https://www.jaegertracing.io/docs/latest/apis/)

#### Tags

- Distributed Tracing
- Extensions
- gRPC
- Storage

#### Properties

- [Documentation](https://www.jaegertracing.io/docs/latest/apis/)
- [Reference](https://github.com/jaegertracing/jaeger-idl/blob/main/proto/api_v2/query.proto)
- [GitHub Repository](https://github.com/jaegertracing/jaeger)
- [Postman Collection](collections/jaeger-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jaeger-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Jaeger Remote Sampling API

The Jaeger Remote Sampling API provides HTTP and gRPC endpoints that SDKs use to retrieve sampling strategies for distributed trace collection. It is implemented by the jaeger-collector and defined in the sampling.proto IDL, supporting both static file-based and adaptive sampling strategies.

- **Human URL:** [https://www.jaegertracing.io/docs/latest/apis/](https://www.jaegertracing.io/docs/latest/apis/)

#### Tags

- Configuration
- Distributed Tracing
- gRPC
- Sampling

#### Properties

- [Documentation](https://www.jaegertracing.io/docs/latest/apis/)
- [Reference](https://github.com/jaegertracing/jaeger-idl/blob/main/proto/api_v2/sampling.proto)
- [GitHub Repository](https://github.com/jaegertracing/jaeger)
- [Postman Collection](collections/jaeger-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/jaeger-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.jaegertracing.io/)
- [Documentation](https://www.jaegertracing.io/docs/)
- [Getting Started](https://www.jaegertracing.io/docs/latest/getting-started/)
- [GitHub Organization](https://github.com/jaegertracing)
- [GitHub Repository](https://github.com/jaegertracing/jaeger)
- [Blog](https://www.jaegertracing.io/news/)
- [Community](https://www.jaegertracing.io/get-involved/)
- [Support](https://www.jaegertracing.io/get-in-touch/)
- [Changelog](https://github.com/jaegertracing/jaeger/blob/main/CHANGELOG.md)
- [JSON-LD](json-ld/jaeger-trace.yml) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/jaeger-trace.yml) — [JSON Schema](https://json-schema.org/specification)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
