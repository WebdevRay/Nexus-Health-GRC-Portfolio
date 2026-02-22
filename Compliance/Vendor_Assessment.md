# Vendor Security Assessment: CloudStorage Pro

**Assessor:** Ray A. Price  
**Status:** Under Review  
**Criticality:** High (Sub-processor of Patient Data)

## 1. Executive Summary
This assessment evaluates **CloudStorage Pro** as a potential vendor for offsite HIPAA-compliant backups. Our primary concern is ensuring their uptime aligns with our **99.9% Service Availability** requirement.

## 2. Security & Compliance Review
| Requirement | Status | Observations |
| :--- | :--- | :--- |
| **HIPAA Compliance** | Pass | Provided signed BAA and SOC 2 Type II Report. |
| **Data Encryption** | Pass | AES-256 at rest; TLS 1.2 in transit. |
| **Availability (SLA)** | **Fail** | Vendor only guarantees 99.0% uptime (Nexus requires 99.9%). |

## 3. Disaster Recovery (The "Nightmare" Check)
* **RTO (Recovery Time Objective):** 4 Hours.
* **RPO (Recovery Point Objective):** 24 Hours.
* **Geographic Redundancy:** Vendor only operates in a single AWS region.

## 4. Assessor Recommendation: **CONDITIONAL APPROVAL**
The vendor meets privacy standards but poses a significant risk to **Service Availability**. 

**Required Compensating Control:** Nexus Health AI must not use CloudStorage Pro as the *sole* backup provider. We must maintain a secondary backup in a different cloud region (e.g., Azure or a different AWS region) to mitigate the vendor's 1% downtime risk.
