# PSVS Peer-Review Comparison

## 1. Purpose

Compare the original defect log with the findings identified by a classmate during an independent review of PSVS requirements S1–S12.

## 2. Review Participants

- Original reviewer: [Your Name / Roll Number]
- Peer reviewer: [Classmate Name / Roll Number]
- Review date: [YYYY-MM-DD]
- Baseline reviewed: PSVS-REQ-v1.0

## 3. Comparison Method

1. Exchange the two defect logs.
2. Compare the underlying issues, not just the defect IDs.
3. Match findings that describe the same underlying defect.
4. Record findings in the peer log that are missing from the original log.
5. Count the union of unique findings across both logs.

## 4. Peer Findings Missing from the Original Log

| Peer Finding ID | Requirement ID | Description of Missed Defect | Category | Accepted as Distinct? | Notes |
|---|---|---|---|---|---|
| P-01 | [S-ID] | [Actual peer finding] | [Category] | [Yes/No] | [Reason] |
| P-02 | [S-ID] | [Actual peer finding] | [Category] | [Yes/No] | [Reason] |
| P-03 | [S-ID] | [Actual peer finding] | [Category] | [Yes/No] | [Reason] |

Replace these illustrative rows with actual peer findings. Add rows as needed.

## 5. Detection Rate

Let:

- A = number of unique defects identified by the original reviewer.
- B = number of unique defects identified by the peer reviewer.
- I = number of distinct defects identified by both reviewers.
- U = size of the union of both sets of findings.

Formula:

Detection rate = A / U × 100%

Where:

U = A + B − I

## 6. Results

| Metric | Actual Result |
|---|---:|
| Original reviewer findings (A) | [Enter count] |
| Peer reviewer findings (B) | [Enter count] |
| Shared findings (I) | [Enter count] |
| Unique combined findings (U) | [A + B − I] |
| Original reviewer detection rate | [A / U × 100]% |

## 7. Reflection

The peer review helped identify gaps that may have been overlooked during the initial inspection. Differences in findings should be resolved by examining the original requirement text and the taxonomy definitions.

The final report should explain which peer findings were accepted, which were duplicates, and why any disputed findings were excluded.
