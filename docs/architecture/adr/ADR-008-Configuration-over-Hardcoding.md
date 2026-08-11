---
ADR Number      : ADR-008
Title           : Configuration over Hardcoding
Status          : Accepted
Category        : Configuration
Version         : 1.0
Created         : 2026-08-11
Last Updated    : 2026-08-11
Author          : Harish Nagaraju
Reviewers       : TBD
Related Chapters: SAS Chapter 18
Related ADRs    : ADR-009
Supersedes      : None
Superseded By   : None
Tags            : Configuration, JSON, YAML, Environment
---

# ADR-008

# Configuration over Hardcoding

---

## Status

Accepted

---

## Date

August 2026

---

## Context

AI systems evolve rapidly.

Model names

Endpoints

Workflow templates

Prompt templates

Runtime parameters

Provider URLs

Deployment environments

change frequently.

Embedding these values directly into source code increases maintenance cost.

---

## Problem Statement

How should AstraMind manage platform configuration?

---

## Decision

Platform behavior SHALL be driven through configuration rather than hardcoded implementation.

Examples include:

- Workflow Definitions
- Prompt Templates
- AI Models
- Runtime Selection
- Provider Endpoints
- Database Connections
- Feature Flags

Configuration SHALL be externalized.

---

## Preferred Formats

- JSON
- YAML
- TOML
- Environment Variables

---

## Hardcoded Values

Hardcoded values SHALL be limited to:

- Mathematical Constants
- Protocol Constants
- Internal Framework Values

Business configuration SHALL NOT be hardcoded.

---

## Consequences

### Positive

- Easier Deployment
- Simpler Maintenance
- Environment Independence
- Better Version Control

### Negative

Requires robust configuration validation.

---

## References

Chapter 18

Coding Standards