# Evidence Collection and Validation Procedure
## Enterprise Risk Assessment — Acme Financial Services

**Organization:** Acme Financial Services (Fictional)  
**Document Type:** GRC Evidence Validation Procedure  
**Framework Reference:** NIST Cybersecurity Framework (CSF) 2.0  
**Document Status:** Proposed Procedure

---

## 1. Purpose

This procedure establishes a consistent process for collecting, reviewing, validating, and retaining evidence used to assess information security controls.

The objective is to ensure that conclusions about control design, implementation, and operating effectiveness are supported by relevant, reliable, and appropriately documented evidence.

This procedure supports the enterprise risk assessment, control assessment, evidence tracker, and risk treatment plan.

## 2. Scope

This procedure applies to evidence associated with the following security domains:

- AWS identity and access management.
- Amazon S3 security configurations.
- Data encryption and AWS KMS.
- AWS CloudTrail logging and monitoring.
- Network security and security group configurations.
- Vulnerability scanning and patch management.
- Backup and recovery operations.
- Employee and service account access reviews.

Evidence should be associated with its applicable risk ID, control ID, and evidence ID.

## 3. Evidence Collection Principles

Evidence should be:

**Relevant:** Directly supports the control requirement being assessed.

**Authentic:** Obtained from an identifiable and trustworthy source.

**Complete:** Contains sufficient information to support the intended assessment.

**Current:** Reflects the applicable assessment period or the date of testing.

**Reliable:** Produced by an appropriate system, process, or authorized individual.

**Traceable:** Linked to the relevant risk, control, evidence record, and assessment conclusion.

Evidence should be collected using approved access methods and handled according to organizational security and data protection requirements.

Sensitive information, credentials, customer records, and other confidential data should not be unnecessarily copied into assessment documentation.

## 4. Evidence Sources

Examples of acceptable evidence sources include:

| Security Domain | Example Evidence |
|---|---|
| S3 security | Block Public Access settings, bucket policies, access configuration |
| IAM security | IAM users, roles, permissions, MFA configuration |
| Encryption | KMS key policies, encryption settings, configuration exports |
| Logging | CloudTrail configuration, event history, log validation records |
| Network security | Security group rules, network access configurations |
| Vulnerability management | Authenticated vulnerability scan reports, remediation records |
| Patch management | Patch compliance reports, change records |
| Backup and recovery | Backup job reports, retention settings, restoration test results |
| Access governance | Access review records, manager approvals, termination records |

Evidence should originate from the relevant AWS service, approved security tool, business process, or responsible control owner.

## 5. Evidence Collection Procedure

### Step 1 — Identify the Control Requirement

Review the control assessment and determine:

- What security requirement must be validated?
- Which risk does the control address?
- What evidence would demonstrate implementation?
- What evidence would demonstrate operating effectiveness?

### Step 2 — Identify the Evidence Source

Determine the authoritative source of the requested evidence.

Examples include AWS IAM, Amazon S3, AWS CloudTrail, AWS KMS, vulnerability management platforms, and approved organizational records.

### Step 3 — Request or Collect Evidence

Obtain evidence through approved procedures.

Record:
- Evidence ID.
- Related risk ID.
- Related control ID.
- Evidence description.
- Source system or responsible individual.
- Collection date.
- Assessment period.
- Person responsible for collection.

### Step 4 — Preserve Evidence

Retain evidence in an approved, access-controlled location.

Where appropriate, preserve original exports or reports and record collection metadata.

Evidence should not be altered in a way that changes its meaning or compromises its integrity.

### Step 5 — Review Evidence

Compare the evidence against the documented control requirements.

Determine whether the evidence demonstrates:
- Control design.
- Control implementation.
- Control operation.
- Consistent performance over the applicable assessment period.

### Step 6 — Document the Assessment

Record the evidence review outcome and any identified deficiencies.

Update the evidence tracker and control assessment with the appropriate status.

## 6. Evidence Validation Checks

Each evidence item should be evaluated against the following criteria.

| Validation Check | Review Question |
|---|---|
| Relevance | Does the evidence support the intended control? |
| Authenticity | Can the source of the evidence be identified? |
| Completeness | Is sufficient information available to evaluate the control? |
| Currency | Does the evidence cover the relevant assessment period? |
| Integrity | Is there reason to believe the evidence was altered or corrupted? |
| Traceability | Is the evidence linked to the correct risk and control? |
| Reliability | Is the source appropriate for the conclusion being made? |

Evidence that fails a required validation check should be documented as insufficient, rejected, or requiring additional information.

## 7. Control Testing Procedures

Evidence review alone may not demonstrate operating effectiveness.

Where appropriate, controls should be tested using inspection, inquiry, observation, and reperformance.

Examples:

**S3 Access Restrictions**
- Inspect account-level and bucket-level Block Public Access settings.
- Review bucket policies and access permissions.
- Test whether unauthorized access is prevented using an approved test procedure.

**IAM Multi-Factor Authentication**
- Inspect MFA configuration for privileged identities.
- Review applicable IAM policies and authentication requirements.
- Verify enforcement using an approved test account or controlled test procedure.

**CloudTrail Logging**
- Inspect trail configuration and required regional coverage.
- Review log delivery and retention settings.
- Generate or identify an approved test event and confirm that it is recorded.

**Security Group Restrictions**
- Inspect production security group inbound rules.
- Identify unrestricted administrative access.
- Verify that approved restrictions are in place.

**Vulnerability Management**
- Review authenticated vulnerability scan reports.
- Inspect remediation records for critical findings.
- Perform follow-up scanning to confirm remediation.

**Backup and Recovery**
- Inspect backup schedules, retention, and protection settings.
- Review backup job success and failure records.
- Perform an approved restoration exercise.
- Compare measured recovery performance with approved RTO and RPO objectives.

Testing should be authorized, appropriately scoped, and documented. Testing must not disrupt production services or expose sensitive information.

## 8. Evidence Assessment Outcomes

The following outcomes should be used when documenting evidence validation.

| Outcome | Meaning |
|---|---|
| Verified | Evidence is sufficient and supports the stated control requirement |
| Partially Verified | Evidence supports some requirements, but gaps remain |
| Insufficient Evidence | Evidence is incomplete, unreliable, or does not support the conclusion |
| Not Collected | Required evidence has not been obtained |
| Rejected | Evidence is invalid, irrelevant, or cannot be relied upon |
| Pending Review | Evidence has been received but not yet evaluated |

A `Verified` result should only be assigned after the applicable evidence review has been completed.

A control should not be marked effective solely because evidence has been received.

## 9. Deficiency and Exception Management

When evidence identifies a control deficiency:

1. Document the affected control and risk IDs.
2. Describe the observed condition.
3. Identify the applicable security requirement.
4. Assess the potential impact.
5. Assign a responsible owner.
6. Define a remediation action and target date.
7. Track the issue through resolution.
8. Obtain follow-up evidence.
9. Retest the control where appropriate.
10. Update the risk assessment and residual risk evaluation.

Approved exceptions should include a business justification, documented risk impact, compensating controls where applicable, an authorized approver, and an expiration or review date.

## 10. Evidence Retention and Protection

Evidence should be retained according to approved organizational retention requirements.

Access should be limited to authorized personnel.

Evidence handling should consider:
- Confidentiality.
- Integrity.
- Availability.
- Access restrictions.
- Retention requirements.
- Secure disposal.
- Audit trail and traceability.

Credentials, secret keys, access tokens, and unnecessary customer information must not be stored in public repositories or unprotected project files.

## 11. Reporting Requirements

Evidence validation results should be reflected in the control assessment and evidence tracker.

Assessment reporting should distinguish between:

- Controls designed appropriately.
- Controls implemented and verified.
- Controls operating effectively.
- Controls with identified deficiencies.
- Controls not assessed due to missing evidence.

Material deficiencies should be communicated to the appropriate risk owner and management stakeholders.

## 12. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| GRC Analyst | Coordinate evidence requests, validate documentation, maintain assessment records |
| Control Owner | Provide evidence and explain control operation |
| Cloud Security Team | Provide cloud security configuration and monitoring evidence |
| IT Operations | Provide infrastructure, backup, and recovery evidence |
| IAM Administrator | Provide identity, access, and authentication evidence |
| Management | Review significant deficiencies and approve risk treatment decisions |

Responsibilities shown are proposed for the simulated organization and have not been formally assigned or approved.

## 13. Current Assessment Application

For this portfolio assessment:

- Thirty evidence requirements have been documented.
- All thirty evidence records are currently marked `Simulated - Not Collected`.
- Sixteen controls have documented design assessments of Adequate.
- All sixteen controls remain Not Verified for implementation.
- All sixteen controls remain Not Tested for operating effectiveness.

No actual organizational evidence has been collected or independently validated.

This procedure describes how evidence should be evaluated when available. It does not represent completed evidence testing.

## 14. Procedure Review and Maintenance

This procedure should be reviewed periodically and updated when:

- Security requirements change.
- New systems or cloud services are introduced.
- Evidence sources or collection methods change.
- New audit or regulatory requirements apply.
- Deficiencies are identified in the evidence validation process.

Changes should be documented and approved by the appropriate organizational authority before operational adoption.

---

**Project:** Enterprise Risk Assessment & GRC Portfolio  
**Organization:** Acme Financial Services (Fictional)  
**Document:** Evidence Collection and Validation Procedure  
**Classification:** Simulated Portfolio Exercise