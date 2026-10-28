
# PSVS Defect Taxonomy

## Purpose

This taxonomy provides consistent categories for identifying defects in the Polar Seed Vault System's informal requirements.

| Code | Category | Definition | Example |
|---|---|---|---|
| D01 | Ambiguity | A statement supports two or more reasonable interpretations. | S5 does not define who qualifies as the "vault authority." |
| D02 | Vagueness | A statement uses imprecise terms without measurable criteria. | S6 uses "safe temperature." |
| D03 | Incompleteness | Necessary information or conditions are missing. | S1 does not define how depositor registration is verified. |
| D04 | Contradiction | Two requirements impose incompatible conditions in the same context. | S7 prohibits temperatures above -18°C, while S8 permits warming to 0°C during maintenance without an explicit exception. |
| D05 | Non-verifiability | A requirement lacks a clear objective test or acceptance criterion. | S12 requires a "good" audit trail without defining completeness or retention. |
| D06 | Redundancy | Requirements repeat the same obligation without adding distinct meaning. | S6 and S7 both address storage temperature, although S7 adds a specific limit. This is potential partial redundancy, not necessarily a duplicate. |
| D07 | Infeasibility | A requirement may be impossible or impractical to meet under its stated conditions. | A literal interpretation of S7 could make the permitted warming in S8 impossible. |
| D08 | Untraceability | A requirement lacks a clear link to its source, objective, or verification evidence. | A derived requirement to retain inspection records would be untraceable if its relationship to S11 were not recorded. |
| D09 | Missing exception handling | Exceptional conditions are not adequately specified. | S5 does not describe emergency authorization, expiry, or post-release documentation. |
| D10 | Missing data definition | A requirement does not define how a key quantity or status is represented. | S10 does not define whether the yearly withdrawal count is based on boxes, withdrawals, or net quantity. |
| D11 | Missing timing constraint | A time-related obligation lacks a measurable deadline or trigger. | S9 uses "promptly" without a maximum number of minutes or hours. |
| D12 | Missing access control | The required permissions or authorization checks are not fully specified. | S4 identifies who may withdraw a box but does not specify how identity is authenticated. |

## Classification Rules

1. Assign a primary category to each defect.
2. Record secondary categories when one issue genuinely fits multiple categories.
3. Use evidence from the requirement wording.
4. Distinguish confirmed wording defects from possible design risks.
5. Avoid counting the same underlying issue multiple times unless distinct consequences are documented.
6. Propose fixes separately from the original requirement text.

## Severity Scale

- **Critical:** May undermine ownership, seed safety, or emergency control.
- **High:** May lead to a major operational, security, or compliance failure.
- **Medium:** Creates a meaningful gap in interpretation, verification, or operation.
- **Low:** Primarily affects clarity, consistency, or maintainability.

Severity is an initial analytical assessment and should be confirmed during review.
