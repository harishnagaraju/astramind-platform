# ADR Dependency Matrix

---

## Purpose

This document records dependencies between Architecture Decision Records.

Changes to one ADR may require review of dependent ADRs.

---

| ADR | Depends On | Related ADRs |
|------|------------|--------------|
| ADR-001 | None | ADR-002 |
| ADR-002 | ADR-001 | ADR-006 |
| ADR-003 | ADR-001 | ADR-005, ADR-007 |
| ADR-004 | ADR-002 | ADR-006, ADR-010 |
| ADR-005 | ADR-003 | ADR-009 |
| ADR-006 | ADR-002 | ADR-004 |
| ADR-007 | ADR-001 | ADR-003 |
| ADR-008 | ADR-001 | ADR-009 |
| ADR-009 | ADR-003 | ADR-005 |
| ADR-010 | ADR-002 | ADR-004 |

---

Future ADRs SHALL update this matrix whenever new architectural dependencies are introduced.

---

End of Matrix