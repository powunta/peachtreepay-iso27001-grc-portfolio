# MFA Corrective-Action Validation and Retest Workpaper

> **Simulated evidence and testing exercise — not a real client engagement or production-system review.**  
> All accounts, tickets, reports, approvals, corrective actions, and test results below were created for portfolio purposes.

## Retest Overview

| Field | Detail |
|---|---|
| Related risk | Risk 1 — Employee account compromised because MFA is not enabled everywhere |
| Original test | [MFA Control-Testing Workpaper](08-mfa-control-testing-workpaper.md) |
| Original result | Exception — control not operating effectively across the full population |
| Corrective-action owner | IT/Security |
| Simulated remediation period | October 1–14, 2026 |
| Simulated retest date | October 21, 2026 |
| Tester | GRC Analyst |
| Retest scope | Complete population of 108 in-scope Microsoft 365 and AWS human accounts |
| Retest criterion | 100% MFA enforcement or a documented, approved, time-bound exception with compensating controls |
| Framework alignment | ISO/IEC 27001:2022 Annex A 8.5; NIST CSF 2.0 PR.AA-03; SOC 2 CC6.1 alignment theme |

## Original Findings and Root-Cause Analysis

| Finding | Original condition | Root cause | Corrective action |
|---|---|---|---|
| MFA-EX-01 | One Microsoft 365 standard-user account lacked MFA and approval | The account remained in a legacy group excluded from the deployment policy | Removed the exclusion, enforced MFA, and added a review of policy exclusions to the provisioning checklist |
| MFA-EX-02 | One AWS human-user account lacked MFA and approval | The account was created outside the standard onboarding workflow | Enforced MFA, reviewed recent AWS human accounts, and required ticket-based approval for new IAM human users |
| MFA-EX-03 | One Microsoft 365 account had an approved temporary exception | The user required a transition period for a replacement authentication method | Issued the replacement method, verified enrollment, and closed the exception before its expiration |

## Simulated Corrective-Action Evidence

| Evidence ID | Simulated artifact | Validation performed | Result |
|---|---|---|---|
| E-MFA-R01 | Corrective-action tickets for MFA-EX-01 and MFA-EX-02 | Confirmed owner, action, date, and closure evidence | Sufficient |
| E-MFA-R02 | Updated Microsoft 365 MFA enforcement report | Confirmed all 100 Microsoft 365 human accounts were enforced | Sufficient |
| E-MFA-R03 | Updated AWS IAM credential report | Confirmed all 8 AWS human users were enforced | Sufficient |
| E-MFA-R04 | Updated MFA exception register | Confirmed the temporary exception was closed and no active exceptions remained | Sufficient |
| E-MFA-R05 | Revised account-provisioning checklist | Confirmed policy-exclusion review and AWS ticket approval were added | Sufficient |
| E-MFA-R06 | IT/Security owner attestation | Confirmed corrective actions were reviewed and approved for retest | Sufficient |

## Retest Procedures and Results

| Step | Retest procedure | Result | Workpaper conclusion |
|---:|---|---|---|
| 1 | Reconcile the refreshed account population to HR, Microsoft 365, and AWS inventories | Pass | All 108 in-scope human accounts were included |
| 2 | Compare every account to the updated Microsoft 365 and AWS enforcement reports | Pass | MFA was enforced for 108 of 108 accounts |
| 3 | Review the exception register for approval, owner, expiration, and compensating controls | Pass | No active exceptions remained |
| 4 | Inspect corrective-action tickets and configuration evidence for the two unsupported exceptions | Pass | Both original control failures were remediated and traceable |
| 5 | Inspect the revised provisioning checklist for preventive workflow changes | Pass | Root-cause corrective actions were incorporated into the process |
| 6 | Reperform enforcement checks for 15 accounts across standard, privileged, and AWS access | Pass | All selected accounts required MFA |
| 7 | Evaluate whether the evidence supports the proposed residual-risk score | Supported | Likelihood is reasonably reduced from 4 to 2 while impact remains 5 |

## Population Retest Summary

| System and account type | Population | MFA enforced | Active approved exception | Unsupported exception | Result |
|---|---:|---:|---:|---:|---|
| Microsoft 365 standard users | 94 | 94 | 0 | 0 | Pass |
| Microsoft 365 privileged users | 6 | 6 | 0 | 0 | Pass |
| AWS IAM human users | 8 | 8 | 0 | 0 | Pass |
| **Total** | **108** | **108** | **0** | **0** | **Pass** |

**Observed enforcement coverage:** 108 of 108 accounts, or **100%**, at the simulated retest date.

## Closure and Residual-Risk Decision

**Retest conclusion: Pass — the control operated effectively across the complete population at the simulated retest date.**

The two unsupported exceptions were corrected, the temporary exception was closed, and root-cause changes were added to the provisioning workflow. The finding may therefore be marked **Closed — Remediated and Retested** for this simulated exercise.

The evidence supports reducing likelihood from **4 (Likely)** to **2 (Unlikely)** while retaining impact at **5 (Severe)**. The resulting residual-risk score is **10 (Medium)**.

| Decision field | Outcome |
|---|---|
| Finding status | Closed — Remediated and Retested |
| Residual likelihood | 2 |
| Residual impact | 5 |
| Residual score | 10 — Medium |
| Simulated risk owner | IT/Security |
| Decision | Accept with continued monitoring |
| Monitoring requirement | Quarterly population reconciliation, exception review, and provisioning-workflow testing |

## Limitations and Ongoing Assurance

This point-in-time simulated retest does not prove that MFA will remain effective indefinitely. Continued assurance requires monitoring new accounts, privileged access, policy exclusions, authentication-method changes, and approved exceptions. Any future unsupported exception should reopen the finding or create a new corrective action.

The original gap assessment remains the baseline snapshot and is not retroactively rewritten. This workpaper documents a later simulated remediation and validation event.

## Related Artifacts

- [Original MFA control-testing workpaper](08-mfa-control-testing-workpaper.md)
- [Risk treatment plan](03-risk-treatment-plan.md)
- [Readiness gap assessment](02-gap-assessment.md)
- [MFA cross-framework mapping](09-mfa-cross-framework-crosswalk.md)
- [MFA risk traceability case study](../case-studies/mfa-risk-traceability.md)
