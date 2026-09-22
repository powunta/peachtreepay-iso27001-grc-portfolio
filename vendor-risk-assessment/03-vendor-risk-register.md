# Vendor Risk Register

| ID | Risk | Likelihood | Impact | Inherent Score | Rating | Treatment |
|---|---|---:|---:|---:|---|---|
| VR-01 | Privileged account compromise due to incomplete MFA enforcement | 4 | 5 | 20 | Critical | Mitigate |
| VR-02 | Delayed breach notification could slow PeachtreePay response and legal assessment | 3 | 5 | 15 | High | Mitigate / Contract |
| VR-03 | Incomplete disaster-recovery testing could result in prolonged service outage | 3 | 4 | 12 | High | Mitigate |
| VR-04 | Excessive retention could increase privacy and breach exposure | 3 | 4 | 12 | High | Mitigate / Contract |
| VR-05 | Delayed removal of privileged access after termination could permit unauthorized access | 3 | 4 | 12 | High | Mitigate |
| VR-06 | Open medium penetration-test findings could be exploited if remediation is delayed | 2 | 4 | 8 | Moderate | Monitor / Mitigate |
| VR-07 | Subprocessor changes could introduce new downstream risk | 2 | 4 | 8 | Moderate | Monitor |
| VR-08 | Vendor outage could interrupt customer-support operations | 3 | 3 | 9 | Moderate | Mitigate / Continuity |

## Detailed Analysis

### VR-01 - Incomplete MFA for Privileged Access
**Business impact:** Unauthorized administrator access could expose or alter PeachtreePay customer information.

**Why it matters:** Privileged credentials provide broad access. A legacy workflow without mandatory MFA creates a disproportionate attack path.

**Required treatment:** Mandatory MFA for every privileged administrative workflow before production onboarding, or a documented compensating control approved by PeachtreePay's security owner.

**Target residual risk:** Moderate.

### VR-02 - No Fixed Breach Notification Timeline
**Business impact:** PeachtreePay may lose valuable response time during a security event and could face contractual, regulatory, or customer-notification complications.

**Required treatment:** Add a contractual notification requirement, preferably within 24 hours of confirmed impact to PeachtreePay data.

**Target residual risk:** Moderate.

### VR-03 - Incomplete Recovery Testing
**Business impact:** Recovery assumptions may fail during a real outage.

**Required treatment:** Obtain evidence of a completed recovery exercise with documented RTO/RPO results and lessons learned.

**Target residual risk:** Moderate.

### VR-04 - Excessive Data Retention
**Business impact:** Keeping information longer than necessary increases the amount of data exposed in a breach and can complicate privacy obligations.

**Required treatment:** Configure shorter retention where possible and define verified deletion procedures in contract or operating procedure.

**Target residual risk:** Moderate.

### VR-05 - Privileged Termination Delay
**Business impact:** Departed personnel could retain sensitive access longer than PeachtreePay considers acceptable.

**Required treatment:** Require expedited privileged-account disablement and immediate action for involuntary termination.

**Target residual risk:** Low to Moderate.
