# Reporting & Analytics

## Section Overview

This section explains how TapMind captures events, processes data, and delivers reporting. It covers the event lifecycle, reporting architecture, and the role of key data infrastructure.

Use this section when you need to understand how performance and revenue data flows through the platform.

## Who Should Read This Section

- **Product Managers** evaluating reporting capabilities for clients
- **Project Managers** tracking reporting-related milestones
- **Client Stakeholders** who rely on revenue and performance data
- **Support Teams** investigating reporting delays or data discrepancies
- **Developers** working on event pipelines or data integrations

## Pages In This Section

| Page | What you will learn |
|------|---------------------|
| [Event Lifecycle](./event-lifecycle.md) | How events are generated, transmitted, and stored |
| [Reporting Architecture](./reporting-architecture.md) | How the reporting pipeline is structured end to end |
| [Why RabbitMQ](./why-rabbitmq.md) | Why TapMind uses a message queue for event processing |
| [Why MongoDB](./why-mongodb.md) | Why TapMind uses document storage for event data |
| [Why PostgreSQL](./why-postgresql.md) | Why TapMind uses relational storage for structured data |

## Suggested Reading Path

**New user**

[What is TapMind](../getting-started/what-is-tapmind.md) → [Event Lifecycle](./event-lifecycle.md) → [Reporting Architecture](./reporting-architecture.md)

**Developer**

[Event Lifecycle](./event-lifecycle.md) → [Reporting Architecture](./reporting-architecture.md) → [Why RabbitMQ](./why-rabbitmq.md)

**Operations**

[Reporting Architecture](./reporting-architecture.md) → [Monitoring & Troubleshooting](../operations/monitoring-troubleshooting.md) → [FAQ](../reference/faq.md)
