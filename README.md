# Byfinance

Byfinance is a planned cross-border fintech platform for digital factoring,
flexible credit, operating leases, credit-risk scoring, compliance
(SARLAFT/AML), and portfolio management across the Pacific Alliance and
applicable free-trade agreements.

## Monorepo structure

This repository currently provides the domain-oriented monorepo scaffold. The
directories and workflow files establish ownership boundaries and planned
locations; they are not implementations of the listed products, infrastructure,
or deployment processes. Configure and review each workflow for the target
environment before using it.

- `apps/`: MiPyme and enterprise portals, admin console, and documentation site.
- `services/`: API gateway and financial, identity, compliance, and integration
  services; `scoring-service/` contains the planned ML lifecycle.
- `packages/`: shared libraries and design system.
- `database/`, `data-platform/`: PostgreSQL/Redis assets, ingestion, warehouse,
  analytics, and MLOps.
- `infrastructure/`, `environments/`: cloud, Kubernetes, Helm, Argo CD, and
  environment-specific configuration.
- `observability/`, `security/`: telemetry, dashboards, policies, and controls.
- `architecture/`, `docs/`: architecture decisions, models, technical
  documentation, and operating guidance.
- `tests/`, `scripts/`, `tools/`: quality domains and supporting automation.

The GitHub Actions files are dispatchable placeholders until their
environment-specific checks and deployment steps are implemented. The CI
workflow only verifies that the principal monorepo areas are present.
