# Data Flow: Patient Scan Analysis
## Ingestion: Doctor uploads scan to Web Portal (HTTPS/TLS 1.2).

## Processing: API Gateway routes data to the Nexus-Core AI in AWS.

## Storage: Analysis results are written to the Patient Health DB.

## Delivery: Encrypted results are pulled by the Oncology Dashboard for review.
