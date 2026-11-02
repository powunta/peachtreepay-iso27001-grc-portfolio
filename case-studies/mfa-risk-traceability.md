# Critical MFA Risk: End-to-End Traceability Case Study

> **Simulated portfolio case study — not a real client engagement or certification audit.**  
> This page demonstrates how one PeachtreePay risk flows from assessment through corrective action, retesting, finding closure, and residual-risk review.

## Executive Summary

PeachtreePay's highest-rated simulated risk is employee account compromise caused by inconsistent multi-factor authentication (MFA). The baseline readiness assessment found MFA enabled for administrators but not consistently enforced for regular users.

The risk received an inherent likelihood of 4/5 and impact of 5/5, producing a Critical score of 20. PeachtreePay selected mitigation through company-wide MFA. Initial testing over 108 human accounts found two unsupported exceptions and one approved temporary exception, so the control failed its 100% criterion and the proposed residual-risk score was withheld.

After simulated corrective action, a complete-population retest confirmed MFA enforcement for 108 of 108 accounts, no active exceptions, and preventive workflow improvements. The finding was closed, and the evidence supported a residual score of 10 (Medium) with continued quarterly monitoring.

## End-to-End Traceability

| Traceability field | PeachtreePay decision |
|---|---|
| Risk statement | Employee account compromised because MFA is not enabled everywhere |
| Business context | PeachtreePay relies on Microsoft 365, AWS, employee endpoints, customer data, and cloud services |
| Threat scenario | Credential theft, phishing, password reuse, or brute-force activity leads to account takeover |
| Baseline control weakness | MFA was enabled for administrators only; regular users were not consistently protected |
| Potential business impact | Unauthorized access, information exposure, service disruption, fraud, or lateral movement |
| Inherent likelihood and impact | 4 × 5 |
| Inherent score | 20 — Critical |
| Treatment decision and owner | Mitigate — IT/Security |
| ISO/IEC 27001:2022 alignment | Annex A 8.5 — Secure authentication |
| Primary evidence | Account population, Microsoft 365 and AWS reports, exception register, change tickets, provisioning checklist |
| Initial test result | Exception — 105 of 108 enforced, one approved exception, and two unsupported exceptions |
| Corrective action | Enforce MFA, remove a legacy exclusion, require ticketed AWS account creation, and close the temporary exception |
| Retest result | Pass — 108 of 108 enforced, no active exceptions |
| Finding status | Closed — Remediated and Retested |
| Residual-risk decision | 2 × 5 = 10 — Medium; accept with continued monitoring |
| Ongoing assurance | Quarterly population reconciliation, exception review, and provisioning-workflow testing |

## Assurance Timeline

1. **Identify and score the risk:** Inconsistent MFA produces a Critical inherent score of 20.
2. **Select treatment:** Require MFA across Microsoft 365 and AWS human accounts.
3. **Define evidence:** Establish the population and obtain authoritative enforcement and exception reports.
4. **Perform initial testing:** Test all 108 accounts and identify two unsupported exceptions.
5. **Withhold residual-risk acceptance:** Keep the risk open because the evidence does not meet the control criterion.
6. **Analyze root causes:** Identify a legacy policy exclusion and an AWS account created outside the approved workflow.
7. **Validate corrective action:** Inspect tickets, refreshed reports, the exception register, and the revised provisioning checklist.
8. **Retest the complete population:** Confirm 108 of 108 accounts have MFA enforced and no active exceptions remain.
9. **Close the finding:** Mark it Closed — Remediated and Retested.
10. **Reassess residual risk:** Support the planned score of 10 and require quarterly monitoring.

## Evidence and Decision Trail

| Phase | Evidence or activity | Result |
|---|---|---|
| Baseline | Gap assessment and risk register | MFA weakness identified; inherent risk 20 |
| Treatment | Risk treatment plan and 30-day roadmap | Company-wide MFA prioritized |
| Initial validation | 108-account population, system reports, and exception register | Control failed; two unsupported exceptions |
| Root-cause review | Policy-exclusion and AWS provisioning analysis | Workflow weaknesses identified |
| Corrective action | Remediation tickets and revised provisioning checklist | Exceptions corrected and preventive steps added |
| Retest | Refreshed complete population and 15-account reperformance | 108/108 enforced; no active exceptions |
| Management decision | Retest conclusion and risk-owner review | Finding closed; residual risk 10 accepted with monitoring |

## Residual-Risk Interpretation

The residual score of 10 is supported only within this simulated, point-in-time exercise. MFA reduces the likelihood of account compromise from 4 to 2, but impact remains 5 because a successful compromise could still cause severe harm. Continued monitoring is necessary because new accounts, policy exclusions, authentication-method changes, and temporary exceptions can reintroduce exposure.

## Management Recommendation

Maintain quarterly population reconciliation and exception review. Require ticketed approval for new AWS human users, monitor policy exclusions, and reopen the finding if an unsupported exception appears.

## How I Would Explain This in an Interview

> I started with the business risk rather than selecting a control first. Initial testing of all 108 Microsoft 365 and AWS human accounts found two unsupported MFA exceptions, so I did not accept the proposed residual-risk score. I documented the root causes, reviewed corrective-action evidence, retested the complete population, and confirmed 108 of 108 accounts had MFA enforced with no active exceptions. That supported closing the finding and accepting a Medium residual risk with quarterly monitoring.

## Related Artifacts

- [Initial MFA control-testing workpaper](../iso27001-readiness/08-mfa-control-testing-workpaper.md)
- [MFA corrective-action validation and retest](../iso27001-readiness/11-mfa-corrective-action-retest.md)
- [Risk treatment plan](../iso27001-readiness/03-risk-treatment-plan.md)
- [Evidence register](../iso27001-readiness/05-evidence-register.md)
- [MFA cross-framework mapping](../iso27001-readiness/09-mfa-cross-framework-crosswalk.md)
