# Contributing Guidelines

## Purpose

This document defines the working principles for all contributors to the ERP DevCon Engineering Repository.

The objective is to ensure that documentation, architectural decisions and engineering knowledge remain consistent, maintainable and traceable throughout the lifetime of the repository.

---

# General Principles

Every contribution shall improve the quality of the repository.

Contributors are expected to prioritize

- clarity
- consistency
- maintainability
- traceability
- long-term usability

over short-term convenience.

---

# Documentation Language

The official documentation language is English.

Business terminology shall remain consistent across all documents.

If a business term has been defined in the glossary, the glossary definition shall always be used.

---

# Single Source of Truth

Every business rule, architectural principle or technical standard shall have exactly one authoritative definition.

Duplicate documentation shall be avoided.

Documents shall reference existing definitions instead of copying them.

---

# Repository Structure

Documentation shall always be stored in the appropriate section of the repository.

Company-wide principles belong to

/company-guide

Architecture decisions belong to

/architecture/adr

Technical standards belong to

/standards

Reusable document templates belong to

/templates

Business terminology belongs to

/glossary

Product-specific documentation belongs to

/products

Research material belongs to

/research

Archived documentation belongs to

/archive

---

# Markdown

Markdown is the authoritative source format.

Generated Word and PDF documents are considered publication formats.

The Markdown sources always take precedence.

---

# Branch Strategy

Documentation shall never be developed directly in the main branch.

Development takes place in dedicated working branches.

Examples

company-guide

time-management

business-central

research

Additional feature branches may be created whenever appropriate.

---

# Commit Messages

Each commit shall represent one logical change.

Commit messages should be short, descriptive and written in English.

Examples

Add company philosophy

Add ADR-0001 Business before Technology

Update documentation standards

Correct glossary definitions

Avoid generic commit messages such as

Update

Changes

Fix

Miscellaneous

---

# Reviews

Important documentation shall be reviewed before being merged.

The review focuses on

- correctness
- consistency
- terminology
- completeness
- readability

Review comments shall improve the document rather than merely identify problems.

---

# Architecture Decision Records

Fundamental engineering decisions shall be documented as Architecture Decision Records (ADR).

An ADR records

- the problem
- the decision
- the rationale
- the expected consequences

The Company Guide references ADRs but does not duplicate their contents.

---

# Product Documentation

Each product maintains its own documentation.

Typical product documentation includes

- Functional Requirements
- Solution Design
- Technical Design
- Decision Log
- Change Request Backlog
- Test Documentation
- Release Notes

Company standards remain independent from product documentation.

---

# Continuous Improvement

Documentation is considered a living asset.

Improvements are encouraged whenever they

- increase clarity,
- remove ambiguity,
- eliminate redundancy,
- improve consistency,
- simplify maintenance.

Documentation quality is regarded as an essential part of software quality.