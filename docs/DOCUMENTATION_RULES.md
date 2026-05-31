# TapMind Documentation Rules

This document defines the standards for writing and maintaining the TapMind product knowledge base.

---

## Primary Audience

Documentation must serve, in order of emphasis:

1. **Product Managers** — Feature purpose, user impact, and business outcomes
2. **Project Managers** — Timelines, dependencies, and cross-team coordination
3. **Client Stakeholders** — Plain-language explanations of what TapMind delivers
4. **Support Teams** — Troubleshooting, operations, and client-facing answers
5. **Developers** — Integration guides and implementation details (after business context)

Write so any reader understands *what* TapMind does and *why* it matters before encountering technical depth.

---

## Documentation Philosophy

This knowledge base must explain:

1. **What** the system does
2. **Why** it exists
3. **What business problem** it solves
4. **How** it works at a high level
5. **Technical implementation** — only after business understanding is established

Business understanding is always more important than implementation details.

Documentation should read like **Stripe**, **AWS**, or **Twilio** product documentation — not internal engineering notes.

---

## Terminology Rules

Whenever a technical concept is introduced, explain in this order:

1. **What it is** — Plain English first
2. **Why we use it** — Purpose in the TapMind context
3. **Business benefit** — Value to clients and stakeholders
4. **Technical implementation** — How it works under the hood

Apply this pattern to Redis, RabbitMQ, MongoDB, PostgreSQL, and all infrastructure components.

---

## Standard Page Structure

Every documentation page must include these sections in order:

1. **Overview** — What this page covers at a glance
2. **Why It Exists** — Rationale and context
3. **Business Problem** — The problem this topic addresses
4. **High Level Explanation** — Plain-language process or concept (use Mermaid for flows)
5. **Technical Details** — Implementation specifics (after business context)
6. **Business Benefit** — Value delivered to clients and the business
7. **Related Pages** — Links to related documentation

Use [PAGE_TEMPLATE.md](./PAGE_TEMPLATE.md) when creating new pages.

---

## Diagrams

- Use Mermaid diagrams whenever a process or flow is described
- Keep diagrams focused on one flow or concept per diagram
- Reference [Mermaid Diagrams](./appendix/mermaid-diagrams.md) for shared diagram patterns

---

## Modularity

- One topic per page where possible
- Link to related pages instead of duplicating content
- Keep sections independently updatable

---

## File Naming and Structure

- Use kebab-case for filenames: `high-level-architecture.md`
- Group pages by GitBook section under `docs/`
- Navigation is defined in [SUMMARY.md](../SUMMARY.md) at the repository root
- [README.md](../README.md) is the repository entry point

---

## What Not to Do

- Do not publish secrets, credentials, or environment-specific values
- Do not lead with implementation details or internal jargon
- Do not write documentation like internal engineering notes
- Do not leave sections empty when publishing — placeholders are for structure only; replace before release
