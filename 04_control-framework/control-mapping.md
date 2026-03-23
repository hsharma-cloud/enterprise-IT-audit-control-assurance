# Control Mapping

**Project:** enterprise-IT-audit-control-assurance
**Version:** 1.0
**Owner:** IT Audit Function

---

## 1. Purpose

The purpose of this document is to map identified risks to control objectives and implemented controls. This ensures traceability and demonstrates that risks are adequately addressed through appropriate controls.

---

## 2. Objectives

* Establish clear linkage between risks, control objectives, and controls
* Ensure complete coverage of identified risks
* Support audit testing and validation
* Enable traceability for audit and compliance purposes

---

## 3. Mapping Structure

The control mapping includes:

* Risk ID (from Risk Register)
* Control Objective (from Control Objectives)
* Control ID (from Control Library)
* Control Description
* Control Type
* Audit Test Reference

---

## 4. Control Mapping Table

| Risk ID | Risk Description            | Control Objective Ref | Control ID | Control Description          | Type       | Audit Test Ref |
| ------- | --------------------------- | --------------------- | ---------- | ---------------------------- | ---------- | -------------- |
| R-001   | Unauthorized access         | 4.1                   | C-001      | Multi-Factor Authentication  | Preventive | AP-01          |
| R-001   | Unauthorized access         | 4.5                   | C-007      | Firewall Rule Enforcement    | Preventive | AP-02          |
| R-002   | Excessive user privileges   | 4.1                   | C-002      | Role-Based Access Control    | Preventive | AP-03          |
| R-002   | Excessive user privileges   | 4.3                   | C-004      | Privileged Access Monitoring | Detective  | AP-04          |
| R-003   | Delayed user deprovisioning | 4.2                   | C-003      | User Deprovisioning Process  | Preventive | AP-05          |
| R-004   | Insufficient logging        | 4.4                   | C-005      | Centralized Logging          | Detective  | AP-06          |
| R-005   | Unpatched vulnerabilities   | 4.6                   | C-006      | Patch Management Process     | Corrective | AP-07          |

---

## 5. Traceability

This mapping ensures full traceability across:

* Risk Register → Control Objectives
* Control Objectives → Control Library
* Controls → Audit Procedures

---

## 6. Coverage Analysis

The mapping should be reviewed to ensure:

* All high-risk items have corresponding controls
* Controls are aligned with appropriate objectives
* No critical gaps exist

---

## 7. Gap Identification

Gaps may exist if:

* A risk has no associated control
* Controls do not fully address the control objective
* Controls are not properly implemented

Identified gaps must be documented and addressed.

---

## 8. Audit Testing Integration

Each control is linked to an audit test reference, ensuring:

* Clear connection between controls and testing procedures
* Efficient execution of audit programs
* Consistent documentation of results

---

## 9. Maintenance

Control mappings must be:

* Updated when risks or controls change
* Reviewed periodically
* Aligned with audit findings and updates

---

## 10. Conclusion

Control Mapping provides a comprehensive view of how risks are mitigated through controls, enabling effective audit planning, execution, and reporting.

---

**End of Document**

