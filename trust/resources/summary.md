# Summary
* **Version**: v2.0
* **Date of version**: 2025-02
* **Author**: Information Security Officer
* **Approver**: CTO


## 1. Introduction
### 1.1 Purpose
This report documents the security, availability, processing integrity, confidentiality, and privacy controls implemented by Ecostars ESG AI in accordance with the AICPA’s Trust Services Criteria. The assessment period covers 2024-01 to 2025-02.

### 1.2 Scope
This report applies to all systems, processes, and data management policies governing Ecostars ESG AI’s operations, including:
- Cloud infrastructure and data centers
- Access control and authentication mechanisms
- Data management and retention policies
- Incident response and business continuity planning
- Compliance with regulatory standards (e.g., GDPR, ISO 27001)

### 1.3 System Description
- Ecostars ESG AI provides ESG-focused digital solutions with a strong commitment to security and compliance.
- Infrastructure is hosted in EU-based Microsoft Azure data centers (West Europe - Amsterdam), with planned geo-redundancy expansion, Google Cloud Platform or Amazon Web Services, always within EU-based, compliant data centers.
- Cloud services are configured with automated backup, encryption, and secure access controls.
- Data access follows a strict Role-Based Access Control (RBAC) model with Multi-Factor Authentication (MFA).
- Single Sign-On (SSO) is enabled via SAML2, OAuth2, and OpenID Connect.

## 2. Trust Services Criteria and Controls
### 2.1 Security
- Implementation of Role-Based Access Control (RBAC) to enforce least privilege access.
- Multi-Factor Authentication (MFA) for all critical systems.
- Network security measures including firewalls, intrusion detection systems, and regular penetration testing.
- Automated monitoring and logging of security events.

### 2.2 Availability
- 99.9% uptime SLA for customer-facing applications.
- High-availability architecture with load balancing and failover mechanisms.
- Regular data backups stored in secure Azure Blob Storage.

### 2.3 Processing Integrity
- Secure software development lifecycle (SDLC) with automated security testing.
- Data validation and integrity checks implemented in all systems.
- API rate limiting to prevent abuse and ensure stable performance.

### 2.4 Confidentiality
- Encryption of data at rest (AES-256) and in transit (TLS 1.2+).
- Confidential data access is logged and monitored for anomalies.
- Third-party data sharing governed by Data Processing Agreements (DPA).

### 2.5 Privacy
- Compliance with GDPR and ISO 27001 for data privacy and protection.
- User data is anonymized where possible and securely stored.
- Regular audits ensure compliance with privacy obligations.

## 3. Risk Management and Incident Response
### 3.1 Risk Management
- Periodic risk assessments conducted to identify and mitigate security threats.
- Security awareness training for all employees.
- Formal policies in place for vulnerability management and remediation.

### 3.2 Incident Response
- Dedicated incident response team responsible for investigating security incidents.
- Defined escalation procedures for critical events.
- Incident logs and reports maintained for compliance review.

## 4. Business Continuity and Disaster Recovery
### 4.1 Business Continuity
- Redundant systems and data replication for continuity.
- Emergency response plans documented and tested regularly.

### 4.2 Disaster Recovery
- Recovery Time Objectives (RTO) and Recovery Point Objectives (RPO) defined for all systems.
- Encrypted offsite backups ensure rapid recovery.

## 5. Compliance and Auditing
### 5.1 Compliance Standards
- Aligned with SOC 2, ISO 27001, and GDPR frameworks.
- Align with OWASP and 12 Factor app methodologies and recommendations.
- Regular audits conducted to maintain compliance and identify areas for improvement.

### 5.2 Audit Results
- This assessment confirms that Ecostars ESG AI has implemented effective security, availability, processing integrity, confidentiality, and privacy controls.
- No major deficiencies were identified during the audit period.

## 6. Conclusion
Ecostars ESG AI maintains a robust security posture aligned with SOC 2 Type II, ISO 27001 and GDPR requirements. The company remains committed to ongoing improvements, regulatory compliance, and the highest standards of security and privacy.

