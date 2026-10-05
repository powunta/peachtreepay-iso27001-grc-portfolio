# Risk Treatment Plan

This plan converts the 15 assessed risks into accountable remediation work. It preserves the priorities, owners, target dates, residual-risk estimates, and status recorded in the source workbook.

> **Portfolio note:** PeachtreePay is a fictional fintech organization. The actions and residual scores below are simulated planning assumptions, not evidence that controls have been implemented.

| ID | Risk | Treatment | Recommended action | Owner | Priority | Target | Residual score | Status |
|---:|---|---|---|---|---|---:|---:|---|
| 1 | Employee account compromised because MFA is not enabled everywhere | Mitigate | Require MFA for all users and critical systems | IT/Security | Critical | 30 days | 10 | Planned |
| 2 | Phishing attack steals employee credentials | Mitigate | Phishing training, MFA, and email filtering | Security | High | 60 days | 8 | Planned |
| 3 | Former employee retains access after termination | Mitigate | Formal HR-to-IT offboarding workflow | HR + IT | High | 30 days | 5 | Planned |
| 4 | AWS misconfiguration exposes customer information | Mitigate | Cloud configuration reviews and security baseline | Cloud/Security | High | 60 days | 5 | Planned |
| 5 | Critical third-party vendor suffers a security breach | Mitigate/Transfer | Vendor assessments, security clauses, and insurance | GRC/Legal | High | 90 days | 8 | Planned |
| 6 | Employee laptop is lost or stolen | Mitigate | Encryption, MFA, screen lock, and remote wipe | IT | High | 60 days | 6 | Planned |
| 7 | Malware or ransomware disrupts business operations | Mitigate | EDR, backups, patching, and response procedures | Security/IT | High | 60 days | 8 | Planned |
| 8 | Sensitive information is accidentally emailed to the wrong person | Mitigate | Data handling training and technical safeguards | Security | Medium | 90 days | 6 | Planned |
| 9 | Excessive user permissions allow unauthorized access | Mitigate | Least privilege and quarterly access reviews | IT/GRC | High | 60 days | 5 | Planned |
| 10 | Backups fail during a major incident | Mitigate | Automated backups and restoration testing | IT | High | 60 days | 5 | Planned |
| 11 | Vulnerable software remains unpatched | Mitigate | Formal patch and vulnerability management SLAs | IT/Security | High | 30 days | 8 | Planned |
| 12 | Employees are not adequately trained on security | Mitigate | Annual and new-hire security awareness training | HR/Security | Medium | 90 days | 6 | Planned |
| 13 | Security logs are not reviewed and attacks go undetected | Mitigate | Centralized logging, alerts, and review procedures | Security | High | 60 days | 6 | Planned |
| 14 | Weak vendor security assessment allows risky suppliers | Mitigate | Vendor questionnaire, risk tiering, and reassessment | GRC | Medium | 90 days | 6 | Planned |
| 15 | Incident response procedures are incomplete or untested | Mitigate | Document and test incident response plan | Security/GRC | High | 60 days | 5 | Planned |

## Prioritization rationale

The first 30 days focus on MFA, offboarding, and vulnerability-remediation timelines because these actions address one Critical risk and several High risks while establishing repeatable control processes.

A lower residual score is an expected post-treatment result. Closure should require evidence review and control testing before the organization accepts that estimate.

## Related artifacts

- [Risk register](01-risk-register.md)
- [Evidence register](05-evidence-register.md)
- [90-day remediation roadmap](07-remediation-roadmap.md)
