# Information-Security Risk Register

This simulated register assesses 15 PeachtreePay information-security risks using the portfolio's 5 × 5 likelihood-and-impact method.

| ID | Risk | Area | Inherent L × I | Score | Rating | Treatment | Owner | Target | Residual L × I | Residual score | Residual rating |
|---:|---|---|---:|---:|---|---|---|---:|---:|---:|---|
| 1 | Employee account compromised because MFA is not enabled everywhere | Identity & Access | 4 × 5 | 20 | Critical | Mitigate | IT/Security | 30 days | 2 × 5 | 10 | Medium |
| 2 | Phishing attack steals employee credentials | Security Awareness | 4 × 4 | 16 | High | Mitigate | Security | 60 days | 2 × 4 | 8 | Medium |
| 3 | Former employee retains access after termination | Identity & Access | 3 × 5 | 15 | High | Mitigate | HR + IT | 30 days | 1 × 5 | 5 | Low |
| 4 | AWS misconfiguration exposes customer information | Cloud Security | 3 × 5 | 15 | High | Mitigate | Cloud/Security | 60 days | 1 × 5 | 5 | Low |
| 5 | Critical third-party vendor suffers a security breach | Third-Party Risk | 3 × 4 | 12 | High | Mitigate/Transfer | GRC/Legal | 90 days | 2 × 4 | 8 | Medium |
| 6 | Employee laptop is lost or stolen | Endpoint Security | 3 × 4 | 12 | High | Mitigate | IT | 60 days | 2 × 3 | 6 | Medium |
| 7 | Malware or ransomware disrupts business operations | Endpoint/Resilience | 3 × 5 | 15 | High | Mitigate | Security/IT | 60 days | 2 × 4 | 8 | Medium |
| 8 | Sensitive information is accidentally emailed to the wrong person | Data Protection | 3 × 4 | 12 | High | Mitigate | Security | 90 days | 2 × 3 | 6 | Medium |
| 9 | Excessive user permissions allow unauthorized access | Identity & Access | 3 × 5 | 15 | High | Mitigate | IT/GRC | 60 days | 1 × 5 | 5 | Low |
| 10 | Backups fail during a major incident | Resilience | 2 × 5 | 10 | Medium | Mitigate | IT | 60 days | 1 × 5 | 5 | Low |
| 11 | Vulnerable software remains unpatched | Vulnerability Management | 4 × 4 | 16 | High | Mitigate | IT/Security | 30 days | 2 × 4 | 8 | Medium |
| 12 | Employees are not adequately trained on security | Security Awareness | 4 × 3 | 12 | High | Mitigate | HR/Security | 90 days | 2 × 3 | 6 | Medium |
| 13 | Security logs are not reviewed and attacks go undetected | Monitoring | 3 × 4 | 12 | High | Mitigate | Security | 60 days | 2 × 3 | 6 | Medium |
| 14 | Weak vendor security assessment allows risky suppliers | Third-Party Risk | 3 × 4 | 12 | High | Mitigate | GRC | 90 days | 2 × 3 | 6 | Medium |
| 15 | Incident-response procedures are incomplete or untested | Incident Response | 3 × 5 | 15 | High | Mitigate | Security/GRC | 60 days | 1 × 5 | 5 | Low |

## Recommended Actions

| ID | Recommended action |
|---:|---|
| 1 | Require MFA for all users and critical systems |
| 2 | Implement phishing training, MFA, and email filtering |
| 3 | Establish a formal HR-to-IT offboarding workflow |
| 4 | Perform cloud-configuration reviews and establish a security baseline |
| 5 | Conduct vendor assessments and add security clauses and insurance requirements |
| 6 | Require encryption, MFA, screen lock, and remote wipe |
| 7 | Implement EDR, backups, patching, and response procedures |
| 8 | Provide data-handling training and technical safeguards |
| 9 | Enforce least privilege and quarterly access reviews |
| 10 | Automate backups and perform restoration testing |
| 11 | Establish formal patch and vulnerability-remediation SLAs |
| 12 | Require annual and new-hire security-awareness training |
| 13 | Centralize logging, alerts, and review procedures |
| 14 | Implement vendor questionnaires, risk tiering, and reassessment |
| 15 | Document and test the incident-response plan |

## Interpretation

Residual scores are estimates contingent on successful treatment implementation and validation. They should not be presented as tested outcomes while the related remediation remains planned.
