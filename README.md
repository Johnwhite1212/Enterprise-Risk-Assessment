# Enterprise Risk Assessment & GRC Portfolio Project

## Overview

This project demonstrates a structured enterprise risk assessment and Governance, Risk, and Compliance (GRC) workflow for a fictional financial services organization, Acme Financial Services.

The assessment identifies business and technology risks, evaluates inherent risk, documents proposed controls, tracks evidence requirements, develops risk treatment plans, and maps risks to the NIST Cybersecurity Framework (CSF) 2.0.

The project was developed as a simulated portfolio exercise to demonstrate practical risk management, security documentation, control assessment, and compliance-support skills.

## Project Objectives

- Identify and document enterprise security risks.
- Evaluate inherent risk using a consistent likelihood and impact methodology.
- Prioritize risks using a 5×5 risk matrix.
- Assess control design separately from implementation and operating effectiveness.
- Establish evidence requirements and validation procedures.
- Develop risk treatment plans with proposed ownership and timelines.
- Map identified risks to NIST CSF 2.0.
- Define proposed business continuity and disaster recovery requirements.
- Perform cross-file data validation and quality checks.

## Project Deliverables

| Deliverable | Description |
|---|---|
| Risk Register | Eight documented enterprise risks with likelihood, impact, inherent scores, and severity |
| Risk Prioritization Matrix | 5×5 matrix showing risk placement by likelihood and impact |
| Control Assessment | Sixteen proposed security controls with design and assessment statuses |
| Evidence Tracker | Thirty evidence requirements linked to risks and controls |
| Risk Treatment Plan | Eight proposed treatment plans with actions, owners, and target timelines |
| NIST CSF 2.0 Mapping | Eight proposed mappings connecting risks to framework functions and categories |
| Business Impact Analysis | Five business assets with proposed criticality ratings and recovery objectives |
| Recovery Requirements | Proposed RTO and RPO requirements for critical business assets |
| Executive Summary | Management-oriented overview of assessment results and priorities |
| Risk Assessment Methodology | Documented risk scoring, severity thresholds, and assessment approach |
| Evidence Validation Procedure | Proposed evidence collection, review, validation, and testing procedures |

## Risk Assessment Results

Eight risks were documented and evaluated.

| Severity | Number of Risks |
|---|---:|
| Critical | 4 |
| High | 3 |
| Moderate | 1 |
| Low | 0 |
| **Total** | **8** |

### Risk Scoring Methodology

Inherent risk is calculated using:

**Likelihood × Impact = Inherent Risk Score**

Both likelihood and impact use a 1–5 scale.

| Score | Severity |
|---|---|
| 17–25 | Critical |
| 10–16 | High |
| 5–9 | Moderate |
| 1–4 | Low |

## Control Assessment Approach

The control assessment distinguishes between three separate dimensions:

- **Design adequacy:** Whether the proposed control is appropriately designed to address the identified risk.
- **Implementation status:** Whether the control has actually been implemented and supported by evidence.
- **Operating effectiveness:** Whether the control operates consistently and achieves its intended purpose.

All 16 controls have an assessment status of Adequate for design. Implementation remains Not Verified, and operating effectiveness has Not Been Tested.

These distinctions prevent proposed controls from being misrepresented as implemented or effective controls.

## Evidence Management

The evidence tracker contains 30 evidence requirements.

All evidence records are currently classified as:

`Simulated - Not Collected`

The evidence validation procedure defines how evidence should be collected, reviewed, authenticated, evaluated, and documented.

No actual organizational security evidence or control-testing results are claimed.

## Risk Treatment

Eight risk treatment plans were developed using the Mitigate strategy.

Each plan includes:

- Treatment rationale
- Proposed remediation actions
- Proposed ownership
- Target completion timeline
- Implementation status
- Residual risk assessment
- Approval status
- Verification evidence requirements

Treatment timelines and ownership are proposed and have not been approved as organizational commitments.

## NIST CSF 2.0 Alignment

The project includes eight proposed risk mappings to the NIST Cybersecurity Framework 2.0.

The mappings cover applicable framework functions, categories, subcategory references, related controls, and evidence requirements.

These are proposed mappings, not a formal NIST assessment, certification, or compliance determination.

## Business Impact Analysis and Recovery Planning

The Business Impact Analysis documents five business assets with proposed criticality ratings.

The customer database and customer portal are classified as Critical, with proposed recovery objectives of:

- Recovery Time Objective (RTO): 4 hours
- Recovery Point Objective (RPO): 15 minutes

All recovery objectives are pending business approval. No actual disaster recovery or restoration tests have been performed.

## Quality Assurance and Validation

PowerShell was used to validate project data and relationships across deliverables.

Validation checks included:

- Risk scoring and severity classification
- Unique risk, control, and evidence identifiers
- Valid control-to-risk references
- Valid treatment-plan-to-risk references
- Valid NIST-to-risk references
- Valid control-to-evidence references
- Evidence coverage across controls
- Treatment plan coverage across risks
- Control and NIST mapping coverage across risks
- Required field completeness

The completed cross-file validation reported zero invalid risk references and zero invalid evidence references.

## Project Documentation and Screenshots

The `documentation` folder contains the risk assessment methodology and evidence validation procedure.

The `reports` folder contains the executive summary.

The `screenshots` folder contains six project screenshots demonstrating:

1. Risk register
2. Risk prioritization matrix
3. Cross-file validation results
4. Risk assessment methodology
5. Evidence validation procedure
6. Executive summary

## Tools and Technologies

- Windows PowerShell
- Visual Studio Code
- Microsoft Excel
- CSV data management
- Markdown documentation
- NIST Cybersecurity Framework 2.0
- Risk assessment and GRC concepts

## Repository Structure

```text
enterprise-risk-assessment/
│
├── archive/
│   ├── evidence-tracker.backup-before-cleanup.csv
│   └── evidence-tracker.before-E010-fix.csv
│
├── documentation/
│   ├── risk-assessment-methodology.md
│   └── evidence-validation-procedure.md
│
├── reports/
│   └── executive-summary.md
│
├── screenshots/
│   ├── 01-risk-register.png
│   ├── 02-risk-prioritization-matrix.png
│   ├── 03-cross-file-validation.png
│   ├── 04-risk-assessment-methodology.png
│   ├── 05-evidence-validation-procedure.png
│   └── 06-executive-summary.png
│
├── business-impact-analysis.csv
├── control-assessment.csv
├── evidence-tracker.csv
├── nist-control-mapping.csv
├── recovery-requirements.csv
├── risk-prioritization-matrix.csv
├── risk-register.csv
├── risk-treatment-plan.csv
└── README.md
```

## Assessment Limitations

This is a simulated portfolio assessment based on a fictional organization.

It does not represent an actual enterprise audit, penetration test, security certification, or independent control assessment.

No claims are made that the proposed controls have been implemented, that evidence has been collected, or that organizational compliance has been established.

The project demonstrates the documentation, analytical approach, validation techniques, and structured workflows used in GRC and cybersecurity risk assessment activities.

## Key Skills Demonstrated

- Enterprise risk identification and analysis
- Inherent risk scoring and prioritization
- Security control assessment
- Evidence management and validation
- Risk treatment planning
- NIST CSF 2.0 framework mapping
- Business impact analysis
- Business continuity and disaster recovery planning
- PowerShell data validation and automation
- Technical documentation and reporting