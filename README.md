# Botium-Toys-Internal-Security-Audit

# Table of contents

1. [Introduction](#introduction)
2. [Scenario](#scenario)
3. [Scope & Goals](#scope-&-goals)
4. [Risk Assessment Report](#risk-assessment-report)
5. [Controls Assessment Checklist](#controls-assessment-checklist)
6. [Compliance Checklist](#compliance-checklist)

-------

# Introduction <a name="introduction">

An internal security audit for Botium Toys, a fictional company, completed for the Google Cybersecurity Professional Certificate. It evaluates the company’s cybersecurity program, identifies high-risk issues, and recommends strategies to strengthen its security posture.

An internal security audit for Botium Toys, a fictional toy company, completed as part of my cybersecurity portfolio and as part of Google's <a href='https://www.coursera.org/google-certificates/cybersecurity-certificate'>Cybersecurity Professional Certificate</a> on Coursera in the  <a href='https://www.coursera.org/learn/manage-security-risks?specialization=cybersecurity-certificate'> Play It Safe: Manage Security Risks </a> Course .
   
The goal is to perform an audit of Botium Toys’ cybersecurity program. The audit needs
to align current business practices with industry standards and best practices. The
audit is meant to provide mitigation recommendations for vulnerabilities found that are
classified as “high risk,” and present an overall strategy for improving the security
posture of the organization. The audit team needs to document their findings, provide
remediation plans and efforts, and communicate with stakeholders.

# Scenario  <a name="scenario">
Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse for their products. However, Botium Toy’s online presence has grown, attracting customers in the U.S. and abroad. As a result, their information technology (IT) department is under increasing pressure to support their online market worldwide. 

The manager of the IT department has decided that an internal IT audit needs to be conducted. She's worried about maintaining compliance and business operations as the company grows without a clear plan. She believes an internal audit can help better secure the company’s infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to internally processing and accepting online payments and conducting business in the European Union (E.U.). 

The IT manager starts by implementing the **National Institute of Standards and Technology Cybersecurity Framework** (NIST CSF), establishing an audit scope and goals, listing assets currently managed by the IT department, and completing a risk assessment. The goal of the audit is to provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.

# Scope & Goals  <a name="scope-&-goals">

**Scope**: The scope of this audit is defined as the entire security program at Botium Toys.
This includes their assets like employee equipment and devices, their internal network,
and their systems. You will need to review the assets Botium Toys has and the controls
and compliance practices they have in place.

**Goals**: Assess existing assets and complete the controls and compliance checklist to
determine which controls and compliance best practices that need to be implemented
to improve Botium Toys’ security posture.

------------------------

Risk  Assessment Report  <a name="risk-assessment-report">
===================

Current Assets 
--------------

Assets managed by the IT Department include:
- On-premises equipment for in-office business needs
- Employee equipment: end-user devices (desktops/laptops, smartphones),
remote workstations, headsets, cables, keyboards, mice, docking stations,
surveillance cameras, etc.
- Storefront products available for retail sale on site and online; stored in the
company’s adjoining warehouse
- Management of systems, software, and services: accounting,
telecommunication, database, security, ecommerce, and inventory management
- Internet access
- Internal network
- Data retention and storage
- Legacy system maintenance: end-of-life systems that require human monitoring

Additional Comments 
--------------
The potential impact from the loss of an asset is rated as medium, because the IT
department does not know which assets would be at risk. The risk to assets or fines
from governing bodies is high because Botium Toys does not have all of the necessary
controls in place and is not fully adhering to best practices related to compliance
regulations that keep critical data private/secure. Review the following bullet points for
specific details:
- Currently, all Botium Toys employees have access to internally stored data and
may be able to access cardholder data and customers’ PII/SPII.
- Encryption is not currently used to ensure confidentiality of customers’ credit
card information that is accepted, processed, transmitted, and stored locally in
the company’s internal database.
- Access controls pertaining to least privilege and separation of duties have not
been implemented.
- The IT department has ensured availability and integrated controls to ensure
data integrity.
- The IT department has a firewall that blocks traffic based on an appropriately
defined set of security rules.
- Antivirus software is installed and monitored regularly by the IT department.
- The IT department has not installed an intrusion detection system (IDS).
- There are no disaster recovery plans currently in place, and the company does
not have backups of critical data.
- The IT department has established a plan to notify E.U. customers within 72
hours if there is a security breach. Additionally, privacy policies, procedures, and
processes have been developed and are enforced among IT department
members/other employees, to properly document and maintain data.
- Although a password policy exists, its requirements are nominal and not in line
with current minimum password complexity requirements (e.g., at least eight
characters, a combination of letters and at least one number; special
characters).
- There is no centralized password management system that enforces the
password policy’s minimum requirements, which sometimes affects productivity
when employees/vendors submit a ticket to the IT department to recover or
reset a password.
- While legacy systems are monitored and maintained, there is no regular
schedule in place for these tasks and intervention methods are unclear.
- The store’s physical location, which includes Botium Toys’ main offices, store
front, and warehouse of products, has sufficient locks, up-to-date closed-circuit
television (CCTV) surveillance, as well as functioning fire detection and
prevention systems.

### Administrative Controls 
| Control Name | Control type and explanation | Needs to be implemented (X) | Priority |
| --- | --- | --- | --- |
| Least Privilege | Preventative; reduces risk by making sure vendors and non-authorized staff only have access to the assets/data they need to do their jobs | X | High |
| Disaster recovery plans | Corrective; business continuity to ensure systems are able to run in the event of an incident/there is limited to no loss of productivity downtime/impact to system components, including: computer room environment (air conditioning, power supply, etc.); hardware (servers, employee equipment); connectivity (internal network, wireless); applications (email, electronic data); data and restoration | X | High |
| Password policies | Preventative; establish password strength rules to improve security/reduce likelihood of account compromise through brute force or dictionary attack techniques | X | High |
| Access control policies | Preventative; increase confidentiality and integrity of data | X | High |
| Account management policies | Preventative; reduce attack surface and limit overall impact from disgruntled/former employees | X | High |
| Separation of duties | Preventative; ensure no one has so much access that they can abuse the system for personal gain | X | High |

### Technical Controls 
| Control Name | Control type and explanation | Needs to be implemented (X) | Priority |
| --- | --- | --- | --- |
| Firewall | Preventative; firewalls ***are already in place*** to filter unwanted/malicious traffic from entering internal network | NA | NA |
| Intrusion Detection System (IDS) | Detective; allows IT team to identify possible intrusions (e.g., anomalous traffic) quickly | X | High |
| Encryption | Deterrent; makes confidential information/data more secure (e.g., website payment transactions) | X | High |
| Backups | Corrective; supports ongoing productivity in the case of an event; aligns to the disaster recovery plan | X | High |
| Password management system | Corrective; password recovery, reset, lock out notifications | X | High |
| Antivirus (AV) software | Corrective; detect and quarantine known threats | X | High |
| Manual monitoring, maintenance, and intervention | Preventative/corrective; required for legacy systems to identify and mitigate potential threats, risks, and vulnerabilities | X | High |


### Physical Controls
| Control Name | Control type and explanation | Needs to be implemented (X) | Priority |
| --- | --- | --- | --- |
| Time-controlled safe | Deterrent; reduce attack surface/impact of physical threats | X | Medium/Low |
| Adequate lighting | Deterrent; limit “hiding” places to deter threats | X | Medium/Low |
| Closed-circuit television (CCTV) surveillance | Preventative/detective; can reduce risk of certain events; can be used after event for investigation | X | High/Medium |
| Locking cabinets (for network gear) | Preventative; increase integrity by preventing unauthorized personnel/individuals from physically accessing/modifying network infrastructure gear | X | High/Medium |
| Signage indicating alarm service provider | Deterrent; makes the likelihood of a successful attack seem low | X | Low |
| Locks | Preventative; physical and digital assets are more secure | X | High |
| Fire detection and prevention (fire alarm, sprinkler system, etc.) | Detective/Preventative; detect fire in the toy store’s physical location to prevent damage to inventory, servers, etc. | X | Medium |

------------------------

Controls Assessment Checklist  <a name="controls-assessment-checklist">
===================

Question: Does Botium Toys currently have this
control in place?

| Yes | No | Control |
| --- | --- | --- |
|  | X | Least Privilege
|  | X | Disaster recovery plans
|  | X | Password policies
|  | X | Separation of duties
| X |  | Firewall
|  | X | Intrusion detection system (IDS)
|  | X | Backups
| X |  | Antivirus software
|  | X | Manual monitoring, maintenance, and intervention for legacy systems
|  | X | Encryption
|  | X | Password management system
| X |  | Locks (offices, storefront, warehouse)
| X |  | Closed-circuit television (CCTV) surveillance
| X |  | Fire detection/prevention (fire alarm, sprinkler system, etc.)

------------------------

Compliance checklist
====================

Question: Does Botium Toys currently adhere
to this compliance best practice?

### Payment Card Industry Data Security Standard (PCI DSS)
| Yes | No | Best Practice |
| --- | --- | --- |
|  | X | Only authorized users have access to customers’ credit card information.
|  | X | Credit card information is accepted, processed, transmitted, and stored internally, in a secure environment.
|  | X | Implement data encryption procedures to better secure credit card transaction touchpoints and data.
|  | X | Adopt secure password management policies.

### General Data Protection Regulation (GDPR)
| Yes | No | Best Practice |
| --- | --- | --- |
|  | X | E.U. customers’ data is kept private/secured.
| X |  | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach.
|  | X | Ensure data is properly classified and inventoried.
| X |  | Enforce privacy policies, procedures, and processes to properly document and maintain data.

### System and Organizations Controls (SOC type 1, SOC type 2)
| Yes | No | Best Practice |
| --- | --- | --- |
|  | X | User access policies are established.
|  | X | Sensitive data (PII/SPII) is confidential/private.
| X |  | Data integrity ensures the data is consistent, complete, accurate, and has been validated.
|  | X | Data is available to individuals authorized to access it.

----------------
