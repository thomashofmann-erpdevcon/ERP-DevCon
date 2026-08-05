---
document: CG-017
title: Repository Structure
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

# Repository Structure

## Purpose

This document defines the structure of the ERP DevCon Engineering Repository.

The repository structure is intended to provide a stable and scalable organization for engineering knowledge, product documentation and reusable engineering assets.

A consistent repository structure improves navigation, traceability and long-term maintainability.

---

# Design Objectives

The repository shall

- separate company standards from product documentation,
- preserve engineering knowledge,
- support parallel product development,
- minimize duplication,
- remain scalable,
- support long-term maintenance.

---

# Engineering Repository

The repository is organized into logical domains.

```
ERP-DevCon
│
├── company-guide
├── architecture
├── standards
├── templates
├── glossary
├── products
├── libraries
├── research
└── archive
```

Each top-level directory has one clearly defined responsibility.

---

# company-guide

The Company Guide contains company-wide engineering principles.

Typical contents include

- Company Philosophy
- Documentation Principles
- Architecture Principles
- Software Engineering
- Project Management
- Knowledge Management

The Company Guide defines how ERP DevCon performs engineering.

---

# architecture

The architecture directory contains long-term architectural knowledge.

Typical contents include

- Architecture Decision Records
- Reference Architectures
- Architectural Patterns
- Architecture Guidelines

Architectural decisions shall remain independent from individual software products.

---

# standards

The standards directory contains reusable engineering standards.

Examples include

- Business Analysis
- Requirements Engineering
- Coding Standards
- Testing Standards
- SQL Standards
- Business Central Standards

Standards define engineering practice.

---

# templates

The templates directory contains reusable engineering document templates.

Examples include

- Functional Requirement
- Solution Design
- Technical Design
- ADR
- Decision Log
- Change Request

Templates improve consistency throughout the repository.

---

# glossary

The glossary defines official business and engineering terminology.

Every important term shall have exactly one authoritative definition.

Documents shall reference glossary definitions whenever practical.

---

# products

Each software product maintains an independent documentation structure.

Example

```
products
    time-management
        functional-requirements
        solution-design
        technical-design
        decision-log
        change-requests
        testing
        releases
```

Products shall not redefine company-wide engineering standards.

---

# libraries

Reusable software components shall be documented independently from products.

Typical documentation includes

- purpose,
- interfaces,
- dependencies,
- version history,
- implementation notes.

Libraries are intended for reuse across multiple products.

---

# research

The research directory contains engineering investigations.

Typical contents include

- technology evaluations,
- prototypes,
- proof of concepts,
- white papers,
- experimental designs.

Research documents do not define company standards.

---

# archive

The archive contains obsolete or historical documentation.

Archived documents remain available for reference but are no longer maintained.

---

# Repository Evolution

The repository structure shall evolve together with the engineering organization.

New top-level directories should only be introduced when

- responsibilities cannot reasonably be represented within the existing structure,
- maintainability improves,
- engineering clarity increases.

Repository restructuring shall preserve document traceability.

---

# Naming Conventions

Directory names should

- remain stable,
- use lowercase,
- use hyphen-separated words,
- describe engineering responsibility.

Document names shall clearly describe their content.

Abbreviations should be avoided unless officially defined.

---

# Separation of Responsibilities

Each document shall belong to one logical engineering domain.

Information shall not be duplicated across directories.

Cross references are preferred over duplicated documentation.

---

# Related Documents

- Company Guide
- Documentation Principles
- Document Classification
- Architecture Decision Records
- Repository README

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |