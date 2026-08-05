---
document: CG-007
title: Requirements Engineering
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

# Requirements Engineering

## Purpose

This document defines the requirements engineering principles applied throughout ERP DevCon.

The objective is to ensure that business requirements remain complete, understandable, verifiable and independent from implementation technologies.

Requirements Engineering transforms business analysis into structured engineering specifications.

---

# Scope

These principles apply to

- product development,
- product enhancements,
- reusable software components,
- customer-specific extensions,
- internal software projects.

---

# CG-007.1 Business Requirements are Technology Independent

Business requirements shall describe required business behaviour.

They shall not prescribe

- implementation technologies,
- programming languages,
- database structures,
- software architecture,
- user interface implementation.

---

# CG-007.2 One Requirement – One Responsibility

Each requirement shall describe exactly one business responsibility.

Large requirements shall be decomposed into smaller, independently understandable requirements.

---

# CG-007.3 Requirements shall be Testable

Every requirement shall be formulated in a way that allows objective verification.

A requirement shall define observable business behaviour.

Subjective statements such as

- user-friendly
- intuitive
- efficient

shall be avoided unless measurable acceptance criteria exist.

---

# CG-007.4 Requirements shall be Complete

A requirement shall define

- the triggering event,
- the required behaviour,
- relevant business rules,
- exceptional situations,
- resulting business state.

If additional assumptions exist they shall be documented explicitly.

---

# CG-007.5 Requirements shall be Unambiguous

Every requirement shall have exactly one intended interpretation.

Ambiguous wording shall be avoided.

Where necessary, business terminology shall be defined by reference to the company glossary.

---

# CG-007.6 Separate Requirements from Design

Requirements describe

"What"

Solution Design describes

"How"

Technical Design describes

"How exactly"

These responsibilities shall remain strictly separated.

---

# CG-007.7 Functional Requirements

Functional Requirements define required business behaviour.

They describe

- business processes,
- business transactions,
- business rules,
- information requirements,
- user interactions,
- required results.

They intentionally avoid implementation details.

---

# CG-007.8 Non-Functional Requirements

Non-functional requirements describe qualities such as

- performance,
- scalability,
- security,
- availability,
- maintainability,
- auditability,
- legal compliance.

Non-functional requirements shall be measurable whenever practical.

---

# CG-007.9 Requirement Traceability

Every requirement should remain traceable.

Typical traceability includes

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

# CG-007.10 Requirement Lifecycle

Requirements evolve during product development.

Possible lifecycle states include

- Draft
- Proposed
- Approved
- Implemented
- Verified
- Deprecated
- Archived

The lifecycle shall remain visible throughout the documentation.

---

# CG-007.11 Deferred Functionality

Business functionality intentionally excluded from the current scope shall not be removed from engineering documentation.

Deferred functionality shall be documented within the corresponding Change Request Backlog.

This principle preserves engineering knowledge while maintaining a manageable implementation scope.

---

# CG-007.12 Product Scope

Every requirement shall belong to exactly one product scope.

Company-wide standards shall not be documented as product requirements.

Likewise, product-specific requirements shall not be incorporated into company standards.

---

# CG-007.13 Continuous Refinement

Requirements Engineering is an iterative engineering discipline.

Improved business understanding shall result in improved requirements.

Refinement shall increase precision without changing the original business intent unless explicitly approved.

---

# Related Documents

- Business Analysis
- Documentation Principles
- Architecture Principles
- Functional Requirement Template
- Change Request Template

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |