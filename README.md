# Applied Security Management Program — University Systems
By Shiwani Joshi — coursework project completed during my Cybersecurity Certificate at Georgian College.
## What this is
A complete security management program designed for a mid-sized university (15,000 students, 1,200 staff) whose core systems — Student Information System (SIS), Learning Management System (LMS), online examination platform, and email/identity systems — process sensitive PII, academic records, and financial data.
The program is aligned with NIST CSF, ISO/IEC 27001, and OWASP guidance.
## What the program covers
**Governance**  — CISO / security team / sysadmin / incident response roles, responsibility allocation, and an escalation path (Help Desk → IT Security → CISO → Executive Leadership)
**Threat–Vulnerability–Asset (TVA) analysis** of the SIS, the institution's most critical asset
**Ranked risk assessment** (likelihood × impact). Top risks found:
No MFA — Critical
Weak password policies — High
Excessive user privileges — High
Lack of logging/monitoring — High
No encryption — High
**Risk treatment plan** — MFA deployment, role-based access control (RBAC), encryption, and SIEM monitoring, with owners and quarters assigned
**Detection & monitoring plan** — SOC use cases: multiple failed logins, privilege escalation, large data transfers, suspicious IP activity; SIEM + IDS tooling and an alert triage process
**Breach response plan** — identification, containment, eradication, recovery, lessons learned, plus internal/external communication and evidence handling
**CVE-based vulnerability management** — prioritization using real CVEs (Log4Shell CVE-2021-44228, CVE-2023-23397, Spring4Shell CVE-2022-22965) with patch SLAs by severity
**Phased roadmap (Q1–Q4) and metrics:** MTTD, MTTR, MFA adoption rate, patch compliance rate, incident counts
## Files in this repo
security-management-program-report.md — the full report in markdown
Report.docx — the full report document
## Skills demonstrated
Risk assessment (TVA), security governance, access control design (MFA, RBAC), SIEM monitoring use cases, incident response planning, vulnerability management and CVE prioritization, security metrics (KPI/KRI).
