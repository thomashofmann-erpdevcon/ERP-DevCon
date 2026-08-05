---
document: CG-022
title: Business Objects and Business Transactions
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

# Business Objects and Business Transactions

## Purpose

This document defines one of the fundamental architectural concepts used throughout ERP DevCon software products.

Business software consists of two fundamentally different categories of information:

- Business Objects
- Business Transactions

Understanding and consistently separating these concepts is essential for creating maintainable, auditable and historically correct software.

---

# Scope

These principles apply to

- business analysis,
- domain modelling,
- solution design,
- technical design,
- software implementation.

---

# BOT-001 Business Objects

Business Objects represent relatively stable entities within the business domain.

A Business Object describes *what exists*.

Examples include

- Employee
- Customer
- Vendor
- Product
- Contract
- Project
- Cost Center
- Warehouse

Business Objects are primarily descriptive.

---

# BOT-002 Business Transactions

Business Transactions describe events.

A Business Transaction records *what happened*.

Examples include

- Employment started
- Working hours posted
- Vacation approved
- Invoice posted
- Payment received
- Inventory adjusted
- Contract terminated

Business Transactions create business history.

---

# BOT-003 Separation of Responsibilities

Business Objects describe identity.

Business Transactions describe change.

Business Objects shall not contain historical information that properly belongs to Business Transactions.

---

# BOT-004 Historical Correctness

Historical business information shall normally remain immutable.

Corrections should be represented by new Business Transactions rather than modifying historical transactions.

This principle ensures

- auditability,
- traceability,
- reproducibility.

---

# BOT-005 Current State

The current business state should be derivable from

- Business Objects
- Business Transactions

The current state shall not become an independent source of truth.

Whenever practical, the current state should be reproducible from recorded history.

---

# BOT-006 Responsibility

Every Business Transaction shall reference the Business Objects it affects.

Business Objects shall not require knowledge of future transactions.

The dependency direction is therefore

Business Transaction

↓

Business Object

not vice versa.

---

# BOT-007 Lifecycle

Business Objects have a lifecycle.

Business Transactions document lifecycle events.

Example

Employee

↓

Employment Started

↓

Working Time Recorded

↓

Vacation Granted

↓

Employment Ended

The Employee remains the Business Object.

The events constitute the Business History.

---

# BOT-008 Information before Automation

Business Transactions shall primarily preserve business information.

Automation may use this information to perform calculations or trigger business processes.

Automation shall never replace the recorded business history.

---

# BOT-009 Product Independence

The distinction between Business Objects and Business Transactions is independent of implementation technology.

It applies equally to

- Business Central
- SQL Server
- REST Services
- Event-driven architectures
- Ledger systems
- Document databases

The concept belongs to the business architecture.

---

# BOT-010 Ledger-Oriented Thinking

Whenever practical, business history should be represented as append-only Business Transactions.

Business Objects represent the current business identity.

Business Transactions represent business history.

This distinction supports

- historical reconstruction,
- auditing,
- reporting,
- analytics,
- future product evolution.

---

# Examples

## Time Management

Business Object

Employee

Business Transactions

- Work Time Recorded
- Vacation Requested
- Vacation Approved
- Vacation Consumed
- Overtime Generated
- Time Correction Posted

---

## Financial Accounting

Business Object

General Ledger Account

Business Transactions

- Journal Posting
- Payment
- Allocation
- Reversal

---

## Warehouse

Business Object

Item

Business Transactions

- Receipt
- Shipment
- Transfer
- Adjustment
- Consumption

---

# Related Documents

- Business Domain Modeling
- Architecture Principles
- Engineering Principles
- Functional Requirement
- Solution Design

---

# Revision History

| Version | Date | Description |
|----------|------------|--------------------------|
| 0.1.0 | 2026-08-05 | Initial draft |