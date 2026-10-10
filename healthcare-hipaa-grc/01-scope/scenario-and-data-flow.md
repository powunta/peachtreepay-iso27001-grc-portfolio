# Scenario, scope and ePHI workflow
**Fictional organization:** Peachtree Health Clinic, 75 staff, outpatient operations. In scope: staff identity lifecycle, cloud EHR, patient portal, scheduling/billing, user laptops/tablets, secure messaging, backup/recovery, vendor support and third-party processing. Exclusions: clinical efficacy and actual provider compliance conclusions.

## Synthetic ePHI data flow
Patient → portal/intake → cloud EHR → clinicians → billing/scheduling → external approved business associates. Workforce identities flow from HR termination and hiring events → IT/identity provider → EHR permissions. EHR support vendors use privileged remote access; access must be risk-assessed and logged.

## Key business impacts
- Unauthorized record access or disclosure
- Care delays or unsafe clinical operations if EHR is unavailable
- Privacy or regulatory exposure from inadequately governed vendors
- Operational costs of ransomware and prolonged outages

**Evidence limitation:** No production logs, clinical systems, real patients or vendor documents were inspected. All findings are hypotheses embedded in the case study.
