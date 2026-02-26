# Security Audit

# Botium Toys Security Audit Project

##  Audit Scope

The scope of this audit covers the entire security program at Botium Toys, including:

- On-premises equipment  
- Employee devices  
- Internal network  
- Ecommerce systems  
- Data storage and retention  
- Legacy systems  

Step 1️ – Define Scope and Goals

- Reviewed the audit scope covering the entire security program
- Identified systems, networks, employee devices, and data storage
- Established audit goal: assess security controls and compliance gaps

**Purpose:** Clearly define what is being evaluated before assessing risk.

---

## Step 2️ – Identify and Classify Assets

- Reviewed managed assets (devices, internal network, ecommerce systems, databases)
- Evaluated potential impact of asset loss
- Identified lack of structured asset inventory and classification process

**Purpose:** Understand what needs protection before evaluating safeguards.

---

## Step 3️ – Assess Security Controls

Evaluated implementation of administrative, technical, and physical controls.

###  Administrative Controls
- Least Privilege → ❌ Not Implemented
- Separation of Duties → ❌ Not Implemented
- Password Policies → ⚠ Weak Enforcement
- Disaster Recovery Plan → ❌ Not Implemented

###  Technical Controls
- Firewall → ✅ Implemented
- Antivirus Software → ✅ Implemented
- Intrusion Detection System (IDS) → ❌ Not Implemented
- Encryption → ❌ Not Implemented
- Backups → ❌ Not Implemented
- Password Management System → ❌ Not Implemented

###  Physical Controls
- Locks → ✅ Implemented
- CCTV Surveillance → ✅ Implemented
- Fire Detection & Prevention Systems → ✅ Implemented

**Purpose:** Determine strengths and weaknesses across the CIA triad (Confidentiality, Integrity, Availability).

---

## Step 4 – Conduct Compliance Gap Analysis

Compared current practices against major regulatory frameworks:

### 💳 PCI DSS
Status: ❌ Not Compliant  
- No encryption for cardholder data  
- Overly broad internal access  
- Weak password policy enforcement  

### 🌍 GDPR
Status: ⚠ Partially Compliant  
- 72-hour breach notification plan in place  
- Privacy policies documented and enforced  
- Lacks encryption and structured data classification  

### 📊 SOC 1 / SOC 2
Status: ❌ Not Compliant  
- Integrity and availability controls present  
- Confidentiality and access control insufficient  

**Purpose:** Measure regulatory exposure and potential financial/legal risk.

---

## Step 5️ – Evaluate Risk Level

- Assigned qualitative risk score: **8/10 (High Risk)**
- Determined confidentiality as the most vulnerable security principle
- Identified high exposure due to missing preventive controls

**Purpose:** Quantify severity and organizational impact.

---

## Step 6️ – Develop Remediation Plan

Prioritized recommendations based on risk severity.

**Risk Score: 8/10 (High Risk)**

Primary issue: Lack of proper controls and incomplete compliance adherence.

---

# Control Categories

Controls are grouped into three primary categories:

## Administrative Controls
- Least Privilege  
- Disaster Recovery Plans  
- Password Policies  
- Separation of Duties  
- Access Control Policies  

## Technical Controls
- Firewall  
- Intrusion Detection System (IDS)  
- Encryption  
- Backups  
- Antivirus Software  
- Password Management System  
- Manual Monitoring of Legacy Systems  

## Physical Controls
- Locks  
- CCTV Surveillance  
- Fire Detection & Prevention Systems  

---

# Controls Assessment Checklist

| Control | Yes | No |
|----------|-----|----|
| Least Privilege |  | ✅ |
| Disaster Recovery Plans |  | ✅ |
| Password Policies (exists but weak) | ✅ |  |
| Separation of Duties |  | ✅ |
| Firewall | ✅ |  |
| Intrusion Detection System (IDS) |  | ✅ |
| Backups |  | ✅ |
| Antivirus Software | ✅ |  |
| Manual Monitoring of Legacy Systems (informal) | ✅ |  |
| Encryption |  | ✅ |
| Password Management System |  | ✅ |
| Locks (Offices, Storefront, Warehouse) | ✅ |  |
| CCTV Surveillance | ✅ |  |
| Fire Detection/Prevention Systems | ✅ |  |

## Observations:
- Integrity and availability controls are partially implemented.
- Confidentiality controls are weak due to lack of encryption and unrestricted internal access.

---

# 📋 Compliance Checklist

## 💳 PCI DSS

| Best Practice | Yes | No |
|---------------|-----|----|
| Only authorized users have access to credit card data |  | ✅ |
| Credit card data processed in secure environment |  | ✅ |
| Encryption implemented for cardholder data |  | ✅ |
| Secure password management policies enforced |  | ✅ |



---

## 🌍 GDPR

| Best Practice | Yes | No |
|---------------|-----|----|
| E.U. customer data kept private/secure |  | ✅ |
| 72-hour breach notification plan | ✅ |  |
| Data properly classified and inventoried |  | ✅ |
| Privacy policies documented and enforced | ✅ |  |


---

## 📊 SOC 1 & SOC 2

| Best Practice | Yes | No |
|---------------|-----|----|
| User access policies established |  | ✅ |
| Sensitive data confidential/private |  | ✅ |
| Data integrity validated | ✅ |  |
| Data available to authorized users | ✅ |  |



---

#  Key Security Gaps Identified

- No encryption for stored cardholder data  
- No disaster recovery plan  
- No backups of critical data  
- No intrusion detection system  
- No least privilege enforcement  
- Weak password complexity enforcement  
- No centralized password management system  

---

#  Recommendations

## High Priority
- Implement encryption for all sensitive data
- Enforce least privilege access control
- Deploy IDS
- Establish disaster recovery plan
- Implement centralized password management system
- Restrict cardholder data access

## Medium Priority
- Formalize legacy system monitoring schedule
- Strengthen password complexity requirements
- Implement structured asset inventory and classification program

---

# Skills Demonstrated

- Risk assessment analysis  
- Control categorization  
- Compliance gap identification  
- Security documentation  
- Application of NIST CSF Identify function  
- PCI DSS, GDPR, and SOC framework comparison  
