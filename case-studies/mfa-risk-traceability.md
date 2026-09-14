# Critical MFA Risk: End-to-End Traceability Case Study

> **Simulated portfolio case study — not a real client engagement or certification audit.**  
> This page demonstrates how one PeachtreePay risk flows through assessment, treatment, control selection, evidence planning, validation, and residual-risk review.

## Executive Summary

PeachtreePay's highest-rated simulated risk is employee account compromise caused by inconsistent multi-factor authentication (MFA). At the time of the readiness assessment, MFA was enabled for administrators only, leaving regular user accounts without consistent protection.

Because credential attacks are common and a compromised account could expose sensitive information or enable further access, the risk received an inherent likelihood of 4/5 and impact of 5/5, producing a Critical inherent score of 20. The selected treatment is to mitigate the risk by requiring MFA on critical systems within 30 days.

## End-to-End Traceability

| Traceability field | PeachtreePay decision |
|---|---|
| Risk statement | Employee account compromised because MFA is not enabled everywhere |
| Business context | PeachtreePay relies on Microsoft 365, AWS, employee endpoints, customer data, and cloud-based services |
| Threat scenario | Credential theft, phishing, password reuse, or brute-force activity leads to account takeover |
| Control weakness | MFA is enabled for administrators only; regular users are not consistently protected |
| Potential business impact | Unauthorized access, sensitive-information exposure, service disruption, fraud, or further access into connected systems |
| Inherent likelihood | 4/5 |
| Inherent impact | 5/5 |
| Inherent risk score | 20 — Critical |
| Treatment decision | Mitigate |
| Risk owner | IT/Security |
| Primary treatment action | Require MFA on critical systems and expand MFA company-wide |
| Target timeframe | First 30 days of the remediation roadmap |
| Primary ISO/IEC 27001:2022 control alignment | Annex A 8.5 — Secure authentication |
| Supporting control themes | Access control, identity management, authentication information, security monitoring, and phishing awareness |
| Primary expected evidence | Microsoft 365/AWS MFA configuration report demonstrating that MFA is enabled for required accounts |
| Validation status | Not yet tested — treatment is planned and the gap remains Not Implemented in the simulated assessment |
| Estimated residual risk | 10, conditional on successful implementation and validation |
| Current remediation status | Planned / Not Implemented |

## Risk-to-Control Decision Trail

1. **Identify the risk:** Inconsistent MFA creates an account-compromise scenario.
2. **Assess inherent risk:** Likelihood 4 × impact 5 = 20, making it the portfolio's only Critical inherent risk.
3. **Select treatment:** Mitigate because the risk can be reduced through stronger authentication and supporting controls.
4. **Assign accountability:** IT/Security owns remediation and follow-through.
5. **Set priority:** Place MFA on critical systems in the first 30 days because it addresses the highest-rated risk.
6. **Define evidence:** Obtain configuration reports showing which Microsoft 365 and AWS accounts are protected.
7. **Validate operation:** Compare the in-scope account population with enforced-MFA results, investigate exceptions, and retain dated test documentation.
8. **Reassess risk:** Confirm whether the evidence supports the estimated residual score of 10; revise the score if testing shows gaps.

## Control Implementation and Evidence Plan

| Activity | Expected output | Validation approach | Status |
|---|---|---|---|
| Identify in-scope Microsoft 365 and AWS accounts | Current account population | Reconcile user and privileged-account lists with system inventories | Planned |
| Enforce MFA for required accounts | MFA configuration settings | Review tenant and cloud-console configuration | Planned |
| Document approved exceptions | Exception log with owner and expiration date | Confirm each exception has business justification and approval | Planned |
| Generate implementation evidence | Microsoft 365/AWS MFA configuration report | Verify the report is dated, attributable, and covers the required population | Planned |
| Test control operation | MFA coverage test results | Sample administrator and regular-user accounts and confirm enforcement | Not tested |
| Review residual risk | Approved residual-risk record | Risk owner reviews test results and accepts or requests further treatment | Pending |

## Evidence Quality Criteria

Evidence should be:

- **Relevant:** It directly demonstrates MFA coverage for the systems and accounts in scope.
- **Complete:** It includes regular users, administrators, service accounts, and documented exceptions where applicable.
- **Current:** It is dated and represents the configuration during the review period.
- **Reliable:** It comes from authoritative Microsoft 365 or AWS administrative reporting.
- **Traceable:** It can be linked to the risk, treatment action, control, owner, and validation result.

A configuration report alone shows how the control is configured at a point in time. A stronger evidence package would also include the in-scope account population, approved exceptions, an implementation/change record, and documented validation results.

## Residual-Risk Interpretation

The residual score of 10 is an **estimate**, not a proven outcome. It assumes MFA is successfully enforced for required accounts and that testing confirms the control is operating as intended. If regular-user coverage is incomplete, exceptions are unmanaged, or evidence cannot be produced, the risk should remain open and the residual score should be reconsidered.

## Management Recommendation

Prioritize company-wide MFA because it reduces the likelihood of the portfolio's highest-rated account-compromise risk. IT/Security should report completion, exceptions, evidence quality, test results, and remaining exposure to management before residual risk is formally accepted.

## How I Would Explain This in an Interview

> I started with the business risk rather than selecting a control first. PeachtreePay had MFA for administrators but not consistently for regular users, creating a critical account-compromise risk scored at 20. I selected mitigation, assigned IT/Security as the owner, placed company-wide MFA in the first 30 days, and defined Microsoft 365 and AWS configuration reports as primary evidence. I would validate that evidence against the full in-scope account population before confirming the estimated residual score of 10.

## Interview Questions This Case Study Supports

**Why did you prioritize MFA?**  
It addressed the only Critical inherent risk, reduced the likelihood of account takeover, and could be implemented early in the remediation roadmap.

**Why is the residual score only an estimate?**  
Residual risk should be confirmed after treatment is implemented and evidence shows the control operates effectively. The project does not claim that simulated remediation has already occurred.

**How would you test the control?**  
I would reconcile the in-scope account list against Microsoft 365 and AWS MFA reports, sample administrator and regular-user accounts, review exceptions, and document the test date, reviewer, results, and follow-up actions.

**What would happen if testing failed?**  
I would keep the risk open, document the deficiency, assign corrective action, update the target date, and reassess the residual-risk estimate after remediation.
