---
document: CG-005
title: Coding Standards
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

# Coding Standards

## Purpose

This document defines the general coding standards that apply to software developed by ERP DevCon.

These standards are intentionally independent of programming languages and implementation platforms.

Language-specific conventions shall be documented separately where required.

---

# Scope

These standards apply to

- application development,
- reusable libraries,
- automation tools,
- scripts,
- prototypes that become production software.

---

# CG-005.1 Readability

Source code shall primarily be written for people.

Readable code has priority over compact code.

The intent of the implementation shall be immediately understandable.

---

# CG-005.2 Self-Documenting Code

Source code should explain itself.

Meaningful names shall be preferred over comments.

Comments shall explain

- why something is implemented,
- business rules,
- assumptions,
- constraints,

rather than describing obvious implementation details.

---

# CG-005.3 Naming

Identifiers shall use meaningful business terminology.

Names shall

- describe responsibility,
- remain consistent,
- avoid unnecessary abbreviations,
- use glossary terminology whenever applicable.

Temporary names such as

- temp
- data
- value
- object
- item

shall only be used when they accurately describe the represented concept.

---

# CG-005.4 Single Responsibility

Every software element shall have one clearly defined responsibility.

Classes, modules, procedures and functions shall avoid combining unrelated responsibilities.

---

# CG-005.5 Business Logic

Business logic shall remain independent from technical infrastructure whenever practical.

Business rules shall not be hidden inside

- database access,
- user interface code,
- integration code,
- configuration handling.

---

# CG-005.6 Explicit Behaviour

Software behaviour shall be explicit.

Hidden side effects shall be avoided.

Dependencies should remain visible.

Unexpected behaviour shall never become part of normal application flow.

---

# CG-005.7 Error Handling

Errors shall be handled deliberately.

Software shall

- detect errors,
- report errors,
- preserve diagnostic information,
- avoid silent failures.

Error handling shall support troubleshooting rather than merely suppressing exceptions.

---

# CG-005.8 Maintainability

Code shall be written with future maintenance in mind.

Engineering decisions shall consider

- readability,
- extensibility,
- debugging,
- testing,
- documentation.

Short-term implementation shortcuts shall be avoided if they increase long-term maintenance costs.

---

# CG-005.9 Consistency

Equivalent concepts shall be implemented consistently throughout a product.

Naming, structure and programming style should remain uniform.

Consistency is generally preferable to individual coding preferences.

---

# CG-005.10 Reuse

Reusable functionality shall be implemented once.

Code duplication should be avoided.

Shared functionality should be moved into reusable components whenever appropriate.

---

# CG-005.11 Documentation

Business-relevant implementation shall be traceable to documented requirements.

Where appropriate, source code should reference

- Functional Requirements,
- Solution Designs,
- Technical Designs,
- Architecture Decision Records.

Documentation shall explain business intent rather than implementation mechanics.

---

# CG-005.12 Refactoring

Refactoring is encouraged whenever it

- improves readability,
- reduces complexity,
- removes duplication,
- simplifies maintenance,

without changing documented business behaviour.

Large refactorings shall be performed incrementally whenever practical.

---

# CG-005.13 Code Reviews

Significant software changes shall undergo peer review.

Reviews should verify

- correctness,
- readability,
- maintainability,
- consistency,
- architectural compliance,
- business alignment.

The objective of a review is continuous improvement rather than fault finding.

---

# Related Documents

- Company Philosophy
- Architecture Principles
- Software Engineering
- Documentation Principles
- Architecture Decision Records

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |