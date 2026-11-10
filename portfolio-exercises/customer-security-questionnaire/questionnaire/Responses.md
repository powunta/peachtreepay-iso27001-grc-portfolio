# Harbor Analytics — Simulated Customer Security Questionnaire

All entries are **illustrative draft answers, not approved external responses**. The status “Met” means the fictional scenario describes the control; it does not mean a real control has been tested. All evidence IDs refer only to the fictional evidence index.

| # | Domain | Question | Illustrative draft response | Evidence | Owner | Scenario status |
|---|---|---|---|---|---|---|
| 1 | Governance | Is there a written, annually reviewed security policy approved by management? | Yes. The Information Security Policy is approved by the CISO and executive team and reviewed annually; last review March 2026. | EV-001 | Security | Met |
| 2 | Risk | Are annual enterprise risk assessments performed and tracked? | Yes. An annual enterprise assessment is performed and the risk register is reviewed quarterly. | EV-002 | Security/GRC | Met |
| 3 | Assurance | Do independent assurance assessments occur? | Yes. The scenario describes an annual SOC 2 Type II report (Security, Availability, Confidentiality) and an ISO/IEC 27001:2022 certificate. | EV-003, EV-004 | GRC | Met |
| 4 | Access | Is MFA required for workforce production and admin access? | Yes. Workforce SSO enforces MFA for production/admin access. Customer MFA via SAML SSO remains the customer's responsibility. | EV-005, EV-006 | IT/Security | Met |
| 5 | Access | How frequently is access reviewed? | Privileged access quarterly; standard access every six months; exceptions tracked to closure. | EV-007 | IT | Met |
| 6 | Encryption | Is data encrypted, and are customer-managed keys offered? | At rest AES-256 and in transit TLS 1.2+. Customer-managed keys are **not offered**; no future delivery date is promised. | EV-008, EV-009 | Security/Product | **Escalate** |
| 7 | Monitoring | Are security logs collected and monitored 24x7? | Logs are centralized with 12-month retention; the staffing/on-call coverage model is **unverified**. Do not claim 24x7 monitoring. | EV-010, EV-011 | Security Ops | **Validate with SME** |
| 8 | Vulnerability | Are scans, remediation SLAs and independent tests used? | Recurring infrastructure/application scans; critical issues within 7 days and high within 30; annual independent penetration test. | EV-012, EV-013 | Security | Met |
| 9 | SDLC | Are code review, dependency scans and SAST integrated? | Peer review is required and static/dependency scans run in CI before release. | EV-014, EV-015 | Engineering | Met |
| 10 | Incident | Is IR documented and tested, and when are customers notified? | Annual tabletop test; fictional contractual notice standard is 72 hours. **Legal must separately confirm applicable regulatory duties and exact notification triggers.** | EV-016, EV-017 | Security/Legal | Met (Legal wording review) |
| 11 | Resilience | What are the RTO/RPO and DR testing frequencies? | Production RTO 4 hours, RPO 1 hour, with documented annual DR tests. | EV-018 | Infrastructure | Met |
| 12 | Third parties | Are vendors/subprocessors assessed and monitored? | Intake, due diligence, risk tiering and tier-based reassessment; maintained subprocessor list and change notices. | EV-019, EV-020 | GRC/Procurement | Met |
| 13 | Privacy | Can you support GDPR access/deletion requests? | Requests are logged and tracked to statutory deadlines; customer-facing language requires Privacy/Legal validation. | EV-021, EV-022 | Privacy/Legal | **Validate with SME** |
| 14 | Data lifecycle | What happens to data after termination? | Production deletion within 30 days, backup expiration within 90 days; optional confirmation. | EV-023 | Engineering/Privacy | Met |
| 15 | Residency | Can customers select data-hosting region? | US or EU hosting selected at provisioning. | EV-024 | Product | Met |
| 16 | Workforce | Are screening and security training performed? | Permitted background checks; security awareness at hire and annually, completion tracked. | EV-025, EV-026 | HR/Security | Met |
| 17 | AI governance | Is customer data used for AI model training, and how is AI managed? | Customer data is not used to train models. AI use policy exists, but formal AI risk assessment process remains incomplete. | EV-027 | Legal/Security | **Escalate** |
| 18 | Shared responsibility | Who secures platform versus customer configurations? | Harbor secures platform/infrastructure/operations; customer manages users, roles, SSO/MFA configurations and uploaded data. | EV-028 | Security/Customer Success | Met |

## Summary
14 Met; 2 Validate with SME; 2 Escalate. **0 responses approved for external use.** The evidence register contains hypothetical references only.

See [methodology](../methodology/Review_and_Escalation_Process.md) for the required review gates.