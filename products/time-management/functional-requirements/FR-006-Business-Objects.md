---
document: FR-006
title: Business Objects
product: Time Management
status: Approved
version: 1.0
---

# FR-006 – Business Objects

## Purpose

This document defines the business objects of the Time Management domain.

Business Objects represent the stable business entities that are managed or
referenced by the Time Management domain. They provide the foundation for
Business Transactions, Business Rules and Business Processes.

The Time Management domain owns only those Business Objects that belong to
its bounded context. Other Business Objects are referenced from external
business domains.

---

# BO-001 – Employment Relationship

## Purpose

An Employment Relationship represents the business context in which planned
time entitlements are managed.

Every activity performed by the Time Management domain belongs to exactly
one Employment Relationship.

The Employment Relationship establishes the context for all Business
Transactions, Business Rules and Business Processes within the Time
Management domain.

## Responsibilities

An Employment Relationship is responsible for providing the business context
required to manage planned time entitlements.

It defines the period during which the Time Management domain applies to a
person and provides access to all information required to determine
applicable Business Rules.

## Business Rules

- Every planned time entitlement belongs to exactly one Employment
  Relationship.
- Every Business Transaction belongs to exactly one Employment
  Relationship.
- An Employment Relationship owns exactly one Time Account.
- At every point in time exactly one applicable Working Time Model shall be
  determinable.
- At every point in time exactly one applicable Standard Calendar shall be
  determinable.

## Out of Scope

The Employment Relationship is not responsible for:

- Personnel Administration
- Payroll
- Attendance Recording
- Absence Recording
- Organisational Structures

These capabilities belong to other business domains and provide information
to the Time Management domain.

---