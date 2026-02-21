# Risk Register
|:--- |:--- |:---|:--- |:---|:---|
|Threat	| Impact (1-5)	| Likelihood (1-5)	| Inherent Risk Score	| Mitigation Control (The Safety Net)	| Residual Risk Score
Failed Code Deployment	5	4	20	Change Management Policy (Peer Reviews & Testing)	5
Regional AWS Outage	5	2	10	Multi-Region Architecture (Failover to a 2nd region)	5
Ransomware Attack	4	3	12	Daily Immutable Backups & Mandatory MFA	4
DDoS Attack	4	3	12	AWS Shield & Web Application Firewall (WAF)	4
Unauthorized Data Access	5	2	10	Encryption at Rest/Transit & Strict IAM Roles	2
