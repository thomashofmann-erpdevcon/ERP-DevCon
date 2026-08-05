---
document: CG-002
title: Documentation Principles
status: Working Draft
version: 0.1.0
owner: ERP DevCon
language: en
category: Company Guide
reviewer:
approved:
created: 2026-08-05
updated: 2026-08-05
---

# Documentation Principles

## Purpose

This document defines the principles governing the creation, maintenance and lifecycle of engineering documentation within ERP DevCon.

The objective is to ensure that documentation remains accurate, maintainable, traceable and valuable throughout the complete lifecycle of a product.

---

# Scope

These principles apply to

- Company Guides
- Standards
- Architecture Decision Records
- Functional Requirements
- Solution Designs
- Technical Designs
- User Documentation
- Test Documentation
- Product Documentation

Unless explicitly stated otherwise.

---

# CG-002.1 Documentation is Part of the Product

Documentation is considered an integral part of every engineering activity.

A feature is not regarded as complete until the required documentation has been updated.

---

# CG-002.2 Documentation before Implementation

Business concepts shall be documented before implementation begins.

Implementation shall never become the primary source of business knowledge.

Software implements documented requirements.

Documentation defines them.

---

# CG-002.3 Business before Technical Documentation

Business documentation shall be created independently from technical implementation.

Business documents shall describe

- business terminology,
- business rules,
- business processes,
- business transactions,
- business decisions.

Technical implementation belongs to technical documentation.

---

# CG-002.4 Single Source of Truth

Every concept shall have exactly one authoritative definition.

Examples include

- glossary entries,
- business rules,
- architectural principles,
- document templates.

Other documents shall reference the original definition instead of duplicating it.

---

# CG-002.5 Separation of Documentation

Different document types serve different purposes.

Each document shall have one clearly defined responsibility.

Typical examples include

| Document | Purpose |
|----------|---------|
| Company Guide | Company-wide engineering principles |
| ADR | Architecture decisions |
| Functional Requirement | Business requirements |
| Solution Design | Product-specific solution |
| Technical Design | Technical implementation |
| Decision Log | Product decisions |
| Change Request | Deferred functionality |

Information shall not be duplicated across document types.

---

# CG-002.6 Incremental Development

Documentation shall evolve continuously.

Large undocumented changes shall be avoided.

Small, reviewable improvements are preferred.

---

# CG-002.7 Traceability

Engineering documentation shall remain traceable.

Whenever practical, the following relationships shall be identifiable.

Business Requirement

↓

Functional Requirement

↓

Solution Design

↓

Technical Design

↓

Implementation

↓

Test

↓

Release

Every engineering decision should be traceable through this chain.

---

# CG-002.8 Living Documentation

Documentation is considered a living engineering asset.

It shall be reviewed and updated whenever

- business processes change,
- engineering principles evolve,
- architecture decisions are revised,
- implementation affects documented behaviour.

Outdated documentation shall either be updated or archived.

---

# CG-002.9 Version Control

All engineering documentation shall be maintained under version control.

Markdown is the authoritative source format.

Generated publication formats shall not replace the repository sources.

---

# CG-002.10 Review

Engineering documentation shall undergo review before approval.

Reviews shall verify

- correctness,
- consistency,
- terminology,
- completeness,
- readability,
- maintainability.

Review comments shall improve documentation quality.

---

# CG-002.11 Consistent Terminology

Business terminology shall remain consistent throughout all documents.

Terms defined in the glossary shall be used without modification unless an approved exception exists.

New terminology should be added to the glossary before being introduced into product documentation.

---

# CG-002.12 Audience

Every document shall have a clearly identifiable target audience.

Possible audiences include

- Product Owners
- Business Analysts
- Architects
- Developers
- Test Engineers
- Technical Writers
- Project Managers
- Customers

The level of technical detail shall reflect the intended audience.

---

# CG-002.13 Document Lifecycle

Engineering documents progress through defined lifecycle stages.

Typical states include

- Draft
- Working Draft
- Review
- Approved
- Deprecated
- Archived

The current status shall always be visible within the document metadata.

---

# CG-002.14 Continuous Improvement

Documentation standards shall themselves be reviewed periodically.

Improvements shall preserve

- consistency,
- traceability,
- maintainability,
- long-term usability.

The objective is continuous improvement rather than unnecessary change.

---

# Related Documents

- Company Guide – Introduction
- Company Philosophy
- ADR-0000 – Establish Engineering Documentation Repository
- CONTRIBUTING.md

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |