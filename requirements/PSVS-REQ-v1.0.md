# PSVS Requirements — Version 1.0

**Artifact ID:** PSVS-REQ-v1.0  
**System:** Polar Seed Vault System  
**Status:** Initial baseline  
**Requirements:** S1–S12

## 1. Informal Requirements

| ID | Requirement |
|---|---|
| S1 | The system shall accept seed boxes only from registered depositors. |
| S2 | Each chamber can hold a large number of boxes. |
| S3 | Chambers 1–3 hold at most 50,000 boxes each; Chamber 4 holds at most 20,000. |
| S4 | A box belongs to exactly one depositor, and only that depositor may withdraw it. |
| S5 | In an emergency, the vault authority may release any box to any requesting party. |
| S6 | Boxes shall be stored at a safe temperature. |
| S7 | Chamber temperature shall never rise above -18°C. |
| S8 | During maintenance, a chamber may be warmed to 0°C. |
| S9 | Seed samples with low viability shall be flagged promptly for regeneration. |
| S10 | A depositor may withdraw at most 20% of its boxes of a species per year. |
| S11 | A withdrawn box may be redeposited only after re-inspection. |
| S12 | The system shall keep a good audit trail of all actions. |

## 2. Scope

These requirements cover depositor registration, box ownership, storage capacity, temperature control, emergency release, seed viability, withdrawal limits, redeposit inspections, and auditing.

## 3. Baseline Rules

1. Preserve the original IDs S1–S12 for traceability.
2. Treat the wording above as the original requirements baseline.
3. Record identified defects separately from the original requirements.
4. Do not silently modify baseline requirements.
5. Propose corrections through formal change requests.

## 4. Known Analysis Concerns

The initial wording contains potentially ambiguous terms, missing operational details, and apparent conflicts requiring investigation.

Examples include:
- "Large number" in S2.
- "Safe temperature" in S6.
- The temperature limit in S7 versus maintenance warming in S8.
- Depositor-only withdrawal in S4 versus emergency release in S5.
- "Promptly" in S9 and "good audit trail" in S12.

These concerns are to be documented and assessed in the defect log.


