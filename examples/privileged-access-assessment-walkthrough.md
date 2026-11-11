# Privileged Access Assessment Walkthrough

This example follows **PA-010**, a privileged cloud account in the fictional evidence, through the assessment.

1. **Identify the gap.** The account inventory lists PA-010 as active, with an unassigned owner and a missing approval reference. The MFA report says multifactor authentication is configured, but enforcement is **Unknown**. Its sampled login also has an **Unknown** MFA outcome.

2. **Make a supported judgment.** These records leave ownership, authorization, and authentication safeguards unverified. They do not prove MFA was disabled or that the account was misused. CTL-05 is rated **Partially Met**, considering the safeguards recorded for nine accounts alongside PA-010 and the other unresolved cases.

3. **Connect the gap to business risk.** Unauthorized administrative access could expose information, change configurations, or disrupt payment services. Related risk R-001, which also covers PA-012, is **High: likelihood 3 × impact 5 = 15/25**. These are scenario-based estimates. Its residual estimate remains 15 because effective safeguards for the affected accounts have not been established.

4. **Define an action and a way to verify it.** Recommend that the fictional IAM / Privileged Access Owner validate ownership and authorization and verify/enforce applicable MFA. Closing R-001 requires ownership and authorization records for PA-010 and PA-012, MFA-enforcement evidence for PA-010, and documented authentication safeguards for PA-012. The roadmap records a November 13, 2026 target; the action remains **Open**.

This demonstrates evidence comparison, control assessment, business-risk reasoning, and remediation planning.

**Trace the example:** [Evidence records](../northstar-grc-assessment/Evidence/CTL-05_Privileged_access_and_MFA/) · [Control assessment — CTL-05](../Northstar_PDFs/02_Northstar_Control_Assessment_Matrix.pdf) · [Risk register — R-001](../Northstar_PDFs/03_Northstar_Risk_Register.pdf) · [Remediation roadmap — R-001](../Northstar_PDFs/Northstar_Remediation_Roadmap.pdf)

[Back to the project overview](../README.md)

