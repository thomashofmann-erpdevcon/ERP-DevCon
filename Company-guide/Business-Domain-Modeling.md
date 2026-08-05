---
document: CG-021
title: Business Domain Modeling
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

# Business Domain Modeling

## Purpose

This document defines the principles governing Business Domain Modeling within ERP DevCon.

Business Domain Modeling establishes a structured representation of the business domain before software architecture, database design or implementation are considered.

A correct understanding of the business domain is regarded as the foundation of every successful software product.

---

# Scope

These principles apply to

- business analysis,
- product architecture,
- functional requirements,
- reusable business components,
- product evolution.

---

# BDM-001 Model the Business, not the Software

Business models shall describe the business domain.

They shall not describe

- database tables,
- software classes,
- APIs,
- user interfaces,
- implementation technologies.

Business models remain valid even if the software implementation changes.

---

# BDM-002 Identify Business Objects

Business Domain Modeling shall identify all relevant Business Objects.

Every Business Object shall have

- business purpose,
- business identity,
- business lifecycle,
- business responsibilities,
- business relationships.

Business Objects represent concepts that exist within the business domain.

---

# BDM-003 Business Objects before Data Structures

Business Objects shall be identified before designing data structures.

Database tables are implementation artefacts.

Business Objects are business concepts.

The two shall not be confused.

---

# BDM-004 Business Relationships

Relationships between Business Objects shall be explicitly documented.

Relationships include

- ownership,
- aggregation,
- composition,
- reference,
- dependency,
- business responsibility.

Relationships shall describe business meaning rather than technical implementation.

---

# BDM-005 Business Transactions

Business Transactions describe changes within the business domain.

Every Business Transaction shall identify

- initiating event,
- participating Business Objects,
- business rules,
- resulting business state.

Business Transactions create business history.

---

# BDM-006 Business State

Business Objects may pass through different business states during their lifecycle.

State transitions shall be

- explicitly defined,
- business-driven,
- reproducible,
- understandable.

Business states shall not depend upon implementation details.

---

# BDM-007 Historical Integrity

Business Domain Models shall preserve historical correctness.

Historical information should normally be represented by additional Business Transactions instead of modifying historical Business Objects.

Historical business behaviour shall remain reproducible.

---

# BDM-008 Explicit Business Rules

Business Rules shall be attached to Business Objects or Business Transactions.

Business Rules shall never remain implicit.

Engineering documentation shall explain

- why a rule exists,
- when it applies,
- how it affects the business domain.

---

# BDM-009 Stable Business Concepts

Business concepts should remain stable throughout product evolution.

Implementation technologies may change.

Business concepts should change only when the business itself changes.

---

# BDM-010 Traceability

Business Domain Models shall remain traceable to

- Business Analysis,
- Functional Requirements,
- Solution Design,
- Architecture Decision Records.

Every important Business Object should have a clearly identifiable origin.

---

# BDM-011 Reuse

Equivalent business concepts should be reused across products whenever practical.

Common business concepts shall not be redefined independently by multiple products.

Reusable business concepts should become part of the Engineering Repository.

---

# BDM-012 Continuous Evolution

Business Domain Models evolve together with business understanding.

Refinement shall improve

- precision,
- completeness,
- consistency,
- maintainability,

without unnecessarily changing established business terminology.

---

# Related Documents

- Business Analysis
- Requirements Engineering
- Architecture Principles
- Engineering Principles
- Functional Requirement
- Solution Design

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |