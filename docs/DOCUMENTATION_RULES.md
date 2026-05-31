# TapMind Documentation Rules

This document defines the standards for writing and maintaining the TapMind GitBook knowledge base.

---

## Audience

Documentation must be useful for:

- **Developers** — Implementation details, integration guides, and system behavior
- **Project Managers** — Timelines, dependencies, and cross-team coordination context
- **Product Managers** — Feature purpose, user impact, and business outcomes
- **Clients** — Plain-language explanations of what TapMind does and why it matters

Write so that any audience can understand the *what* and *why*; add technical depth where developers need it.

---

## Documentation Principles

### Language and clarity

- Use simple language.
- Explain technical concepts in plain English.
- Explain Redis, RabbitMQ, MongoDB, and other technical components using real-world analogies.
- Focus on business logic before implementation details.

### Required coverage for every feature

Every feature or component must explain:

- **What it is**
- **Why it exists**
- **How it works**
- **Business benefit**

### Diagrams

- Use Mermaid diagrams whenever a process or flow is described.
- Keep diagrams focused on one flow or concept per diagram.

### Modularity

- Keep documentation modular so individual sections can be updated independently.
- Avoid duplicating content across pages; link to related pages instead.
- One topic per page where possible.

---

## Standard Page Structure

Every documentation page must include these sections in order:

1. **Overview** — What this topic covers at a glance
2. **Why It Exists** — Problem it solves and rationale
3. **How It Works** — Process, flow, or architecture (include Mermaid where applicable)
4. **Business Benefit** — Value to users, clients, or the business
5. **Failure Scenarios** — What can go wrong and how it is handled or detected
6. **Related Components** — Links or references to other pages and systems

---

## Technical Analogies (Reference)

When introducing infrastructure components, use analogies such as:

| Component | Analogy guidance |
|-----------|------------------|
| **Redis** | Fast in-memory cache or short-term memory — quick lookups, temporary storage |
| **RabbitMQ** | Post office or message queue — delivers tasks between services reliably |
| **MongoDB** | Flexible filing cabinet — stores varied document shapes without rigid schemas |

Adapt analogies to the specific use case in TapMind; do not copy generic definitions without context.

---

## File Naming and Ordering

- Use numbered prefixes for sequential reading: `01-`, `02-`, etc.
- Use kebab-case for multi-word filenames: `02-System-Architecture.md`
- Keep [README.md](../README.md) as the repository entry point and index.

---

## What Not to Do

- Do not publish secrets, credentials, or environment-specific values.
- Do not write implementation-only docs without business context.
- Do not leave sections empty when publishing — placeholders are for draft structure only; replace before release.
