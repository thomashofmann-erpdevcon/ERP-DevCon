---
document: CG-014
title: Engineering Glossary
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

# Engineering Glossary

## Purpose

The Engineering Glossary defines the official terminology used throughout the ERP DevCon Engineering Repository.

Every engineering document shall use the terminology defined in this glossary.

A business or technical term shall have exactly one authoritative definition.

---

# Business Analysis

The engineering discipline responsible for understanding the business domain and defining business requirements independently from technical implementation.

---

# Business Object

A business entity that represents a meaningful concept within the business domain.

A Business Object has

- a defined responsibility,
- a lifecycle,
- business relationships,
- business behaviour.

Examples include Customer, Employee, Contract and Work Time Entry.

---

# Business Process

A sequence of business activities performed to achieve a business objective.

Business Processes are independent of software implementation.

---

# Business Rule

A rule that defines or constrains business behaviour.

Business Rules originate from the business domain and are implemented by software.

---

# Business Transaction

A business event that changes business reality.

Business Transactions create business history.

Historical information should be derived from Business Transactions whenever practical.

---

# Company Guide

The collection of company-wide engineering principles, organizational rules and documentation standards.

The Company Guide applies to all products.

---

# Functional Requirement (FR)

A document describing required business behaviour.

Functional Requirements define

- business processes,
- business rules,
- business information,
- expected behaviour.

They intentionally avoid implementation details.

---

# Solution Design (SD)

A document describing the logical software solution implementing approved Functional Requirements.

Solution Design remains independent from implementation technologies.

---

# Technical Design (TDD)

A document describing the technical implementation of an approved Solution Design.

Technical Design contains platform-specific implementation details.

---

# Architecture Decision Record (ADR)

A document recording an important architectural decision.

An ADR explains

- the problem,
- considered alternatives,
- the decision,
- the rationale,
- expected consequences.

---

# Company Standard

A document defining company-wide engineering principles.

Company Standards apply across all products.

---

# Product Documentation

Documentation belonging to one specific software product.

Typical examples include

- Functional Requirements,
- Solution Designs,
- Technical Designs,
- Decision Logs,
- Change Request Backlogs,
- Release Notes.

---

# Decision Log

A chronological record of significant product decisions that are not Architecture Decision Records.

Decision Logs preserve engineering knowledge throughout product development.

---

# Change Request

A documented request for new functionality or changes to existing functionality.

Deferred functionality shall remain visible within the Change Request Backlog.

---

# Single Source of Truth

The principle that every engineering concept has exactly one authoritative definition.

Duplicate definitions shall be avoided.

---

# Traceability

The ability to follow engineering information through the complete software lifecycle.

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

# Working Draft

A document under active development.

Working Drafts may change without notice until they enter formal review.

---

# Approved

A reviewed document accepted as an official engineering standard.

Approved documents may only be changed through the defined review process.

---

# Deprecated

A document that is no longer recommended for future use but remains available for historical reference.

---

# Archived

A document retained for historical purposes and no longer actively maintained.

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |