# Risk Assessment Methodology
## Enterprise Risk Assessment — Acme Financial Services

**Organization:** Acme Financial Services (Fictional)  
**Assessment Type:** Simulated Enterprise Cloud Security Risk Assessment  
**Framework Reference:** NIST Cybersecurity Framework (CSF) 2.0  
**Document Status:** Proposed Assessment Methodology

---

## 1. Purpose

This document defines the methodology used to identify, analyze, score, prioritize, and treat information security risks within the simulated Acme Financial Services environment.

The methodology provides a consistent approach for evaluating potential threats to cloud infrastructure, customer information, business applications, identity systems, and supporting technology services.

It also establishes how inherent risk and residual risk should be distinguished and documented.

## 2. Assessment Scope

The assessment considers the following security and operational areas:

- AWS cloud infrastructure and configuration.
- Identity and access management.
- Customer information protection.
- Encryption and key management.
- Security logging and monitoring.
- Network security.
- Vulnerability and patch management.
- Backup, recovery, and business continuity.
- Employee and service account access governance.

The assessment is a simulated portfolio exercise. No actual customer environment or production security controls were independently assessed.

## 3. Risk Identification

Risks are documented in the risk register and assigned unique identifiers.

Each risk record includes:
- Risk ID.
- Affected asset or business service.
- Risk description.
- Likelihood rating.
- Impact rating.
- Inherent risk score and severity.
- Recommended controls.
- Risk owner.
- Current status.
- Residual risk score and severity, where applicable.

Risk scenarios describe potential events and consequences rather than asserting that a security incident or vulnerability has been confirmed.

## 4. Likelihood Assessment

Likelihood measures the estimated probability that a risk scenario could occur within the assessed environment.

The assessment uses a five-point scale.

| Rating | Classification | Description |
|---|---|---|
| 1 | Rare | Highly unlikely under normal operating conditions |
| 2 | Unlikely | Could occur, but is not expected frequently |
| 3 | Possible | Could reasonably occur under certain conditions |
| 4 | Likely | Expected to occur or has a credible likelihood of occurrence |
| 5 | Almost Certain | Expected to occur frequently or under current conditions |

Likelihood ratings should be supported by available threat information, exposure, existing safeguards, vulnerability information, and relevant operational context.

For this simulated assessment, ratings are illustrative judgments and have not been validated against actual organizational threat data.

## 5. Impact Assessment

Impact measures the potential consequences if a risk scenario occurs.

The assessment considers:
- Confidentiality impact.
- Integrity impact.
- Availability impact.
- Financial consequences.
- Operational disruption.
- Customer impact.
- Regulatory and contractual implications.
- Reputational damage.

A five-point scale is used.

| Rating | Classification | Description |
|---|---|---|
| 1 | Insignificant | Minimal disruption or negligible business consequence |
| 2 | Minor | Limited disruption with manageable consequences |
| 3 | Moderate | Noticeable operational, financial, or customer impact |
| 4 | Major | Significant business disruption, financial loss, or customer impact |
| 5 | Severe | Critical business disruption, substantial customer impact, or potentially serious regulatory consequences |

The assigned impact rating represents the overall assessed consequence of the risk scenario.

For this simulated assessment, impact ratings are proposed judgments rather than validated business-impact measurements.

## 6. Inherent Risk Calculation

Inherent risk represents the level of risk before considering the effectiveness of mitigating controls.

The assessment calculates inherent risk using:

**Inherent Risk Score = Likelihood × Impact**

Both inputs use a scale from 1 to 5.

The resulting score ranges from 1 to 25.

### Inherent Risk Severity Thresholds

| Score | Severity | Priority |
|---|---|---|
| 17–25 | Critical | Immediate management attention |
| 10–16 | High | High remediation priority |
| 5–9 | Moderate | Planned remediation and monitoring |
| 1–4 | Low | Routine monitoring and acceptance review |

The thresholds are the assessment's proposed scoring criteria and should be approved by organizational management before operational adoption.

## 7. Risk Prioritization

Risks are prioritized using their inherent risk scores and severity classifications.

A five-by-five likelihood-versus-impact matrix provides a visual representation of risk concentration.

The matrix supports:
- Identification of high-priority risk scenarios.
- Comparison of risks across business assets.
- Remediation planning.
- Management reporting.
- Allocation of security resources.

Critical risks receive the highest attention, followed by High, Moderate, and Low risks.

Risk prioritization should also consider business criticality, threat exposure, regulatory obligations, and remediation feasibility rather than relying exclusively on numerical scores.

## 8. Control Assessment

Security controls are documented and mapped to the risks they are intended to mitigate.

Each control is evaluated across four assessment attributes:

**Design Assessment:** Evaluates whether the documented control is appropriately designed to address its intended risk.

**Implementation Status:** Determines whether the control has actually been implemented and supported by evidence.

**Operating Effectiveness:** Evaluates whether an implemented control operates consistently and as intended over an appropriate period.

**Test Result:** Records the outcome of control testing.

A control with an adequate documented design is not automatically considered implemented or effective.

In this assessment, all sixteen controls have a design assessment of Adequate. Their implementation remains Not Verified, and operating effectiveness remains Not Tested.

## 9. Evidence Collection and Validation

Evidence is required to support conclusions about control implementation and effectiveness.

Examples include:

- AWS configuration exports.
- IAM users, roles, and policy records.
- S3 Block Public Access and bucket policy settings.
- AWS KMS encryption configuration.
- CloudTrail logging and monitoring records.
- Security