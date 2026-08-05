---
document: CG-001
title: Company Philosophy
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

# Company Philosophy

## Purpose

This document defines the fundamental principles that govern all engineering, product development and business analysis activities performed by ERP DevCon.

The principles defined in this document are company-wide standards and apply to every product unless an explicitly approved exception exists.

---

# Philosophy Statement

ERP DevCon develops business software.

Technology is regarded as a means to implement business requirements rather than an objective of its own.

Every engineering decision shall therefore begin with understanding the business domain before selecting technical solutions.

---

# Fundamental Principles

## CG-001.1 Business before Technology

Business requirements shall always be defined independently of implementation technology.

The business model shall never be adapted solely because of limitations of a particular platform, programming language or framework.

Technology implements business requirements.

Technology does not define business requirements.

---

## CG-001.2 Information before Automation

The primary responsibility of software is to provide complete, reliable and understandable business information.

Automation is considered an enhancement.

Whenever possible, a business process shall remain executable manually based on the information provided by the system.

This principle ensures

- transparency,
- auditability,
- maintainability,
- business continuity.

---

## CG-001.3 Business Decisions remain Human Decisions

Business software shall support business users.

It shall not replace business responsibility unless explicitly required by law or business policy.

The system shall therefore primarily provide

- information,
- calculations,
- proposals,
- validations,
- warnings,
- business impact analyses.

Final business decisions remain the responsibility of authorized users.

---

## CG-001.4 Platform Independence

Business concepts shall remain independent of implementation technologies.

Business terminology shall never reference

- Business Central,
- SQL Server,
- Azure,
- .NET,
- C#,
- PowerShell,
- Python,
- any database system,
- any cloud provider.

Platform-specific implementation details belong to technical documentation rather than business documentation.

---

## CG-001.5 Long-Term Thinking

Software shall be designed with long-term maintainability as a primary objective.

Engineering decisions shall consider

- maintainability,
- extensibility,
- readability,
- testability,
- upgradeability,
- documentation effort.

Short-term implementation convenience shall never outweigh long-term engineering quality.

---

## CG-001.6 Simplicity

Solutions should be as simple as reasonably possible.

Complexity shall only be introduced where required by the business domain.

Unnecessary abstraction shall be avoided.

---

## CG-001.7 Consistency

Engineering principles shall be applied consistently throughout all products.

Equivalent business concepts shall be represented using the same terminology and architectural principles.

Consistency has priority over local optimization.

---

## CG-001.8 Historical Correctness

Business systems manage business history.

Historical business information shall never be destroyed unless explicitly required by legal regulations.

Corrections should normally be represented by additional business transactions instead of modifying historical records.

---

## CG-001.9 Explicitness

Business rules shall be explicitly documented.

Implicit assumptions shall be avoided.

Engineering decisions shall remain understandable without requiring knowledge of historical discussions.

---

## CG-001.10 Continuous Improvement

Engineering knowledge continuously evolves.

Standards shall therefore be reviewed and improved whenever

- business understanding increases,
- better engineering practices become available,
- architectural improvements are identified.

Continuous improvement shall preserve backward compatibility whenever reasonably possible.

---

# Engineering Culture

ERP DevCon promotes an engineering culture based on

- professional responsibility,
- technical excellence,
- constructive review,
- continuous learning,
- open discussion,
- documented decisions,
- mutual respect.

Engineering discussions are expected to improve the quality of products rather than defend individual opinions.

---

# Compliance

All company-wide standards shall be interpreted in accordance with the principles defined in this document.

Whenever conflicts arise between individual standards, the principles documented in the Company Philosophy shall take precedence until a new Architecture Decision Record defines otherwise.

---

# Related Documents

- ADR-0000 – Establish Engineering Documentation Repository
- Company Guide – Introduction
- Documentation Standards
- Architecture Principles

---

# Revision History

| Version | Date | Description |
|----------|------------|---------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |