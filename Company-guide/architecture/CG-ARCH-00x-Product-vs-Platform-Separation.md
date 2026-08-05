# CG-ARCH-00x – Product versus Platform Separation

## Principle

A product shall be defined independently of any implementation platform.

## Product

A product owns

- Functional Requirements
- Solution Design
- Change Requests
- Decision Log

## Platform

Each platform owns

- Technical Design
- Testing
- Deployment
- Platform Release Notes

## Motivation

A single product may be implemented on multiple platforms.

Each implementation shares the same business behaviour while using
platform-specific technical solutions.

## Result

Business knowledge exists only once.

Technical implementations may exist multiple times.