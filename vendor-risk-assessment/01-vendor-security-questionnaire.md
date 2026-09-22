# Vendor Security Questionnaire

**Vendor:** CloudBridge CRM  
**Business owner:** PeachtreePay Customer Operations  
**Service:** Cloud-based CRM platform  
**Data classification:** Confidential  
**Business criticality:** High  
**Assessment type:** Pre-onboarding third-party security review

## Questionnaire

| # | Domain | Question | Vendor Response | Analyst Assessment |
|---|---|---|---|---|
| 1 | Governance | Do you maintain a documented information security program? | Yes | Satisfactory |
| 2 | Assurance | Do you maintain an independent security certification or attestation? | SOC 2 Type II available | Satisfactory, evidence required |
| 3 | IAM | Is MFA enforced for privileged administrator accounts? | Optional for some legacy admin workflows | Gap |
| 4 | IAM | Are user accounts reviewed periodically? | Quarterly | Satisfactory |
| 5 | Encryption | Is customer data encrypted in transit? | TLS 1.2+ | Satisfactory |
| 6 | Encryption | Is customer data encrypted at rest? | AES-256 | Satisfactory |
| 7 | Vulnerability Mgmt | Are external vulnerability scans performed regularly? | Monthly | Satisfactory |
| 8 | Testing | Is independent penetration testing performed? | Annually | Satisfactory, summary requested |
| 9 | Incident Response | Do you maintain a documented incident-response plan? | Yes | Satisfactory |
| 10 | Incident Response | What is the contractual customer-notification timeline for a confirmed breach? | No fixed timeline in standard contract | Gap |
| 11 | Logging | Are privileged administrative actions logged? | Yes | Satisfactory |
| 12 | Monitoring | Are security logs centrally monitored? | Yes, 24/7 SOC | Satisfactory |
| 13 | Backups | Are production backups performed? | Daily | Satisfactory |
| 14 | Recovery | Is disaster-recovery testing performed at least annually? | Partial tabletop only | Gap |
| 15 | Data Retention | Can customers define retention and deletion requirements? | Standard retention is 7 years; custom deletion requires support request | Gap |
| 16 | Privacy | Is customer data sold for advertising purposes? | No | Satisfactory |
| 17 | Subprocessors | Is a list of subprocessors maintained? | Yes | Satisfactory |
| 18 | Subprocessors | Are customers notified before material subprocessor changes? | 30-day notice | Satisfactory |
| 19 | Secure Development | Are code changes reviewed before production deployment? | Yes | Satisfactory |
| 20 | Access Control | Is production access limited using least privilege? | Yes | Satisfactory |
| 21 | HR Security | Are personnel with production access subject to background checks where legally permitted? | Yes | Satisfactory |
| 22 | Termination | Are departing-worker accounts disabled promptly? | Within 24 hours | Moderate concern; tighter SLA preferred for privileged access |
| 23 | Data Location | Can customer data residency be identified? | Yes, U.S. region available | Satisfactory |
| 24 | Business Continuity | Is there a documented business continuity plan? | Yes | Satisfactory |
| 25 | Cyber Insurance | Do you maintain cyber liability insurance? | Yes | Satisfactory, certificate requested |

## Analyst Follow-Up Questions

1. What controls compensate for the lack of mandatory MFA in legacy administrative workflows?
2. Can CloudBridge commit contractually to breach notification within 24 hours of confirmed impact to PeachtreePay data?
3. Can CloudBridge provide evidence of a completed disaster-recovery exercise with measured recovery results?
4. Can PeachtreePay configure shorter retention or verified deletion for customer data?
5. Can privileged-access termination be reduced from 24 hours to 4 hours or less?
