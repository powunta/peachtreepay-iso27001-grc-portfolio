# CT-01 — Synthetic terminated-user EHR access review
**Risk:** R01 | **Objective:** Terminated staff should lose routine EHR access within the **fictional 24-hour internal policy**. This is not a general statutory HIPAA deadline.

**Population:** 24 fictional workforce departures in September 2026. **Procedure:** Compare HR separation timestamps with EHR/identity disable times across 100% of this synthetic population. **Outcome:** 20 passed, 4 exceptions, 16.7% exception rate. Conclusion: **control not operating effectively in this scenario**.

| Case | Simulated disable delay | Hypothesized cause | Recommended response |
|---|---:|---|---|
| T-04 | 72 hours | HR ticket not entered | Automate HR event trigger |
| T-11 | 96 hours | Vendor identity omitted | Include all human and third-party identities |
| T-18 | 51 hours | Weekend processing gap | Urgent offboarding coverage |
| T-23 | 168 hours | Closure without validation | Independent evidence-based verification |

**Limitations:** A still-enabled account is not proof that anyone accessed patient data. No actual breach, access misuse or legal violation was established. Every record is synthetic.

**Retest:** After remediation, evaluate the next 20–30 departures across staff roles and sites, reconcile HR and EHR/IdP records, investigate any delay over the documented policy, and confirm evidence of control closure.
