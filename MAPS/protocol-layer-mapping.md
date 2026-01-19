# Protocol–Layer Mapping — Robotic Networking

**Domain:** roboticnetworking.com  
**Repository:** roboticnetworking-evidence  
**Reference model:** Robotic Networking Layer Model (RNLM)  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Purpose

This mapping operationalizes the RNLM model by assigning **protocol families and
interface concepts** to the corresponding **networking layers**.

The mapping is classificatory only.  
It does not evaluate suitability, performance, or preference.

---

## Networking layers (in scope)

- **Layer 1 — Transport & Connectivity**
- **Layer 2 — Middleware & Data Exchange**
- **Layer 3 — Coordination & System Boundaries**

Layers outside this model are out of scope.

---

## Protocol and interface families

- IP-based transport protocols  
- Real-time and streaming transport  
- Traffic differentiation and determinism  
- Robotics middleware and data distribution  
- Industrial data exchange interfaces  
- Time synchronization and coordination interfaces

---

## Protocol–layer mapping

| Protocol / Interface family | Layer | Notes |
|-----------------------------|-------|-------|
| UDP                         | Transport & Connectivity | Best-effort packet transport |
| TCP                         | Transport & Connectivity | Reliable, connection-oriented transport |
| RTP                         | Transport & Connectivity | Real-time media transport |
| DiffServ                    | Transport & Connectivity | Traffic classification and handling |
| IEEE 802.1 TSN              | Transport & Connectivity | Deterministic networking concepts |
| DDS                         | Middleware & Data Exchange | Data-centric publish/subscribe |
| ROS 2 Interfaces            | Middleware & Data Exchange | Messages, services, actions |
| OPC UA                      | Middleware & Data Exchange | Structured data and service exchange |
| IEEE 1588 (PTP)             | Coordination & System Boundaries | Time synchronization |
| Coordination contracts      | Coordination & System Boundaries | Interface-level alignment |
| Orchestration handoffs      | Coordination & System Boundaries | System boundary transitions |

---

## Boundary constraints

- Protocol placement reflects **primary responsibility**, not exclusive use.
- No protocol implies semantic interpretation of data.
- Middleware does not guarantee coordination correctness.
- Coordination interfaces require explicit documentation.

---

## Explicit exclusions

The following mappings are explicitly excluded:

- Application or autonomy logic  
- Vendor-specific protocol extensions  
- Performance or latency guarantees  
- Security posture or certification claims  

---

## Consistency rule

Any introduction of a new:
- protocol family, or
- networking layer

requires synchronized updates to:
- this file,
- `MODEL.md`, and
- `CHANGELOG.md`.

---

## Disclaimer

This document defines protocol-to-layer mappings only.  
It does not recommend, certify, or evaluate specific technologies.
