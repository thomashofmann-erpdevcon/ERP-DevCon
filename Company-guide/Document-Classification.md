---
document: CG-016
title: Document Classification
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

# Document Classification

## Purpose

This document defines the document types used within the ERP DevCon Engineering Repository.

Every engineering document shall belong to exactly one document class.

The classification determines the document's purpose, intended audience, lifecycle and relationships to other documents.

---

# Classification Principles

Document classes exist to separate responsibilities.

Each document type shall answer a specific engineering question.

Engineering information shall not be duplicated across document classes.

---

# Company Guide

## Purpose

Defines company-wide principles, governance and engineering philosophy.

## Answers

How does ERP DevCon work?

What engineering principles apply to every product?

## Typical Audience

- Management
- Architects
- Business Analysts
- Developers

---

# Engineering Standard

## Purpose

Defines reusable engineering practices independent of individual products.

## Answers

How should engineering activities be performed?

## Examples

- Business Analysis
- Requirements Engineering
- Software Engineering
- Coding Standards
- Testing

---

# Architecture Decision Record (ADR)

## Purpose

Documents one architectural decision.

## Answers

Why was this architectural decision made?

What alternatives were considered?

What are the consequences?

Each ADR shall describe one decision only.

---

# Functional Requirement

## Purpose

Defines required business behaviour.

## Answers

What shall the software do?

Functional Requirements intentionally avoid implementation details.

---

# Solution Design

## Purpose

Defines the logical software solution.

## Answers

How will the business requirements be fulfilled?

Solution Design remains implementation independent.

---

# Technical Design

## Purpose

Defines platform-specific implementation.

## Answers

How will the approved solution be implemented?

---

# Decision Log

## Purpose

Documents significant product decisions.

## Answers

Why was a product decision made?

Decision Logs complement Architecture Decision Records.

Architectural decisions belong in ADRs.

Product decisions belong in the Decision Log.

---

# Change Request

## Purpose

Documents requested functionality that is

- deferred,
- rejected,
- planned,
- postponed.

Change Requests preserve engineering knowledge beyond the current implementation scope.

---

# Template

## Purpose

Defines reusable document structures.

Templates improve

- consistency,
- readability,
- maintainability.

---

# Glossary

## Purpose

Defines terminology.

Every important business and engineering term shall have exactly one authoritative definition.

---

# Research Document

## Purpose

Documents investigations and evaluations.

Research documents may contain

- prototypes,
- experiments,
- comparisons,
- technology evaluations,
- feasibility studies.

Research documents are informative.

They do not define company standards.

---

# Product Documentation

## Purpose

Documents one specific software product.

Typical product documentation includes

- Functional Requirements
- Solution Designs
- Technical Designs
- Decision Logs
- Change Requests
- Release Notes

Product documentation shall never redefine company standards.

---

# Relationship Between Document Classes

Company Guide

↓

Engineering Standards

↓

Architecture Decision Records

↓

Product Documentation

↓

Implementation

↓

Testing

↓

Release

Each document class has a unique responsibility within the engineering lifecycle.

---

# Continuous Improvement

New document classes may be introduced whenever they provide

- better separation of concerns,
- improved maintainability,
- reduced duplication,
- increased engineering clarity.

The repository structure shall evolve together with the engineering process.

---

# Related Documents

- Company Guide
- Documentation Principles
- Document Lifecycle
- Architecture Decision Records
- Repository README

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |