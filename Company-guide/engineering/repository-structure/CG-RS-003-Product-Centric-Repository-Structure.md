# CG-RS-003 – Product-Centric Repository Structure

## Purpose

Define the standard repository structure for ERP DevCon products.

## Principle

A repository is organised around products.

All artefacts belonging to a product shall be stored below the product root
directory.

The product represents the primary organisational unit.

Platforms are implementation details of the product.

## Repository Structure

/products/
    <product>/
        functional-requirements/
        solution-design/
        platform/
            business-central/
            finance-and-operations/
            sap/
            ...
        change-requests/
        decision-log/
        release-notes/

## Rationale

Developers, architects and consultants usually work on a product rather than
on a platform.

Keeping all product artefacts together

- improves discoverability,
- simplifies navigation,
- keeps traceability intact,
- avoids duplication of documentation.

Platform-specific artefacts are grouped below the corresponding platform
inside the product.

## Consequences

Functional Requirements and Solution Design are shared across all platform
implementations.

Technical Design, Testing and Deployment remain platform-specific.