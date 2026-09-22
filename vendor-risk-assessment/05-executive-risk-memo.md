# Executive Vendor Risk Memo

**To:** PeachtreePay Leadership, Security, Procurement, and Customer Operations  
**From:** GRC Analyst - Simulated Portfolio Exercise  
**Subject:** CloudBridge CRM Third-Party Risk Assessment  
**Decision:** **Conditional Approval**

## Executive Summary

CloudBridge CRM demonstrates several characteristics of a reasonably mature SaaS security program, including independent assurance, encryption, vulnerability management, centralized monitoring, and documented security governance.

However, the assessment identified material gaps involving privileged MFA, breach-notification commitments, disaster-recovery validation, data retention, and privileged-account deprovisioning.

Because the service would process confidential PeachtreePay information and support an important customer-facing business function, these gaps should not be treated as administrative details. They directly affect the likelihood or impact of account compromise, service disruption, delayed incident response, and unnecessary data exposure.

## Recommendation

Proceed with **conditional approval** rather than immediate unrestricted approval.

Production onboarding should not occur until:

1. MFA is enforced for all privileged administrative access, or PeachtreePay approves a documented compensating control.
2. The contract contains a defined security-incident notification commitment.
3. PeachtreePay retention and deletion requirements are agreed and operationally feasible.

The remaining high and moderate findings may proceed under time-bound remediation if the accountable PeachtreePay risk owner accepts the temporary residual exposure.

## Business Rationale

Rejecting the vendor immediately would ignore its existing security strengths and the business value of the CRM service. Approving it without conditions would expose PeachtreePay to avoidable risk. Conditional approval balances business enablement with measurable security requirements.

## Residual Risk Position

If the mandatory pre-production items are completed and the remaining remediation plan is tracked, the overall vendor risk can be reduced to a level that may be acceptable to PeachtreePay management.

## Analyst Takeaway

This assessment demonstrates that third-party risk management is not simply a questionnaire exercise. The analyst must validate claims with evidence, identify meaningful gaps, connect security findings to business impact, define treatment actions, and support a clear risk-informed business decision.
