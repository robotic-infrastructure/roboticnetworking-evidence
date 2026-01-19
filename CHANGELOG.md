# Changelog — Robotic Networking Evidence Layer

**Domain:** roboticnetworking.com  
**Repository:** roboticnetworking-evidence  
**Versioning scheme:** semantic (vX.Y)

---

## v1.0 — 2026-01-19

### Added
- Public reference page (`index.html`) describing robotic networking layers and interface boundaries
- Evidence repository baseline:
  - `README.md` (purpose, scope overview, repository discipline)
  - `SCOPE.md` (included and excluded boundaries for robotic networking)
  - `SOURCES.md` (protocol and standards anchors, stable canonical sources)
  - `MODEL.md` (Robotic Networking Layer Model — RNLM)
  - `MAPS/protocol-layer-mapping.md` (protocol and interface family mappings)

### Scope
- Defined robotic networking as a layered interface discipline:
  - Transport & Connectivity
  - Middleware & Data Exchange
  - Coordination & System Boundaries
- Explicit exclusion of application logic, autonomy behavior, benchmarking, and vendor evaluation

### Model
- Introduced the RNLM with three non-overlapping layers
- Clarified one-directional dependency rules between layers
- Positioned interoperability as a boundary condition, not a feature claim

### Sources
- Anchored networking concepts in IETF, IEEE, OMG, ROS 2, and OPC UA specifications
- Ensured all references are canonical, stable, and non-marketing

### Constraints
- Prohibited performance, security, or certification claims
- Prohibited vendor- or product-specific comparisons
- Required explicit documentation for any future scope or model changes

---

## Versioning policy

- Minor versions (`v1.1`, `v1.2`, …) document:
  - scope clarifications,
  - additional protocol references,
  - mapping refinements.

- Major versions (`v2.0`, …) indicate:
  - fundamental model or scope restructuring.

All changes are additive or explicitly deprecated.  
No silent removals are permitted.

---

## Disclaimer

This changelog documents structural and editorial changes only.  
It does not express endorsement, certification, or operational guarantees.
