# Asset Inventory: Nexus Health AI

| Asset ID | Asset Name | Category | Criticality | Data Type |
| :--- | :--- | :--- | :--- | :--- |
| **ASSET-01** | Nexus-Core AI Engine | Software | **Critical** | Proprietary Logic |
| **ASSET-02** | Patient Health DB (AWS RDS) | Data | **Critical** | PHI / PII |
| **ASSET-03** | Engineer Workstations | Hardware | **Medium** | Internal Specs |
| **ASSET-04** | GitHub Repository | Software | **High** | Source Code |
| **ASSET-05** | AWS S3 Backups | Data | **High** | PHI / Backups |

### Asset Criticality Legend
* **Critical:** Failure causes a total shutdown of the AI service or a breach of PHI (Protected Health Information).
* **High:** Failure significantly degrades service or affects multiple departments/security backups.
* **Medium:** Failure affects individual productivity but does not stop the service or risk data privacy.
* **Low:** Non-essential assets with no impact on security or availability.

# Data Flow: Patient Scan Analysis
## Ingestion: Doctor uploads scan to Web Portal (HTTPS/TLS 1.2).

## Processing: API Gateway routes data to the Nexus-Core AI in AWS.

## Storage: Analysis results are written to the Patient Health DB.

## Delivery: Encrypted results are pulled by the Oncology Dashboard for review.
