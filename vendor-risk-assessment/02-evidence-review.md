# Evidence Review

The questionnaire alone is not sufficient to validate vendor controls. This review records the supporting evidence requested and the analyst conclusion for each item.

| Evidence | Status | Analyst Review |
|---|---|---|
| SOC 2 Type II report | Reviewed - simulated | Strong general control environment; noted carve-outs and user-entity responsibilities |
| Penetration-test executive summary | Reviewed - simulated | No open critical findings; two medium findings under remediation |
| Information Security Policy | Reviewed - simulated | Current, approved, and assigned to an accountable security leader |
| Incident Response Plan | Reviewed - simulated | Roles and escalation defined; customer-notification commitment remains vague |
| Business Continuity Plan | Reviewed - simulated | Documented, but recovery testing evidence is incomplete |
| Disaster Recovery Test Results | Insufficient | Tabletop evidence only; no full recovery exercise results provided |
| Encryption Architecture Summary | Reviewed - simulated | Supports encryption in transit and at rest |
| Subprocessor List | Reviewed - simulated | Major subprocessors identified with service purpose |
| Cyber Insurance Certificate | Reviewed - simulated | Coverage exists; limits would require procurement/legal validation |
| Data Retention Schedule | Reviewed - simulated | Default 7-year retention exceeds PeachtreePay's preferred minimum-necessary approach |
| Privileged Access Standard | Partially sufficient | MFA requirement does not cover all legacy admin workflows |
| Account Termination Procedure | Reviewed - simulated | 24-hour disablement target exists but is weaker than PeachtreePay's preferred privileged-access requirement |

## Evidence-Based Conclusions

### Stronger Areas
- Independent assurance through SOC 2 Type II
- Encryption at rest and in transit
- Vulnerability scanning and annual penetration testing
- Centralized logging and security monitoring
- Documented governance and incident-response processes

### Material Gaps
- Mandatory MFA is not universal for privileged administration
- Contractual incident notification is not time-bound
- Disaster-recovery testing evidence is incomplete
- Data-retention defaults are broader than PeachtreePay prefers
- Privileged-account disablement may take up to 24 hours

## Analyst Principle

A vendor's written answer is treated as a claim until supported by appropriate evidence. Evidence quality, recency, scope, and applicability are considered before a control is treated as effective.
