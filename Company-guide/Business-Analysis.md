---
document: CG-006
title: Business Analysis
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

# Business Analysis

## Purpose

This document defines the principles governing business analysis activities within ERP DevCon.

Business Analysis provides the foundation for all engineering activities by transforming business needs into precise, complete and implementation-independent requirements.

No implementation activity shall begin before the relevant business problem has been sufficiently understood.

---

# Scope

These principles apply to

- new products,
- product enhancements,
- customer-specific developments,
- reusable software components,
- architectural initiatives.

---

# CG-006.1 Understand the Business Domain

Business Analysis shall begin with understanding the business domain.

The objective is to understand

- business objectives,
- business terminology,
- business processes,
- business events,
- business rules,
- legal requirements,
- organizational responsibilities.

Technology shall not influence this analysis.

---

# CG-006.2 Business before Solution

Business Analysis defines the problem.

Solution Design defines the solution.

Technical Design defines the implementation.

These responsibilities shall remain clearly separated.

---

# CG-006.3 Define Business Terminology

Business terminology shall be defined before business rules.

Every important business term shall have

- a clear definition,
- one meaning,
- one authoritative source.

Business terminology shall be maintained within the company glossary.

---

# CG-006.4 Define Business Objects

Business Analysis shall identify all relevant business objects.

Each business object shall have

- a business purpose,
- a clearly defined lifecycle,
- documented relationships,
- documented responsibilities.

Business objects shall not be introduced because they simplify implementation.

---

# CG-006.5 Identify Business Transactions

Business transactions describe events that change business reality.

Typical examples include

- creation,
- approval,
- posting,
- cancellation,
- correction,
- expiration,
- settlement.

Business transactions form the basis for business history.

---

# CG-006.6 Separate Facts from Decisions

Business Analysis distinguishes between

- business facts,
- business calculations,
- business proposals,
- business decisions.

Software may calculate or propose.

Business users decide unless explicit automation has been defined.

---

# CG-006.7 Information before Automation

The first implementation objective is to provide complete business information.

Automation shall only be introduced after the required business information has been identified.

Every automated activity should remain manually executable whenever reasonably possible.

---

# CG-006.8 Product Independence

Business Analysis shall remain independent of

- programming languages,
- databases,
- ERP systems,
- cloud platforms,
- user interface technologies.

Implementation-specific considerations belong to later engineering phases.

---

# CG-006.9 Traceability

Every business requirement should remain traceable throughout the engineering lifecycle.

Typical traceability chain

Business Need

↓

Business Analysis

↓

Functional Requirement

↓

Solution Design

↓

Technical Design

↓

Implementation

↓

Testing

↓

Release

---

# CG-006.10 Completeness

Business Analysis shall describe

- normal business processes,
- exceptional situations,
- error situations,
- boundary conditions,
- historical behaviour,
- business constraints.

Incomplete analysis inevitably results in incomplete software.

---

# CG-006.11 Change Management

Business Analysis is an iterative process.

New knowledge may require

- clarification,
- refinement,
- restructuring,
- reprioritization.

Changes shall remain traceable throughout the documentation.

---

# CG-006.12 Engineering Responsibility

Business Analysis is an engineering discipline.

Its objective is not merely to collect requirements but to understand and document the business domain with sufficient precision that different implementation teams would arrive at equivalent business behaviour.

---

# Related Documents

- Company Philosophy
- Documentation Principles
- Architecture Principles
- Software Engineering
- Functional Requirement Template
- Architecture Decision Records

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |