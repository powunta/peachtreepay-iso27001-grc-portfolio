# PeachtreePay ISO/IEC 27001:2022 Readiness Assessment

> **Simulated portfolio project - not a real client engagement or certification audit.** PeachtreePay is a fictional 100-person Atlanta fintech company created for educational and job-portfolio purposes.

## Scenario

PeachtreePay operates a cloud-based payment platform using Microsoft 365, AWS, employee laptops, customer databases, internal applications, backup systems, and critical third-party services.

This project demonstrates how a junior GRC analyst can define an ISMS scope, identify information-security risk, evaluate control gaps, recommend treatments, map selected ISO/IEC 27001:2022 Annex A controls, define and test evidence, analyze control exceptions, and prioritize remediation.

## Browser-Readable Deliverables

1. [Information-Security Risk Register](01-risk-register.md)
2. [Readiness Gap Assessment](02-gap-assessment.md)
3. [Risk Treatment Plan](03-risk-treatment-plan.md)
4. [Statement of Applicability Sample](04-statement-of-applicability.md)
5. [Evidence Register](05-evidence-register.md)
6. [Policy Samples](06-policy-samples.md)
7. [90-Day Remediation Roadmap](07-remediation-roadmap.md)
8. [MFA Control-Testing Workpaper](08-mfa-control-testing-workpaper.md)
9. [MFA Cross-Framework Mapping](09-mfa-cross-framework-crosswalk.md)
10. [Accessible Executive Summary](10-executive-summary.md)
11. [Critical MFA Risk Traceability Case Study](../case-studies/mfa-risk-traceability.md)

The original [Excel workbook](../PeachtreePay_ISO27001_GRC_Portfolio.xlsx), [employer-facing portfolio PDF](../PeachtreePay_ISO27001_GRC_Portfolio.pdf), and [one-page executive summary PDF](../PeachtreePay_GRC_Executive_Summary.pdf) remain available for downloading and review.

## ISMS Scope

The simulated ISMS scope covers PeachtreePay employees, business processes, Microsoft 365, AWS infrastructure, customer information, employee endpoints, internal applications, backup processes, and critical third-party services supporting the payment platform.

## Key Assets

| Asset | Type | Why it matters |
|---|---|---|
| Customer database | Data | Contains customer and transaction-related information |
| AWS environment | Technology | Hosts the payment-processing application and supporting services |
| Microsoft 365 | SaaS | Provides email, identity, collaboration, and business documents |
| Employee laptops | Endpoint | Provide access to company systems and data |
| Source-code repository | Intellectual property | Contains application source code and configuration |
| HR records | Data | Contain employee personal and employment information |
| Backup systems | Technology | Support recovery after disruption or data loss |
| Third-party payment services | Vendor | Support payment and business operations |

## Risk Method

PeachtreePay uses a 5 x 5 qualitative model.

- Likelihood and impact are scored from 1 to 5.
- Inherent risk is assessed before additional treatment.
- Residual risk estimates what remains after proposed treatment.
- Score bands: **20-25 Critical, 12-19 High, 6-11 Medium, 1-5 Low.**

The current workbook contains 15 risks: **1 Critical, 13 High, and 1 Medium** inherent risk.

## Featured Assurance Example

The MFA work demonstrates a complete assurance cycle:

**Critical risk -> treatment -> ISO control -> expected evidence -> population testing -> exception -> remediation -> retest -> residual-risk decision**

The simulated test identified two unsupported MFA exceptions, concluded that the control was not operating effectively across the full population, and withheld acceptance of the estimated residual-risk score pending remediation and retesting.

## Skills Demonstrated

- ISO/IEC 27001 readiness assessment
- ISMS scoping and asset identification
- Inherent and residual-risk analysis
- Control-gap assessment
- Risk treatment and remediation tracking
- Selected-control SoA reasoning
- Evidence planning, population reconciliation, and sampling
- Control testing and exception analysis
- ISO-NIST-SOC 2 cross-framework mapping
- Policy development
- Business-oriented security communication

## Interview Walkthrough

> I built a simulated ISO 27001 readiness assessment for a fictional fintech company. I defined the ISMS scope and key assets, created a risk methodology and 15-item risk register, assessed inherent risk, recommended treatments, performed a 12-area gap assessment, and mapped selected Annex A controls. I then created an MFA testing workpaper using a simulated 108-account population. I reconciled the population to system reports, evaluated exceptions, concluded the control was not fully effective, and withheld residual-risk acceptance until remediation and retesting. I also mapped the MFA objective to NIST CSF 2.0 PR.AA-03 and the SOC 2 CC6.1 logical-access theme.
