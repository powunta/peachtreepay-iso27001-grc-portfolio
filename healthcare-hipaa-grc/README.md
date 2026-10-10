# Peachtree Health Clinic — HIPAA Security Risk Assessment
> **SIMULATED EDUCATIONAL CASE STUDY.** Peachtree Health is fictional. All accounts, events, findings, vendors and risk assessments are invented. No actual patient information or PHI is included. This is not a HIPAA compliance certification or a client engagement.

**Analyst:** Phil Owunta | **Version:** October 2026

## Scenario and executive summary
Peachtree Health is a simulated 75-person outpatient clinic using a cloud electronic health record (EHR), patient portal, billing/scheduling tools, managed endpoints and third-party IT support. This project evaluates risk to electronic protected health information (ePHI), clinical continuity and third-party access. The exercise identifies **12 risks: 3 Critical, 8 High, 1 Moderate** before treatment.

In a **synthetic 24-account EHR termination review**, four access-disablement exceptions violate the clinic's *fictional internal 24-hour target*; the test does not indicate actual improper EHR access or a real breach. Recommendations prioritize offboarding, MFA, recovery testing, cloud EHR vendor controls and ongoing evidence review.

## Project deliverables
1. [Scope and ePHI data flow](01-scope/scenario-and-data-flow.md)
2. [Asset inventory](assets/asset-inventory.csv)
3. [Risk methodology](02-risk-assessment/methodology.md) and [12-risk register](02-risk-assessment/risk-register.csv)
4. [HIPAA sampled safeguard assessment](03-compliance/hipaa-gap-assessment.md)
5. [EHR offboarding control test](04-control-testing/termination-access-test.md) and [24-account synthetic population](04-control-testing/termination-access-population.csv)
6. [Cloud EHR vendor risk review](05-vendor-risk/ehr-vendor-review.md)
7. [90-day remediation plan](06-remediation/90-day-roadmap.csv)
8. [Management risk brief](07-executive/board-risk-brief.md)
9. [Interview walkthrough](08-interview/interview-playbook.md)

## Regulatory precision
This work samples obligations under the HIPAA Security Rule, 45 CFR §§164.306–164.316, using HHS OCR risk-analysis guidance and NIST SP 800-66 Rev. 2. A sampled safeguard assessment is **not** a comprehensive compliance audit. "Addressable" implementation specifications are not automatically optional. The December 2024 HHS Security Rule proposal is not treated as a final, operative requirement; check rulemaking status before presenting.

Resources: [HHS OCR risk analysis](https://www.hhs.gov/hipaa/for-professionals/security/guidance/guidance-risk-analysis/index.html) · [NIST SP 800-66 Rev. 2](https://csrc.nist.gov/pubs/sp/800/66/r2/final) · [Current regulatory text](https://www.ecfr.gov/current/title-45/subtitle-A/subchapter-C/part-164/subpart-C).

## Relationship to existing portfolio
This healthcare case study is separate from, and complements, the existing PeachtreePay fintech ISO 27001 GRC and vendor-risk work. All existing PeachtreePay materials remain part of this repository. Do not present simulated projects as paid employment or clinical consulting.
