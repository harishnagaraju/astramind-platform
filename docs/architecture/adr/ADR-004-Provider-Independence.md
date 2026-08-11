---
ADR Number      : ADR-004
Title           : AI Provider Independence
Status          : Accepted
Category        : Integration
Version         : 1.0
Created         : 2026-08-11
Last Updated    : 2026-08-11
Author          : Harish Nagaraju
Reviewers       : TBD
Related Chapters: SAS Chapter 14
Related ADRs    : ADR-006, ADR-010
Supersedes      : None
Superseded By   : None
Tags            : Provider Independence, OpenAI, ComfyUI, Ollama
---

# ADR-004

# AI Provider Independence

Status: Accepted

---

## Decision

The Domain Model SHALL remain independent of all AI providers.

Examples include:

- OpenAI

- ComfyUI

- Ollama

- LM Studio

- Future Providers

All providers SHALL be integrated through Adapters.
