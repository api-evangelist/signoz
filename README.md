# SigNoz

SigNoz is an open source observability platform with logs, traces, and metrics in a single pane, built natively on OpenTelemetry. It is a full-stack open-source APM and observability tool that serves as an open-source alternative to DataDog, NewRelic, and other proprietary monitoring solutions. SigNoz provides distributed tracing, log management, infrastructure monitoring, and alerting capabilities unified under a single interface.

**Website:** https://signoz.io  
**Documentation:** https://signoz.io/docs/  
**API Reference:** https://signoz.io/api-reference/  
**GitHub:** https://github.com/SigNoz/signoz  
**Pricing:** https://signoz.io/pricing/  

## APIs

### SigNoz API

The SigNoz REST API provides programmatic access to the observability platform. It enables management of alerts, dashboards, notification channels, cloud integrations, users, organizations, service accounts, and ingestion keys. Query endpoints are available for traces, logs, metrics, and infrastructure monitoring data.

**Authentication:** API key via `SigNoz-Api-Key` header  
**Base URL:** `https://{host}:{port}`

**Key Endpoints:**
- `POST /api/v5/query_range` — Query metrics, traces, or logs over a time range
- `GET/POST /api/v2/rules` — Manage alert rules
- `GET/POST /api/v1/channels` — Manage notification channels
- `GET/POST /api/v2/gateway/ingestion_keys` — Manage ingestion keys
- `GET /api/v2/metrics` — Browse the metrics catalog
- `GET /api/v2/infra_monitoring/hosts` — List monitored infrastructure hosts
- `GET /api/v3/traces/{traceID}/waterfall` — Get trace waterfall view

## Artifacts

### OpenAPI

| Spec | Description |
|---|---|
| [signoz-openapi.yml](openapi/signoz-openapi.yml) | SigNoz REST API — alerts, dashboards, ingestion keys, query, users, cloud integrations |

### Rules

| Ruleset | Description |
|---|---|
| [signoz-rules.yml](rules/signoz-rules.yml) | Spectral ruleset enforcing SigNoz API conventions |

### Capabilities

| Capability | Description |
|---|---|
| [observability-monitoring.yaml](capabilities/observability-monitoring.yaml) | Unified observability monitoring workflow — alerts, metrics, traces, logs, infrastructure |

**Shared Definitions:**

| Shared File | Description |
|---|---|
| [shared/signoz.yaml](capabilities/shared/signoz.yaml) | SigNoz API consumed definition |

### JSON Schema

| Schema | Description |
|---|---|
| [signoz-alert-schema.json](json-schema/signoz-alert-schema.json) | Alert rule schema |
| [signoz-dashboard-schema.json](json-schema/signoz-dashboard-schema.json) | Dashboard schema |
| [signoz-ingestion-key-schema.json](json-schema/signoz-ingestion-key-schema.json) | Ingestion key schema |

### JSON Structure

| Structure | Description |
|---|---|
| [signoz-alert-structure.json](json-structure/signoz-alert-structure.json) | Alert rule field documentation |
| [signoz-dashboard-structure.json](json-structure/signoz-dashboard-structure.json) | Dashboard field documentation |

### JSON-LD

| Context | Description |
|---|---|
| [signoz-context.jsonld](json-ld/signoz-context.jsonld) | SigNoz observability vocabulary linked data context |

### Examples

| Example | Description |
|---|---|
| [signoz-create-alert-example.json](examples/signoz-create-alert-example.json) | Create a metric-based alert rule |
| [signoz-query-traces-example.json](examples/signoz-query-traces-example.json) | Query trace data over a time range |
| [signoz-list-ingestion-keys-example.json](examples/signoz-list-ingestion-keys-example.json) | List organization ingestion keys |

### Vocabulary

| Vocabulary | Description |
|---|---|
| [signoz-vocabulary.yml](vocabulary/signoz-vocabulary.yml) | SigNoz domain vocabulary covering observability, alerting, data collection, visualization, and access control |

## Common Properties

| Property | URL |
|---|---|
| Website | https://signoz.io |
| Documentation | https://signoz.io/docs/ |
| API Reference | https://signoz.io/api-reference/ |
| GitHub Organization | https://github.com/SigNoz |
| Blog | https://signoz.io/blog/ |
| Pricing | https://signoz.io/pricing/ |
| Support | https://signoz.io/support/ |
| Community | https://signoz.io/slack/ |
| Enterprise | https://signoz.io/enterprise/ |
| Changelog | https://signoz.io/changelog/ |
| Status | https://status.signoz.io/ |

## Tags

APM, Alerting, Cloud Monitoring, Dashboards, Distributed Tracing, Infrastructure Monitoring, Logs, Metrics, Observability, OpenTelemetry, Open Source

## Maintainers

- Kin Lane (kin@apievangelist.com)
