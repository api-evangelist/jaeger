# Jaeger (jaeger)

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
