# PSVS Defect Log

**System:** Polar Seed Vault System  
**Baseline:** PSVS-REQ-v1.0  
**Analysis status:** Initial review  
**Status convention:** Open = not yet corrected or formally accepted

## Defect Findings

| Defect ID | Req ID | Category | Description | Evidence | Severity | Suggested fix | Status |
|---|---|---|---|---|---|---|---|
| DF-01 | S1 | Incompleteness | Depositor registration rules are missing. | "registered depositors" | Medium | Define registration, approval, and suspension rules. | Open |
| DF-02 | S1 | Non-verifiability | Acceptance behavior is not linked to a defined registration check. | "only from registered depositors" | High | Specify an authorization check and rejection test for unregistered depositors. | Open |
| DF-03 | S2 | Vagueness | "Large number" is not measurable. | "a large number of boxes" | Medium | Replace with numeric chamber capacities or refer to S3 explicitly. | Open |
| DF-04 | S2, S3 | Redundancy | S2's general capacity statement adds little measurable detail beyond S3. | S2 uses a general capacity phrase; S3 supplies limits. | Low | State that each chamber must support its defined capacity in S3. | Open |
| DF-05 | S3 | Incompleteness | No behavior is specified when a chamber reaches capacity. | Capacity maxima are given, but full-chamber handling is not. | Medium | Require rejection or safe rerouting when capacity is reached. | Open |
| DF-06 | S3 | Non-verifiability | The method for counting stored boxes is not specified. | "at most 50,000 boxes" | Medium | Define when deposits, withdrawals, and quarantined boxes count toward capacity. | Open |
| DF-07 | S4 | Incompleteness | The process for verifying depositor identity is absent. | "only that depositor may withdraw it" | High | Define authenticated identity and authorization checks. | Open |
| DF-08 | S4, S5 | Contradiction / ambiguity | Ordinary withdrawal is restricted to the owner, while emergency release permits release to any requesting party. Priority and authorization rules are unclear. | "only that depositor" versus "any requesting party" | Critical | Define an explicit emergency exception, authorized approver, scope, and audit requirements. | Open |
| DF-09 | S5 | Ambiguity | "Emergency" and "vault authority" are undefined. | "In an emergency, the vault authority" | High | Define qualifying emergencies and authorized roles. | Open |
| DF-10 | S5, S12 | Incompleteness | Emergency release does not explicitly specify what records must be retained. | Emergency release is allowed; audit requirements are general. | High | Require recording of reason, approver, recipient, box ID, and timestamp. | Open |
| DF-11 | S6, S7 | Vagueness | S6 uses "safe temperature" even though S7 supplies a numeric ceiling. | "safe temperature" and "above -18°C" | Medium | Define acceptable storage temperature and clarify the relationship between both requirements. | Open |
| DF-12 | S7, S8 | Contradiction | S7 prohibits temperatures above -18°C, whereas S8 allows warming to 0°C during maintenance. No explicit exception is defined. | "never rise above -18°C" versus "warmed to 0°C" | Critical | Define a controlled maintenance exception and the applicable temperature rules. | Open |
| DF-13 | S8 | Incompleteness | Maintenance warming lacks duration, approval, monitoring, and restoration requirements. | "During maintenance" and "may be warmed to 0°C" | High | Define permitted duration, authorization, monitoring, and return-to-storage conditions. | Open |
| DF-14 | S9 | Vagueness | "Low viability" has no numerical threshold. | "low viability" | High | Specify a viability threshold by species or an approved species-specific policy. | Open |
| DF-15 | S9 | Missing timing constraint | "Promptly" has no measurable deadline. | "flagged promptly" | Medium | Define a maximum delay between receiving viability data and flagging a sample. | Open |
| DF-16 | S9 | Incompleteness | The required response after a low-viability flag is unclear. | "for regeneration" | Medium | Define notification, review, regeneration approval, and tracking steps. | Open |
| DF-17 | S10 | Ambiguity / missing data definition | The 20% rule does not define the annual period or how the eligible box count is calculated. | "20% of its boxes of a species per year" | High | Define the annual window, baseline quantity, rounding, and cumulative accounting. | Open |
| DF-18 | S10, S11 | Incompleteness | It is unclear how a withdrawn box that is later redeposited affects the annual withdrawal allowance. | Withdrawal quota and redeposit rules are specified separately. | Medium | Define whether redeposit changes quota accounting and how re-inspection is recorded. | Open |
| DF-19 | S11 | Incompleteness | The re-inspection criteria and authorization are unspecified. | "only after re-inspection" | Medium | Define inspection checks, responsible role, and acceptance or rejection outcomes. | Open |
| DF-20 | S12 | Vagueness / non-verifiability | "Good audit trail" does not define event coverage, integrity, access, or retention. | "good audit trail of all actions" | High | Define mandatory events, immutable or tamper-evident records, access controls, and retention periods. | Open |

## Cross-Requirement Findings

The following findings depend on relationships between multiple requirements:

- DF-04: S2 and S3 — general versus quantified capacity.
- DF-08: S4 and S5 — ownership-based withdrawal versus emergency release.
- DF-10: S5 and S12 — emergency release versus audit evidence.
- DF-11: S6 and S7 — general temperature safety versus a numeric limit.
- DF-12: S7 and S8 — normal temperature ceiling versus maintenance warming.
- DF-18: S10 and S11 — annual withdrawal accounting versus redeposit after inspection.

## Analysis Notes

- The capacity and ownership requirements are not automatically defective simply because they are brief. The logged defects identify missing operational details or verification criteria.
- DF-08 and DF-12 require stakeholder decisions, not just wording changes.
- The findings are proposals for review; no corrected requirement is considered approved until a change request is authorized.
