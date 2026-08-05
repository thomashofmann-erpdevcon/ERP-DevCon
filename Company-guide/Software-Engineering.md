---
document: CG-004
title: Software Engineering
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

# Software Engineering

## Purpose

This document defines the software engineering principles applied throughout ERP DevCon.

The objective is to establish a common engineering culture that produces maintainable, understandable and extensible software while ensuring that implementation remains aligned with business requirements.

This document intentionally defines engineering principles rather than implementation techniques.

---

# Scope

These principles apply to

- software development,
- software maintenance,
- product enhancements,
- bug fixes,
- reusable libraries,
- prototypes that evolve into production software.

---

# CG-004.1 Business Driven Development

Software development shall begin with understanding the business domain.

Implementation shall follow documented business requirements.

Business knowledge shall never be inferred solely from existing source code.

---

# CG-004.2 Documentation First

Business requirements shall be documented before implementation.

Where applicable, software development follows the sequence

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

Implementation shall not become the primary source of product knowledge.

---

# CG-004.3 Simplicity

Software shall be designed to be understood.

Simple solutions are preferred over complex solutions whenever they satisfy the documented requirements.

Complexity shall only be introduced where justified by business requirements.

---

# CG-004.4 Readability

Source code is primarily written for developers.

Code shall therefore

- be readable,
- be self-explanatory,
- avoid unnecessary complexity,
- use meaningful names,
- minimise hidden behaviour.

Readable software reduces maintenance costs.

---

# CG-004.5 Maintainability

Software shall be maintainable throughout its expected lifetime.

Engineering decisions shall consider

- future enhancements,
- debugging,
- testing,
- onboarding of new developers,
- long-term ownership.

Maintainability has priority over implementation speed.

---

# CG-004.6 Separation of Responsibilities

Each software component shall have one clearly defined responsibility.

Business logic shall remain independent from

- presentation,
- persistence,
- infrastructure,
- integration,
- user interface implementation.

Responsibilities shall remain clearly separated.

---

# CG-004.7 Reuse

Reusable functionality shall be implemented once.

Shared functionality shall be provided through reusable libraries whenever appropriate.

Duplication requires documented justification.

---

# CG-004.8 Explicit Behaviour

Software behaviour shall be explicit.

Hidden side effects should be avoided.

Dependencies shall be visible.

Configuration shall be documented.

Unexpected behaviour shall never become an accepted implementation technique.

---

# CG-004.9 Error Handling

Errors shall be detected as early as reasonably possible.

Error messages shall

- describe the problem,
- support troubleshooting,
- avoid technical ambiguity,
- provide meaningful information.

Errors shall never be silently ignored.

---

# CG-004.10 Testing

Software shall be designed so that its behaviour can be verified.

Testing shall confirm that documented business requirements have been implemented correctly.

Testing is regarded as an engineering activity rather than a final project phase.

---

# CG-004.11 Continuous Improvement

Engineering standards evolve continuously.

Developers are encouraged to improve

- readability,
- consistency,
- documentation,
- architecture,
- maintainability,

provided that business behaviour remains unchanged unless explicitly required.

---

# CG-004.12 Engineering Responsibility

Every developer is responsible for the quality of the delivered software.

Quality includes

- correctness,
- maintainability,
- documentation,
- readability,
- consistency,
- testability.

Quality assurance is therefore a shared engineering responsibility rather than the exclusive responsibility of a testing department.

---

# Related Documents

- Company Philosophy
- Documentation Principles
- Architecture Principles
- Coding Standards
- Architecture Decision Records

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |