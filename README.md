# VV Lab — Polar Seed Vault System (PSVS)

## Project Overview

This repository contains the requirements, defect analysis, verification records, and configuration management artifacts for the Polar Seed Vault System (PSVS).

The system stores sealed crop seed boxes deposited by registered institutions. Depositors retain ownership of their boxes, while the vault acts as a custodian.

## Objectives

- Manage and version system requirements.
- Identify defects in informal requirements.
- Classify defects using a defined taxonomy.
- Maintain defect logs and peer-review records.
- Track changes through Git branches, commits, and tags.
- Improve requirement clarity, consistency, completeness, and verifiability.

## Repository Structure

| Folder | Purpose |
|---|---|
| `requirements/` | Versioned system requirements |
| `defect-logs/` | Defect taxonomy, defect log, and peer review |
| `abstractions/` | System scope, actors, and conceptual abstractions |
| `models/` | System models and diagrams |
| `operations/` | Operational procedures |
| `constraints/` | Capacity, temperature, and withdrawal constraints |
| `proofs/` | Verification arguments and evidence |
| `reports/` | Summary reports, charts, and change-request template |

## Baseline

- Requirement version: PSVS-REQ-v1.0
- Baseline tag: `baseline-1`
- Original requirement IDs: S1–S12

## Configuration Management

Git is used to manage artifact versions. The initial requirements are committed as a baseline. Subsequent defect-analysis changes are developed on a separate branch and merged into `main`.

## Defect Analysis

The informal requirements are reviewed for ambiguity, vagueness, incompleteness, contradiction, non-verifiability, redundancy, infeasibility, and untraceability, along with other relevant defect categories.

## Important Note

Defect findings are analysis results, not confirmed implementation failures. Suggested fixes are proposals and should be approved before becoming normative requirements.

## Author

- Student: MUHAMMAD JAWAD SABIR
- Roll Number: BSSE-SP/24-073
- Course/Lab: Verification and Validation / PSVS

