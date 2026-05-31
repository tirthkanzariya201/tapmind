# TapMind Documentation Rules

This document defines the standards for writing and maintaining the TapMind product knowledge base. It is for maintainers and contributors using Cursor or other editing tools. This file is not published in GitBook navigation.

---

## Purpose

This documentation is not intended to be a technical reference only.

The goal is to help any reader understand:

- How mobile advertising works
- Why TapMind exists
- Where TapMind fits into the advertising ecosystem
- How TapMind solves business problems
- How the platform works technically

A reader should never need prior AdTech knowledge.

---

## Primary Audience

Documentation must serve:

1. **Product Managers**
2. **Project Managers**
3. **Client Stakeholders**
4. **Support Teams**
5. **Developers**

Write so any reader understands *what* TapMind does and *why* it matters before encountering technical depth.

---

## Golden Rule

Never explain a concept before the reader has enough context to understand why it exists.

**Bad example:**

Publisher → Demand Partner → Placement → Bid Request

**Good example:**

User opens Cricbuzz
→ User sees an ad
→ How did the ad get there?
→ Publisher
→ Placement
→ Ad Request
→ Demand Partner
→ Bid Request

Concepts should be introduced naturally as part of a story.

---

## Learning Journey

Documentation should follow this order:

1. Real-world scenario
2. Business problem
3. AdTech concepts
4. TapMind's role
5. High-level architecture
6. Detailed architecture
7. Technical implementation

Never reverse this order.

---

## Story-Driven Documentation

Whenever possible, begin with a relatable example.

Example:

"When you open Cricbuzz and see an advertisement, several systems work together in milliseconds to decide which ad appears."

Then explain the journey.

Readers should understand the problem before seeing the solution.

---

## Progressive Disclosure

Do not introduce all terminology at once.

Introduce concepts only when they become relevant.

| Concept | Introduce when... |
|---------|-------------------|
| **Publisher** | Explaining who owns the app |
| **Placement** | Explaining where ads appear |
| **Demand Partner** | Explaining who provides ads |
| **Bid Request** | Only after Demand Partners are understood |

Apply the same pattern to infrastructure (Redis, RabbitMQ, MongoDB, PostgreSQL): plain English first, business context second, technical implementation last.

---

## Business First

Every content page should answer:

1. What problem exists?
2. Why should I care?
3. How is it solved?
4. Where does TapMind fit?
5. How is it implemented?

Business understanding comes before technical details.

Documentation should read like **Stripe**, **AWS**, or **Twilio** product documentation. Not internal engineering notes.

---

## Writing Style

- Use simple language
- Avoid jargon whenever possible
- Explain technical concepts in plain English first
- Use examples and analogies
- Keep paragraphs short
- Avoid large walls of text
- Do not use em dashes
- Prefer diagrams over lengthy explanations

---

## Content Page Structure

Content pages (not section landing pages) should generally follow:

1. **Real-world example** — A relatable scenario that sets context
2. **Why this matters** — The business problem and why the reader should care
3. **Concept explanation** — Plain-language explanation of relevant AdTech concepts
4. **TapMind implementation** — How TapMind addresses the problem at a high level
5. **Technical details** — Implementation specifics (after business context)
6. **Related pages** — Links to related documentation

Use [PAGE_TEMPLATE.md](./PAGE_TEMPLATE.md) when creating new content pages.

Section landing pages (`README.md` in each folder) use a different hub format. See existing section README files for the navigation hub structure.

---

## Documentation Success Test

A non-technical Product Manager should be able to read the documentation from start to finish and understand:

- How ads appear in apps
- Who participates in the ecosystem
- Why TapMind exists
- How TapMind works

...without requiring external research.

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
- Do not dump terminology before the reader has context
- Do not write documentation like internal engineering notes
- Do not leave sections empty when publishing. Placeholders are for structure only; replace before release
