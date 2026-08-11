# Versioning Policy

## Purpose

This document defines the versioning strategy used across the AstraMind ecosystem.

---

# Semantic Versioning

AstraMind follows Semantic Versioning (SemVer).

```
MAJOR.MINOR.PATCH
```

---

## MAJOR

Increment when incompatible architectural or API changes are introduced.

Example:

```
1.x.x

↓

2.0.0
```

---

## MINOR

Increment when new functionality is added while maintaining backward compatibility.

Example:

```
1.2.0

↓

1.3.0
```

---

## PATCH

Increment for:

- Bug fixes
- Documentation improvements
- Internal optimizations

Example:

```
1.3.1

↓

1.3.2
```

---

# Pre-release Versions

Optional identifiers:

```
1.0.0-alpha

1.0.0-beta

1.0.0-rc1
```

---

# Documentation Versioning

Major documentation should align with the platform version.

Examples:

```
ASTRAMIND_SAS_v1.0.md

ADR-001

Connector Specification v1.0
```

---

# Backward Compatibility

Minor and Patch releases should preserve backward compatibility whenever practical.

Breaking changes should be introduced only in Major releases.

---

# Version Tags

Git tags should use the following format:

```
v1.0.0

v1.1.0

v1.1.1
```

---

# Summary

Consistent versioning improves predictability, traceability, and long-term maintainability across the AstraMind ecosystem.