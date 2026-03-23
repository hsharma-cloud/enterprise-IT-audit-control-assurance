# Test Procedures

**Project:** enterprise-IT-audit-control-assurance
**Version:** 1.0
**Owner:** IT Audit Function

---

## 1. Purpose

The purpose of this document is to define detailed, step-by-step procedures for testing controls identified in the control framework. These procedures ensure consistency, repeatability, and accuracy in audit execution.

---

## 2. Objectives

* Provide clear instructions for control testing
* Ensure alignment with control objectives and risks
* Standardize audit execution
* Enable traceability between controls and test results

---

## 3. Procedure Structure

Each test procedure includes:

* Test ID
* Control ID
* Objective
* Test Type (ToD / ToE)
* Procedure Steps
* Expected Result
* Evidence Required

---

## 4. Test Procedures

---

### AP-01: Multi-Factor Authentication (MFA)

* **Control ID:** C-001
* **Objective:** Ensure MFA is enforced for user access
* **Test Type:** ToD & ToE

**Procedure Steps:**

1. Review MFA policy and configuration settings
2. Verify MFA is enabled for all user accounts
3. Select a sample of users and confirm MFA enforcement during login

**Expected Result:**

* MFA is enabled and enforced for all applicable users

**Evidence Required:**

* System configuration screenshots
* Authentication logs

---

### AP-02: Firewall Rule Enforcement

* **Control ID:** C-007
* **Objective:** Ensure network traffic is properly controlled
* **Test Type:** ToD & ToE

**Procedure Steps:**

1. Review firewall rule configurations
2. Verify rules align with security policy
3. Test sample traffic to confirm enforcement

**Expected Result:**

* Unauthorized traffic is blocked
* Authorized traffic is allowed

**Evidence Required:**

* Firewall configurations
* Network logs

---

### AP-03: Role-Based Access Control (RBAC)

* **Control ID:** C-002
* **Objective:** Ensure access is assigned based on roles
* **Test Type:** ToD & ToE

**Procedure Steps:**

1. Obtain user access listings
2. Review role definitions
3. Verify user permissions align with assigned roles

**Expected Result:**

* Access is consistent with defined roles

**Evidence Required:**

* Access reports
* Role definitions

---

### AP-04: Privileged Access Monitoring

* **Control ID:** C-004
* **Objective:** Ensure privileged activities are logged and monitored
* **Test Type:** ToE

**Procedure Steps:**

1. Obtain list of privileged accounts
2. Review activity logs
3. Verify monitoring and alerting mechanisms

**Expected Result:**

* All privileged activities are logged and reviewed

**Evidence Required:**

* Activity logs
* SIEM alerts

---

### AP-05: User Deprovisioning

* **Control ID:** C-003
* **Objective:** Ensure timely removal of user access
* **Test Type:** ToE

**Procedure Steps:**

1. Select a sample of terminated users
2. Verify account deactivation timelines
3. Confirm access removal from systems

**Expected Result:**

* Access is removed promptly after termination

**Evidence Required:**

* HR records
* System logs

---

### AP-06: Centralized Logging

* **Control ID:** C-005
* **Objective:** Ensure logs are collected and monitored
* **Test Type:** ToD & ToE

**Procedure Steps:**

1. Verify log collection configuration
2. Review sample logs in SIEM
3. Confirm alert generation

**Expected Result:**

* Logs are centralized and monitored

**Evidence Required:**

* SIEM logs
* Alert reports

---

### AP-07: Patch Management

* **Control ID:** C-006
* **Objective:** Ensure systems are patched regularly
* **Test Type:** ToE

**Procedure Steps:**

1. Review patch management policy
2. Select a sample of systems
3. Verify patch levels and update timelines

**Expected Result:**

* Systems are patched within defined timelines

**Evidence Required:**

* Patch reports
* System configurations

---

## 5. Documentation of Results

For each test:

* Record execution steps
* Attach supporting evidence
* Document results and exceptions

---

## 6. Exception Handling

* Document any deviations from expected results
* Assess impact and risk
* Link exceptions to findings

---

## 7. Conclusion

Test procedures provide a consistent and structured approach to evaluating controls and ensuring reliable audit outcomes.

---

**End of Document**

