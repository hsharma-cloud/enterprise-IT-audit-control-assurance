# Test Results

**Project:** enterprise-IT-audit-control-assurance
**Version:** 1.0
**Owner:** IT Audit Function

---

## 1. Purpose

The purpose of this document is to record the results of control testing performed during the audit. It provides a structured record of test execution, evidence collected, and conclusions regarding control effectiveness.

---



## 2. Objectives

* Document outcomes of control testing
* Provide evidence-based conclusions
* Identify control deficiencies and exceptions
* Support development of audit findings

---

## 3. Results Structure

Each test result includes:

* Test ID
* Control ID
* Test Description
* Test Type (ToD / ToE)
* Result (Effective / Partially Effective / Ineffective)
* Observations
* Evidence Reference

---

---

## 4. Executive Summary

This control testing activity evaluated the effectiveness of cloud security controls across compute, storage, and identity services.

Testing identified multiple security issues, including a critical attack path that could allow unauthorized access to sensitive data through a combination of public exposure, excessive permissions, and resource misconfigurations.

Automated validation using Wiz provided visibility into misconfigurations, vulnerabilities, and identity risks, enabling prioritized remediation based on real-world attack scenarios.

Key risks identified include:
- Publicly exposed compute resources
- Over-permissioned IAM roles
- Unrestricted network access via security groups

These findings indicate gaps in control implementation and highlight the need for improved enforcement of least privilege, network restrictions, and secure configuration practices.

Overall, the control environment requires remediation to reduce risk exposure and align with security best practices and compliance frameworks such as CIS and NIST.

## 4. Test Results Summary

| Test ID | Control ID | Description                  | Type    | Result              | Observation                              | Evidence Ref |
| ------- | ---------- | ---------------------------- | ------- | ------------------- | ---------------------------------------- | ------------ |
| AP-01   | C-001      | MFA Enforcement              | ToD/ToE | Effective           | MFA enabled for all sampled users        | EV-001       |
| AP-02   | C-007      | Firewall Rule Enforcement    | ToD/ToE | Effective           | Rules align with policy                  | EV-002       |
| AP-03   | C-002      | Role-Based Access Control    | ToD/ToE | Partially Effective | Some users have excessive permissions    | EV-003       |
| AP-04   | C-004      | Privileged Access Monitoring | ToE     | Effective           | Logs monitored and alerts configured     | EV-004       |
| AP-05   | C-003      | User Deprovisioning          | ToE     | Ineffective         | Delays in removing access for some users | EV-005       |
| AP-06   | C-005      | Centralized Logging          | ToD/ToE | Effective           | Logs collected and monitored             | EV-006       |
| AP-07   | C-006      | Patch Management             | ToE     | Partially Effective | Some systems not patched on time         | EV-007       |

---

## 5. Result Classification

### 5.1 Effective

* Control is properly designed and operating consistently

### 5.2 Partially Effective

* Control exists but has weaknesses or inconsistencies

### 5.3 Ineffective

* Control is missing, poorly designed, or not operating

---

## 6. Key Observations

* Excessive access permissions identified in some user accounts
* Delays in user deprovisioning process
* Inconsistent patching across systems

---

## 7. Exceptions Identified

Exceptions include:

* Users with inappropriate access levels
* Delayed removal of access for terminated users
* Systems not meeting patching timelines

---

## 8. Evidence Reference

Evidence is stored in the audit evidence repository and includes:

* System screenshots
* Logs and reports
* Configuration files

Each test result references corresponding evidence IDs.

---

## 9. Conclusion

Control testing results indicate that while several controls are operating effectively, some controls require improvement to fully mitigate associated risks.

---
Detailed evidence and validation outputs are documented in Section 06: Evidence and Validation.

## Finding: Critical Cloud Attack Path Identified

### Description
A critical attack path was identified through automated analysis using Wiz. The path combines multiple security weaknesses that could allow an attacker to gain unauthorized access to sensitive data.

### Observation
- An EC2 instance was publicly accessible via an open security group
- The EC2 instance had an attached IAM role with excessive permissions
- The IAM role allowed access to S3 resources

### Risk
An external attacker could potentially:
- Access the EC2 instance
- Exploit vulnerabilities or misconfigurations
- Leverage IAM role permissions
- Access or exfiltrate sensitive data from S3

### Impact
- Unauthorized access to cloud resources
- Potential data breach
- Compromise of cloud environment

### Evidence
- Findings identified through Wiz cloud security platform
- Configuration review of EC2, IAM roles, and S3 permissions

### Recommendation
- Restrict public access to EC2 instances
- Apply least privilege to IAM roles
- Review and secure S3 bucket permissions

### Severity
Critical

### Control Mapping

| Control Framework | Control ID | Description |
|------------------|-----------|------------|
| CIS AWS Foundations | 4.1 | Ensure no security groups allow unrestricted inbound access |
| CIS AWS Foundations | 1.16 | Ensure IAM policies follow least privilege |
| NIST SP 800-53 | AC-6 | Least Privilege |
| NIST SP 800-53 | SC-7 | Boundary Protection |

### Compliance Impact
The identified issues indicate non-compliance with established security best practices and control frameworks. Failure to remediate may result in increased risk exposure and potential audit findings.
## Finding: Overly Permissive Security Group Configuration

### Description
A security group was identified allowing unrestricted inbound access from the internet, increasing exposure of cloud resources.

### Observation
- Security group allows inbound traffic from 0.0.0.0/0
- Ports exposed include SSH (22) and/or HTTP (80)

### Risk
Unrestricted access increases the likelihood of:
- Unauthorized access attempts
- Brute-force attacks
- Exploitation of exposed services

### Impact
- Increased attack surface
- Potential compromise of compute resources

### Evidence
- Security group configuration review
- Findings identified through Wiz cloud security platform

### Recommendation
- Restrict inbound access to trusted IP ranges
- Implement bastion host or VPN for administrative access

### Severity
Medium

### Control Mapping

| Control Framework | Control ID | Description |
|------------------|-----------|------------|
| CIS AWS Foundations | 4.1 | Ensure no security groups allow unrestricted inbound access |
| NIST SP 800-53 | SC-7 | Boundary Protection |

### Compliance Impact
The configuration does not align with recommended network security practices and increases exposure to external threats.
**End of Document**

