# NONO-GATE â€” Deterministic Governance Gate

[Ledger: Append-Only]  
[Deterministic Hashing]  
[Policy Enforced]  
[CI Ready]

---

## What Problem Does This Solve?

Modern pipelines detect issues.  
NONO-GATE enforces deterministic governance.

It ensures:
- Staging integrity
- Deterministic evidence generation
- Unexpected file injection detection
- Tamper-evident governance trail

This is enforcement â€” not passive validation.

---

## Quick Demo

PASS:
npm run govern:pass

FAIL:
npm run govern:fail

FAIL output example:
STAGING_UNEXPECTED_FILE:INJECTED_UNEXPECTED_FILE.txt

---

## Core Capabilities

- Deterministic SHA256 root hashing
- Append-only governance ledger
- Governance anchor snapshot
- SBOM generation layer
- Key-leak detection gate
- Strict CI enforcement

---

## Architecture Model

1. Canonical normalization
2. Sorted deterministic hashing
3. Evidence bundle generation
4. Ledger chain update
5. Governance anchor lock

---

## Positioning

NONO-GATE is a governance infrastructure layer  
for build integrity, release control, and compliance-grade evidence.

Full enforcement demo included in /demo.
---

## Why This Is Not Another Scanner

Most tools detect problems.

NONO-GATE enforces deterministic build governance.

It does NOT:
- Lint code
- Detect vulnerabilities
- Replace SAST tools

It DOES:
- Enforce staging boundaries
- Block unexpected file injection
- Produce reproducible cryptographic evidence
- Maintain tamper-evident governance trail

This positions NONO-GATE as governance infrastructure,
not a detection utility.

---

## Governance Proof Snapshot

This demo includes a deterministic evidence run.

Example root hash (demo run):

9B5BA43536BB72F810D7560D27BBC73A439F2A2C144E04B841382217C2F802FF

Re-running the same staging produces the same root hash.

This demonstrates deterministic reproducibility.


---

## Enterprise Adoption Path

### Step 1 — Add to CI

Install NONO-GATE in your pipeline container:

npm install nono-gate --omit=dev

### Step 2 — Define Governance Policy

Create policy.json defining allowed staging structure.

### Step 3 — Enforce in CI

Run:

npx nono enterprise --staging ./build --policy ./policy.json

Pipeline fails automatically if:

- Unexpected file appears
- Staging structure changes
- Governance boundary is violated

### Step 4 — Archive Evidence

Store:
- BUNDLE_ROOT_SHA256
- Ledger entry
- Governance anchor

This enables:

- Release integrity verification
- Compliance evidence traceability
- Tamper-evident build audit

---

## Intended Audience

- DevSecOps teams
- Platform engineering teams
- Compliance-sensitive environments
- Release engineering teams

NONO-GATE is not built for hobby pipelines.
It is built for deterministic governance control.


---

## Where NONO-GATE Sits in the Toolchain

Build security stack typically looks like this:

Detection Layer:
- SAST tools
- Dependency scanners
- Secret scanners

Artifact Integrity Layer:
- Code signing
- Container signing
- SBOM generators

Governance Enforcement Layer:
- NONO-GATE

NONO-GATE does not replace detection tools.
It enforces deterministic governance boundaries over build outputs.

It ensures:
- What enters staging is exactly what policy allows.
- No unexpected file crosses release boundary.
- Evidence remains reproducible across runs.

This places NONO-GATE between detection and release integrity,
as a deterministic governance enforcement layer.


<!-- Signed commit trigger -->

<!-- unsigned test -->
