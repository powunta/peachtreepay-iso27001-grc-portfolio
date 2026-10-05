# MFA Control-Testing Workpaper

> **Simulated evidence and testing exercise - not a real client engagement or production-system review.**  
> The account records, evidence extracts, exceptions, and test results below were created for portfolio purposes.

## Test Overview

| Field | Detail |
|---|---|
| Risk | Risk 1 - Employee account compromised because MFA is not enabled everywhere |
| Control owner | IT/Security |
| Control objective | Require MFA for all in-scope human accounts accessing Microsoft 365 and AWS |
| Control frequency | Continuous enforcement; quarterly access-control review |
| Test type | Point-in-time design and operating-effectiveness test |
| Simulated test date | September 30, 2026 |
| Tester | GRC Analyst |
| Expected result | 100% of required accounts have MFA enforced; any exception is approved, documented, time-bound, and monitored |
| Framework alignment | ISO/IEC 27001:2022 Annex A 8.5; NIST CSF 2.0 PR.AA-03; SOC 2 CC6.1 alignment theme |

## Simulated Evidence Inventory

| Evidence ID | Simulated artifact | Purpose | Quality review |
|---|---|---|---|
| E-MFA-01 | In-scope account population export | Establishes the complete population of human accounts | Dated, system-generated, and reconciled to HR and administrator inventories |
| E-MFA-02 | Microsoft 365 MFA registration and enforcement report | Shows MFA status for Microsoft 365 accounts | Dated and attributable to the tenant; includes standard and privileged users |
| E-MFA-03 | AWS IAM credential report | Shows authentication status for AWS human users | System-generated and current for the test date |
| E-MFA-04 | MFA exception register | Documents business justification, approval, owner, and expiration | One approved exception recorded; unsupported exceptions are absent |
| E-MFA-05 | Change ticket for company-wide MFA rollout | Shows implementation approval and deployment activity | Approved by IT/Security and linked to the treatment plan |

## Population-Level Evidence Extract

The simulated population contains 108 human accounts. Some employees have accounts in both Microsoft 365 and AWS.

| System and account type | Population | MFA enforced | Approved exception | Unsupported exception | Result |
|---|---:|---:|---:|---:|---|
| Microsoft 365 standard users | 94 | 92 | 1 | 1 | Exception |
| Microsoft 365 privileged users | 6 | 6 | 0 | 0 | Pass |
| AWS IAM human users | 8 | 7 | 0 | 1 | Exception |
| **Total** | **108** | **105** | **1** | **2** | **Exception** |

**Observed enforcement coverage:** 105 of 108 accounts, or **97.2%**.

The approved exception does not satisfy the normal control requirement, but it is documented and time-bound. The two unsupported exceptions lack evidence of approval and therefore represent control failures.

## Testing Procedures and Results

| Step | Test procedure | Result | Workpaper conclusion |
|---:|---|---|---|
| 1 | Reconcile E-MFA-01 to the Microsoft 365 and AWS account populations | Pass | All 108 human accounts were included in the test population |
| 2 | Compare each in-scope account with MFA-enforcement status in E-MFA-02 and E-MFA-03 | Exception | Three accounts did not have MFA enforced |
| 3 | Review E-MFA-04 for approval, justification, owner, and expiration | Exception | One account had an approved temporary exception; two lacked approval |
| 4 | Select 12 accounts across standard, privileged, and AWS access and inspect enforcement | Exception | 11 passed; one unsupported AWS exception failed |
| 5 | Inspect E-MFA-05 for authorized implementation activity | Pass | The rollout change was approved and traceable to the treatment plan |
| 6 | Evaluate whether the evidence supports the estimated residual-risk score of 10 | Not supported | Coverage gaps remain; the residual-risk estimate should not yet be accepted |

## Exception Details

| Exception ID | Observation | Risk | Required remediation | Owner | Target |
|---|---|---|---|---|---|
| MFA-EX-01 | One Microsoft 365 standard-user account lacked MFA and had no approved exception | Credential compromise and unauthorized access | Enforce MFA, investigate why the account bypassed deployment, and confirm through retesting | IT Operations | 7 days |
| MFA-EX-02 | One AWS human-user account lacked MFA and had no approved exception | Elevated cloud-account compromise risk | Enforce MFA or disable the account; review AWS account-creation procedures | Cloud/Security | 7 days |
| MFA-EX-03 | One temporary Microsoft 365 exception was approved but expires in 14 days | Exposure remains during the exception period | Monitor use, apply compensating controls, and close or renew through formal approval | IT/Security | 14 days |

## Test Conclusion

**Overall result: Exception - control is not operating effectively across the full required population.**

The control is appropriately designed around company-wide MFA, and privileged Microsoft 365 coverage tested successfully. However, two unsupported exceptions prevent the control from meeting its 100% enforcement criterion. The planned residual-risk score of 10 remains an estimate and should not be formally accepted until remediation and retesting are complete.

## Remediation and Retest Plan

1. Enforce MFA or disable the two unsupported accounts within seven days.
2. Confirm the approved temporary exception has compensating controls, an accountable owner, and a valid expiration.
3. Determine why the unsupported accounts were excluded and correct the provisioning or deployment workflow.
4. Regenerate Microsoft 365 and AWS reports after remediation.
5. Retest the complete population and document closure evidence.
6. Reassess residual risk and obtain risk-owner approval.

## Auditor-Oriented Takeaway

This workpaper distinguishes four separate conclusions:

- A policy or planned control establishes the requirement.
- Configuration reports show the control state.
- Population reconciliation and sampling test whether the evidence is complete and reliable.
- Residual risk should be accepted only after exceptions are remediated or formally approved.

## Related Artifacts

- [MFA risk traceability case study](../case-studies/mfa-risk-traceability.md)
- [MFA cross-framework mapping](09-mfa-cross-framework-crosswalk.md)
- [Evidence register](05-evidence-register.md)
- [Risk treatment plan](03-risk-treatment-plan.md)
