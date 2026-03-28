# Enterprise IT Audit Control & Assurance

## 📌 Overview

This project demonstrates a full **enterprise-grade IT audit and control assurance program**, covering the complete audit lifecycle from planning to reporting.

The objective is to evaluate the design and operating effectiveness of IT controls across a hybrid enterprise environment.

---

## 🎯 Key Capabilities Demonstrated

* Risk-based audit planning and execution
* Control identification and mapping
* Control testing (Design & Operating Effectiveness)
* Evidence-based validation
* Findings development and risk rating
* Executive-level reporting

---

Hands-on enterprise security project implementing NIST-aligned controls using ELK Stack and SaltStack.

## 🔐 Security Control Framework Alignment (NIST-Based)

This project demonstrates hands-on implementation of enterprise security controls aligned with guidance from the National Institute of Standards and Technology (NIST), specifically referencing:

- NIST SP 800-53 (Security and Privacy Controls)
- NIST SP 800-171 (Protection of Controlled Unclassified Information)

The environment simulates a real-world enterprise security monitoring and control system using Ubuntu-based infrastructure, ELK Stack (Elasticsearch, Logstash, Kibana), and SaltStack for configuration management.

---

### 🛠️ Implemented Control Families

#### 🔑 Access Control (AC)
- Implemented role-based access control (RBAC) principles
- Enforced least privilege access across services and systems
- Managed authentication and system access boundaries

#### 📊 Audit & Accountability (AU)
- Deployed centralized logging using ELK Stack
- Collected and analyzed system and application logs
- Enabled visibility into user and system activity for monitoring and auditing

#### 🛡️ System & Communications Protection (SC)
- Implemented network segmentation concepts using virtualized environments
- Controlled traffic flow and secured communication channels
- Applied firewall and access boundary principles

#### 🔒 Configuration Management (CM)
- Utilized SaltStack for automated configuration management
- Established consistent system baselines
- Enabled repeatable and scalable infrastructure deployment

#### 🚨 Incident Response (IR)
- Established monitoring capabilities to detect suspicious behavior
- Enabled log-based investigation and response workflows

---

### 🎯 Key Outcome

This project showcases practical application of NIST-aligned security controls in a lab-based environment, focusing on security monitoring, configuration management, and audit readiness.

It bridges the gap between theoretical security frameworks and real-world implementation using modern cloud and infrastructure tools.

## 🏗️ Project Structure

```
enterprise-IT-audit-control-assurance/
│
├── 00_program-management/
├── 01_audit-planning/
├── 02_entity-understanding/
├── 03_risk-assessment/
├── 04_control-framework/
├── 05_control-testing/
├── 06_evidence-and-validation/
├── 07_findings-management/
├── 08_reporting/
```

---

## 🔍 Audit Scope

The audit covers:

* Identity and Access Management (IAM)
* Network Security Controls
* Vulnerability and Patch Management
* Security Monitoring and Logging
* Change and Configuration Management

---

## ⚠️ Key Risks Identified

* Unauthorized access due to weak access controls
* Excessive user privileges
* Delayed user deprovisioning
* Inconsistent patch management
* Insufficient logging and monitoring

---

## 🛡️ Control Areas Evaluated

* Multi-Factor Authentication (MFA)
* Role-Based Access Control (RBAC)
* Privileged Access Management
* Centralized Logging (SIEM)
* Firewall and Network Segmentation
* Patch Management Processes

---

## 🧪 Audit Approach

The audit was conducted using a structured methodology:

1. Audit Planning
2. Entity Understanding
3. Risk Assessment
4. Control Framework Development
5. Control Testing (ToD & ToE)
6. Findings and Risk Analysis
7. Reporting and Recommendations

---

## 📊 Key Findings Summary

| Finding                     | Risk Level | Description                          |
| --------------------------- | ---------- | ------------------------------------ |
| Delayed User Deprovisioning | High       | Access not removed promptly          |
| Excessive Permissions       | Medium     | Users have more access than required |
| Patch Management Gaps       | Medium     | Systems not updated on time          |

---

## 📈 Outcome

* Identified control gaps and risks
* Provided actionable remediation recommendations
* Delivered an executive-level audit report
* Demonstrated a complete enterprise audit lifecycle

---

## 🚀 Value of This Project

This project reflects real-world capabilities in:

* IT Audit & Assurance
* Risk Management
* Control Evaluation
* Governance and Compliance

### 🏗️ Enterprise Architecture

```mermaid
flowchart LR
User --> Endpoint
Endpoint --> AD[Active Directory]
Endpoint --> AzureAD[Cloud Identity]
AD --> Apps
AzureAD --> Apps
Apps --> DB[(Database)]
Apps --> Logs
Logs --> SIEM



