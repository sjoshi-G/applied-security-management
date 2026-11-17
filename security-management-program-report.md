# Applied Security Management Program — Industry Case: University Systems
By Shiwani Joshi — Cybersecurity Certificate coursework, Georgian College
## 1. Executive Summary
- A university operates a complex digital ecosystem supporting academic, administrative, and financial processes. With over 15,000 students and 1,200 staff, the institution relies heavily on the Student Information System (SIS), Learning Management System (LMS), and online examination platforms. These systems process highly sensitive data, including personally identifiable information (PII), academic records, and financial transactions.
- This program identifies critical vulnerabilities in the infrastructure, including the absence of multi-factor authentication (MFA), weak access control mechanisms, and insufficient monitoring capabilities. These weaknesses significantly increase the risk of data breaches, insider threats, and ransomware attacks.
- The proposed strategy is grounded in governance, risk assessment, and layered security controls. Key initiatives: implementing MFA, deploying a SIEM system, enforcing role-based access control (RBAC), and establishing a structured incident response framework. The program follows a phased roadmap across four quarters. Metrics such as Mean Time to Detect (MTTD), incident response time, and MFA adoption rate measure effectiveness.
## 2. Organization Context & Assumptions
**Core systems**: SIS (student records, grades, enrollment), LMS (course materials and assignments), online examination platform (remote assessments), email & identity management system (authentication and communication)
**Data classification**: Confidential (student records, grades, financial information), Internal (staff communications, internal documents), Public (course descriptions, public announcements)
**Constraints**: limited cybersecurity staffing, budget limitations, legacy systems lacking modern controls, high availability requirements during exam periods
## 3. Security Management Goals & Objectives
**Goal**: ensure the confidentiality, integrity, and availability (CIA) of university systems and data while minimizing operational disruption
**Risk tolerance:** low tolerance for data breaches involving PII and academic records; moderate tolerance for system downtime under two hours during non-critical periods
**Objectives:** 
- (1) reduce unauthorized access through strong authentication;
- (2) ensure system availability, especially during exams;
- (3) detect and respond to incidents within 15 minutes;
- (4) secure sensitive data through encryption and access controls;
- (5) improve staff and student security awareness
## 4. Governance: Roles, Responsibilities, and Escalation
- **CISO**: defines strategy, oversees the security program
- **IT Security Team:** implements controls, monitors systems
- **System Administrators:** maintain systems, enforce configurations
- **Incident Response Team:** handles security incidents
- **Help Desk:** first point of contact for user-reported issues
- **Responsibility allocation:** access control — IT Admin + Security Team; monitoring — Security Operations; incident handling — Incident Response Team; policy enforcement — CISO.
**Escalation path:** Help Desk → IT Security → CISO → Executive Leadership.
## 5. Threat–Vulnerability–Asset (TVA) Analysis
- **Key asset:** Student Information System (SIS) — most critical due to its sensitive data.
- **Threats:** external data breaches, insider misuse, ransomware, unauthorized access, phishing
- **Vulnerabilities:** weak password policies, absence of MFA, excessive user privileges, lack of encryption, insufficient monitoring
- **CIA impact:** Confidentiality — high (PII exposure); Integrity — high (grade manipulation); Availability — critical (downtime disrupts operations and exams)
## 6. Ranked Vulnerability Risk Assessment
**Methodology**: Likelihood (1–5) × Impact (1–5).
- Vulnerability
- Risk
- No MFA
- Critical
- Weak passwords
- High
- Excessive privileges
- High
- Lack of logging
- High
- No encryption
- High
**Justification**: no MFA is highly exploitable through credential theft; no logging prevents detection and investigation; excess privileges enable insider threats.
## 7. Risk Control Strategies & Treatment Plan
**Strategies**: Mitigate (reduce likelihood/impact), Avoid (eliminate), Transfer (e.g., cyber insurance), Accept (acknowledge low risk).
- Risk
- Treatment
- Control
- Owner / Timing
- No MFA
- Mitigate
- Deploy MFA
- IT Security, Q2
- Excess privileges
- Mitigate
- RBAC
- Admins, Q3
- No logging
- Mitigate
- SIEM deployment
- Security Team, Q2
- Weak passwords
- Mitigate
- Policy enforcement
- Q2
- Residual risk
- Transfer
- Cyber insurance
## 8. Intrusion Detection & Monitoring Plan
- Objectives: identify unauthorized access, detect abnormal behavior, prevent data exfiltration
- Monitoring use cases: multiple failed logins, privilege escalation events, large data transfers, suspicious IP activity
- Tools: SIEM, intrusion detection systems (IDS), log aggregation platforms
- Triage: analysts review alerts, classify severity, and escalate accordingly (Alert → Triage → Escalate → Contain)
## 9. Breach Response Plan
- Activation criteria: confirmed unauthorized access, data exfiltration detected, system compromise identified
- Phases: 1. Identification 2. Containment 3. Eradication 4. Recovery 5. Lessons learned
- Communication: internal (IT, management); external (students, regulators)
- Evidence handling: log preservation, system snapshots, forensic analysis
## 10. CVE-Based Vulnerability Management
- CVE-2021-44228 (Log4Shell) — remote code execution in logging libraries; risk of full system compromise
- CVE-2023-23397 — email system exploit requiring no user interaction; enables credential theft
- CVE-2022-22965 (Spring4Shell) — affects web applications like LMS/SIS; allows remote execution
- Prioritization: Critical CVEs — patch immediately; High — patch within 7 days; Medium — scheduled updates. CVE severity feeds risk ranking, patch prioritization, and resource allocation.
## 11. Strategic Roadmap & Metrics
- Q1: asset inventory, logging baseline
- Q2: MFA implementation, password policy enforcement
- Q3: access control improvements, data encryption
- Q4: security audit, policy refinement
- Metrics (KPI/KRI): MTTD, MTTR, MFA adoption rate (target >90%), patch compliance rate (target >95%), number of incidents. Metrics enable ongoing evaluation and continuous improvement.
## 12. Conclusion
This program provides a structured, realistic approach to managing cybersecurity risk: governance, risk assessment, technical controls, and continuous monitoring combined in a phased roadmap, with CVE-based vulnerability management aligning it to real-world threats. It safeguards the university's systems and users while ensuring operational continuity.
## 13. References
- NIST Cybersecurity Framework
- ISO/IEC 27001
- OWASP Top 10
- CISA Cybersecurity Guidelines
- SANS Institute Resources
- ENISA Threat Landscape Report
