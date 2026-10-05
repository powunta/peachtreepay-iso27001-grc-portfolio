# MFA Cross-Framework Mapping

> **Portfolio crosswalk - not an official equivalency determination.**  
> Frameworks have different purposes, structures, scopes, and assessment requirements. This mapping shows how one PeachtreePay control objective relates to comparable outcomes and criteria.

## Control Objective

**Require multi-factor authentication for all in-scope human accounts accessing Microsoft 365, AWS, administrative functions, remote access, and sensitive applications.**

## Focused Crosswalk

| Framework | Reference | Relationship to the MFA objective | Example PeachtreePay evidence |
|---|---|---|---|
| ISO/IEC 27001:2022 Annex A | **A.8.5 - Secure authentication** | Supports secure authentication technologies and procedures based on access restrictions and risk | Microsoft 365/AWS MFA configuration reports; authentication standard; approved exception register |
| NIST Cybersecurity Framework 2.0 | **PR.AA-03 - Users, services, and hardware are authenticated** | Expresses the desired authentication outcome; NIST lists requiring MFA as an implementation example | MFA-enforcement export; AWS IAM credential report; sample login validation |
| SOC 2 Trust Services Criteria | **CC6.1 alignment theme** | Relates to implementing logical-access security over protected information and system resources | Access-control policy; user-access inventory; MFA settings; approvals; periodic access reviews |

## Supporting ISO Control Themes

| ISO/IEC 27001:2022 control | Why it supports the MFA objective |
|---|---|
| A.5.15 - Access control | Establishes access-control expectations based on business and security requirements |
| A.5.16 - Identity management | Supports management of identities across their lifecycle |
| A.5.17 - Authentication information | Supports appropriate allocation and management of authentication information |
| A.8.5 - Secure authentication | Provides the most direct alignment to the technical MFA objective |

## Evidence-to-Framework Traceability

| Evidence | ISO/IEC 27001:2022 | NIST CSF 2.0 | SOC 2 alignment | What the analyst tests |
|---|---|---|---|---|
| Access-control policy | A.5.15, A.8.5 | PR.AA-03 | CC6.1 | Whether management established a clear MFA requirement |
| In-scope account population | A.5.16 | PR.AA-01, PR.AA-03 | CC6.1 | Whether all required identities are included |
| MFA configuration reports | A.8.5 | PR.AA-03 | CC6.1 | Whether MFA is enforced for required accounts |
| Exception register | A.5.15, A.8.5 | PR.AA-03 | CC6.1 | Whether deviations are approved, time-bound, and monitored |
| Control-testing workpaper | A.8.5 | PR.AA-03 | CC6.1 | Whether evidence supports design and operating effectiveness |

## Mapping Rationale

The mapping begins with a shared business outcome rather than assuming the frameworks are identical:

1. PeachtreePay needs to reduce the likelihood of credential-based account compromise.
2. MFA is selected as a risk treatment and authentication safeguard.
3. ISO/IEC 27001 Annex A 8.5 provides the primary control alignment used in the portfolio.
4. NIST CSF 2.0 PR.AA-03 expresses the corresponding authentication outcome and explicitly includes MFA as an implementation example.
5. SOC 2 CC6.1 provides a logical-access criterion theme relevant to protecting information and system resources.
6. Evidence is tested once, then interpreted against each applicable framework's purpose and assessment context.

## Important Limitations

- This crosswalk does not claim certification, attestation, or compliance.
- A matching control theme does not make two frameworks equivalent.
- SOC 2 applicability depends on the system description, selected Trust Services Categories, service commitments, and control design.
- An organization should document its mapping rationale and validate it against the authoritative framework publications.

## References

- [NIST Cybersecurity Framework 2.0](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.pdf)
- [NIST CSF 2.0 Implementation Examples](https://www.nist.gov/document/csf-20-implementations-pdf)
- [ISO/IEC 27001 overview](https://www.iso.org/standard/27001)
- AICPA, *Trust Services Criteria* (CC6 logical-access criteria)

## Related Artifacts

- [MFA control-testing workpaper](08-mfa-control-testing-workpaper.md)
- [MFA risk traceability case study](../case-studies/mfa-risk-traceability.md)
- [Statement of Applicability sample](04-statement-of-applicability.md)
