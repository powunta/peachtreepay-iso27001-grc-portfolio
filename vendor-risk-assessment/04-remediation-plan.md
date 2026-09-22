# Vendor Remediation Plan

| ID | Finding | Required Action | Owner | Priority | Target | Validation Evidence |
|---|---|---|---|---|---|---|
| REM-01 | MFA not enforced for all privileged workflows | Enforce MFA or approved compensating control across all privileged administration | CloudBridge Security | Critical | Before production | Configuration evidence + test |
| REM-02 | No fixed breach-notification commitment | Add contractual notification timeline for confirmed incidents affecting PeachtreePay data | Procurement / Legal | High | Before contract signature | Executed contract language |
| REM-03 | DR exercise evidence incomplete | Complete recovery exercise and provide results against RTO/RPO | CloudBridge BC/DR | High | 60 days | Test report |
| REM-04 | Default data retention too broad | Define PeachtreePay-specific retention and deletion procedure | Privacy / Vendor Owner | High | Before production data load | Retention configuration + procedure |
| REM-05 | Privileged deprovisioning target is 24 hours | Reduce privileged-access removal target and require immediate action for high-risk terminations | CloudBridge IAM | High | 30 days | Updated procedure + sample evidence |
| REM-06 | Two medium pen-test items remain open | Track remediation to closure or approved risk acceptance | CloudBridge Security | Moderate | 60 days | Closure evidence |
| REM-07 | Vendor outage could disrupt support | Document PeachtreePay contingency process for CRM unavailability | PeachtreePay Customer Ops | Moderate | 45 days | Continuity procedure |

## Approval Gates

### Must be completed before production onboarding
- REM-01: Privileged MFA
- REM-02: Breach-notification clause
- REM-04: Retention/deletion requirements

### May remain open under tracked remediation
- REM-03: DR exercise evidence
- REM-05: Privileged deprovisioning improvement
- REM-06: Medium pen-test findings
- REM-07: PeachtreePay contingency procedure

## Escalation Rule

If a critical or high finding cannot be remediated by the target date, the issue must be escalated to the PeachtreePay risk owner for documented acceptance, additional compensating controls, delayed onboarding, or rejection of the vendor.
