# Business Continuity and Disaster Recovery Plan
* Version: v1.1
* Date of version: 2024-04
* Author: Information Security Officer
* Approver: CTO
* Confidentiality: Internal use. Shared upon request as part of a due diligence

We have monitoring, alarms and procedures set up
Monitoring: service health tools, ping-monitoring connected to alerts if the system goes down or if performance of any component is low
On-call protocol: 24x7, to address and rectify any issues promptly
Disaster recovery protocol in case the whole datacenter goes down and we are able to replicate our full environment in a matter of minutes.
We are currently working on establishing a geo-redundant, load-balanced, high-availability cluster so the eventual downtime in case of a disaster is minimized even further


ess Continuity and Disaster Recovery Plan

1. Introduction 1.1 Purpose
The purpose of this document is to outline the business continuity and disaster recovery (BCDR) plan for Ecostars ESG AI. This plan ensures that critical business functions can continue and recover effectively in the event of an incident, in compliance with SOC 2, ISO 27001, and other relevant security frameworks.

### 1.2 Scope
This plan applies to all business units, employees, and systems critical to the operation of Ecostars ESG AI. It covers potential disruptions such as natural disasters, cyberattacks, infrastructure failures, and other unforeseen events.

### 1.3 Objectives

    Minimize the impact of disruptions on business operations.

    Ensure the safety of employees and assets.

    Maintain compliance with legal and regulatory requirements.

    Restore critical systems within the defined recovery time objectives (RTOs) and recovery point objectives (RPOs).

2. Business Impact Analysis (BIA) 2.1 Identification of Critical Functions

    Customer-facing applications

    Cloud infrastructure and databases

    Internal communication systems

    Third-party dependencies

### 2.2 Risk Assessment

    Cyber threats (e.g., ransomware, DDoS attacks)

    Natural disasters (e.g., earthquakes, floods)

    Infrastructure failures (e.g., data center outages, power loss)

    Insider threats (e.g., employee sabotage, human error)

### 2.3 Recovery Prioritization

    High-priority systems: Recovery within 4 hours

    Medium-priority systems: Recovery within 24 hours

    Low-priority systems: Recovery within 72 hours

3. Business Continuity Plan (BCP) 3.1 Prevention Measures

    Regular security audits and penetration testing

    Employee training on security best practices

    Redundant infrastructure for key services

### 3.2 Communication Plan

    Internal notification system for employees

    External communication strategy for customers and stakeholders

    Media response guidelines

### 3.3 Alternate Work Arrangements

    Remote work capabilities

    Temporary office locations

    Secure VPN access for employees

4. Disaster Recovery Plan (DRP) 4.1 Incident Response Procedures

    Detection and initial response

    Containment and mitigation

    Incident classification and escalation

### 4.2 System Recovery Procedures

    Restoration of critical applications from backups

    Verification and integrity checks

    User access revalidation

### 4.3 Backup Strategy

    Daily incremental and weekly full backups

    Offsite and cloud-based backup storage

    Periodic backup testing and validation

### 4.4 Testing and Drills

    Annual full-scale disaster recovery testing

    Quarterly tabletop exercises

    Post-mortem analysis and continuous improvement

## 5. Roles and Responsibilities
### 5.1 Business Continuity Team

    Chief Technology Officer (CTO): Oversees BCDR plan implementation

    Security Officer: Manages compliance and risk assessment

    IT Infrastructure Lead: Ensures system resilience and backup procedures

    HR & Operations: Coordinates employee safety and communication

### 5.2 Contact Information

    Emergency IT Support: [Contact Details]

    Data Center Operations: [Contact Details]

    Crisis Management Team: [Contact Details]

6. Compliance and Review 6.1 Regulatory Compliance

    SOC 2, ISO 27001, GDPR, and other applicable standards

    Legal and industry-specific requirements

### 6.2 Plan Review and Updates

    Reviewed bi-annually or after major incidents

    Updates documented and communicated to all stakeholders

7. Conclusion This Business Continuity and Disaster Recovery Plan is essential for ensuring the resilience and security of Ecostars ESG AI. All employees must familiarize themselves with the procedures outlined in this document to ensure preparedness for potential disruptions.



