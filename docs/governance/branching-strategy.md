# Branching Strategy

## Purpose

This document defines the Git branching strategy used across the AstraMind ecosystem.

The objective is to provide a simple, consistent, and predictable workflow that supports parallel development, stable releases, and traceable history.

---

# Branch Types

## main

The `main` branch represents the latest stable production-ready code.

Rules:

- Always deployable
- Protected branch
- No direct commits
- Pull Requests required
- Passing CI required before merge

---

## feature/*

Used for new functionality.

Examples:

```
feature/workflow-engine
feature/comfyui-connector
feature/image-editing
```

Rules:

- Created from `main`
- One feature per branch
- Deleted after merge

---

## bugfix/*

Used for defect corrections.

Examples:

```
bugfix/session-timeout
bugfix/api-validation
```

---

## hotfix/*

Used for urgent production fixes.

Examples:

```
hotfix/security-patch
hotfix/login-failure
```

Hotfix branches should be short-lived and merged back into `main` immediately after validation.

---

## release/*

Optional release stabilization branches.

Examples:

```
release/v1.0.0
release/v1.1.0
```

---

# Branch Naming

Use lowercase and hyphen-separated names.

Examples:

```
feature/workflow-engine
feature/template-manager
bugfix/api-timeout
hotfix/authentication
```

Avoid spaces, underscores, and version numbers in feature branches.

---

# Merge Strategy

Preferred merge method:

- Squash Merge for feature branches
- Merge Commit for release branches
- Preserve history for significant architectural work

---

# Commit Messages

Recommended format:

```
type: short description
```

Examples:

```
feat: add workflow execution engine
fix: resolve session persistence issue
docs: update software architecture specification
refactor: simplify connector abstraction
test: add integration tests for image workflow
```

---

# Pull Requests

Every Pull Request should include:

- Summary of changes
- Motivation
- Testing performed
- Related Issue or ADR (if applicable)

---

# Summary

A simple branching strategy reduces complexity while maintaining a clean and traceable project history.