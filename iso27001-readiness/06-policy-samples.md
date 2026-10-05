# Policy Samples

These concise policy samples demonstrate the difference between governance requirements and operating procedures. PeachtreePay is fictional, so the statements below are portfolio examples rather than approved corporate policy.

## Information Security Policy

**Purpose:** Establish PeachtreePay's overall expectations for protecting company, customer, and employee information.

- Protect the confidentiality, integrity, and availability of information.
- Apply security responsibilities across management, IT, Security/GRC, and employees.
- Use risk management to identify, assess, treat, and monitor information-security risk.
- Apply least privilege, MFA for critical systems, periodic access reviews, and prompt access removal.
- Provide security awareness training and maintain vulnerability, incident, vendor, backup, and continuity practices.
- Review this policy at least annually or after significant organizational or technology change.

## Access Control Policy

- Access must be based on business need and least privilege.
- New accounts require appropriate approval before provisioning.
- MFA is required for Microsoft 365, AWS, administrative access, remote access, and sensitive applications.
- Critical-system access is reviewed quarterly.
- Role changes trigger an access review and removal of no-longer-needed permissions.
- Termination triggers prompt account disablement, session revocation, privileged-access removal, and equipment recovery.
- Third-party access must have a documented purpose, approval, limited scope, and end date or removal process.

## Incident Response Policy

PeachtreePay uses a consistent incident-response lifecycle:

1. **Identification:** Determine whether suspicious activity is a security incident.
2. **Investigation:** Determine what happened, when it happened, which systems were affected, and what information may be involved.
3. **Containment:** Stop additional harm, such as disabling a compromised account or isolating a device.
4. **Eradication:** Remove the cause, such as malware, vulnerable configuration, or compromised credentials.
5. **Recovery:** Restore systems safely and monitor for recurrence.
6. **Lessons learned:** Document root cause, control failures, response effectiveness, and remediation.

Significant incidents should be documented, evidence should be preserved where appropriate, and the response process should be periodically tested through tabletop exercises.

## Policy versus procedure

A policy states **what** the organization requires. A procedure explains **how** people perform and document the requirement.

For example, the Access Control Policy requires prompt access removal after termination. An offboarding procedure would define the HR notification, IT ticket, account-disablement steps, evidence captured, escalation path, and closure approval.

## Related artifacts

- [Evidence register](05-evidence-register.md)
- [Gap assessment](02-gap-assessment.md)
- [90-day remediation roadmap](07-remediation-roadmap.md)
