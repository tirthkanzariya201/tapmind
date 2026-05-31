# TapMind Documentation

Product knowledge base for the [TapMind](https://github.com/tirthkanzariya201/tapmind) platform — written for product managers, project managers, client stakeholders, support teams, and developers.

This documentation explains **what** TapMind does, **why** it exists, **what business problems** it solves, and **how** it works — with technical details only after business understanding is established.

---

## Primary Audience

1. Product Managers
2. Project Managers
3. Client Stakeholders
4. Support Teams
5. Developers

---

## GitBook Navigation

Full navigation is defined in [SUMMARY.md](./SUMMARY.md). Import this repository into GitBook and point the table of contents to `SUMMARY.md`.

### Overview

| Page | Purpose |
|------|---------|
| [Overview](./docs/overview/README.md) | Section landing page |
| [What is TapMind](./docs/overview/what-is-tapmind.md) | Introduce the platform |
| [Business Problems We Solve](./docs/overview/business-problems-we-solve.md) | Explain why TapMind exists |
| [Custom Adapter vs OrchSDK](./docs/overview/custom-adapter-vs-orchsdk.md) | Explain the difference in simple terms |

### Architecture

| Page | Purpose |
|------|---------|
| [Architecture](./docs/architecture/README.md) | Section landing page |
| [High Level Architecture](./docs/architecture/high-level-architecture.md) | Introduce all major components |
| [Core Components](./docs/architecture/core-components.md) | Publisher App, Mediation, Custom Adapter, SDK, Backend, Demand Partners |
| [Terminology & Glossary](./docs/architecture/terminology-glossary.md) | Simple language definitions |

### Ad Serving

| Page | Purpose |
|------|---------|
| [Ad Serving](./docs/ad-serving/README.md) | Section landing page |
| [End-to-End Ad Journey](./docs/ad-serving/end-to-end-ad-journey.md) | Single high-level flow from ad request to ad display |
| [SDK Flow](./docs/ad-serving/sdk-flow.md) | How the SDK participates |
| [Backend Serving Flow](./docs/ad-serving/backend-serving-flow.md) | How the backend returns configuration |
| [Demand Partner Selection](./docs/ad-serving/demand-partner-selection.md) | How priorities and waterfalls work |

### Reporting & Analytics

| Page | Purpose |
|------|---------|
| [Reporting & Analytics](./docs/reporting-analytics/README.md) | Section landing page |
| [Event Lifecycle](./docs/reporting-analytics/event-lifecycle.md) | Explain event generation |
| [Reporting Architecture](./docs/reporting-analytics/reporting-architecture.md) | Explain the reporting pipeline |
| [Why RabbitMQ](./docs/reporting-analytics/why-rabbitmq.md) | Business explanation first |
| [Why MongoDB](./docs/reporting-analytics/why-mongodb.md) | Business explanation first |
| [Why PostgreSQL](./docs/reporting-analytics/why-postgresql.md) | Business explanation first |

### Configuration Management

| Page | Purpose |
|------|---------|
| [Configuration Management](./docs/configuration-management/README.md) | Section landing page |
| [Dashboard Hierarchy](./docs/configuration-management/dashboard-hierarchy.md) | Supply Partner → Publisher → App → Version → Placement → Demand Partner |
| [Placement Configuration](./docs/configuration-management/placement-configuration.md) | Explain placement setup |
| [Demand Partner Configuration](./docs/configuration-management/demand-partner-configuration.md) | Ad Unit IDs, Priority, Sizes, TTL |

### Operations

| Page | Purpose |
|------|---------|
| [Operations](./docs/operations/README.md) | Section landing page |
| [G-Sheet Automation](./docs/operations/g-sheet-automation.md) | Explain operations workflow |
| [Monitoring & Troubleshooting](./docs/operations/monitoring-troubleshooting.md) | Support team reference |

### Reference

| Page | Purpose |
|------|---------|
| [Reference](./docs/reference/README.md) | Section landing page |
| [FAQ](./docs/reference/faq.md) | Questions from clients, PMs, and support teams |
| [API Examples](./docs/reference/api-examples.md) | Reference API examples |
| [Error Codes](./docs/reference/error-codes.md) | Error code reference |

---

## Getting Started

1. Read [Documentation Rules](./docs/DOCUMENTATION_RULES.md) before contributing.
2. Start with [What is TapMind](./docs/overview/what-is-tapmind.md) for a platform overview.
3. Follow [SUMMARY.md](./SUMMARY.md) for the full guided navigation.

---

## Contributing

Every page uses the same structure:

- Overview
- Why It Exists
- Business Problem
- High Level Explanation
- Technical Details
- Business Benefit
- Related Pages

Copy [PAGE_TEMPLATE.md](./docs/PAGE_TEMPLATE.md) when adding new pages. See [Documentation Rules](./docs/DOCUMENTATION_RULES.md) for full guidelines.

---

## Repository Structure

```
Tapmind/
├── README.md                 # Repository entry point
├── SUMMARY.md                # GitBook grouped navigation
├── .gitignore
└── docs/
    ├── DOCUMENTATION_RULES.md   # Maintainer-only (not in GitBook nav)
    ├── PAGE_TEMPLATE.md
    ├── overview/                # README.md + pages
    ├── architecture/
    ├── ad-serving/
    ├── reporting-analytics/
    ├── configuration-management/
    ├── operations/
    ├── reference/
    └── appendix/                # Maintainer resources (e.g. Mermaid patterns)
```
