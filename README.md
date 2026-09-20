SOC Incident Case Studies

A collection of SOC investigation scenarios from my cybersecurity labs and security monitoring practice.

The case files show how I work through an alert, review the evidence and decide whether further investigation or escalation is needed.

---

Case Studies

Case 01 — Repeated SSH Failures

Reviewing repeated SSH authentication failures, including source IP, affected host, timestamps and surrounding authentication activity.

Case 02 — Successful Login After SSH Failures

Investigating a successful SSH login that occurred after repeated authentication failures.

Case 03 — Suricata Login Alert

Investigation of repeated login requests against OWASP Juice Shop using Suricata and Splunk.

Detection used in the lab:

POST /rest/user/login

Threshold: 5 attempts within 30 seconds

Case 04 — Entra ID Sign-In Failure

Reviewing failed Microsoft Entra ID sign-ins, error information, source IPs and surrounding authentication activity.

Case 05 — Suspicious IP

Searching logs for additional activity associated with a suspicious IP and reviewing whether escalation or containment is required.

---

My Investigation Approach

Alert
↓
Triage
↓
Review logs and evidence
↓
Check related activity
↓
Document findings
↓
Escalate or contain if required
↓
Close

I normally look at the user, host, source IP, timestamps, authentication results and related events before making a decision.

---

Lab Tools

- Microsoft Sentinel
- KQL
- Microsoft Entra ID
- Kali Linux
- Suricata
- Splunk
- Syslog
- OWASP Juice Shop

---

Case Files

- case-01-repeated-ssh-failures.md
- case-02-success-after-ssh-failures.md
- case-03-suricata-login-alert.md
- case-04-entra-signin-failure.md
- case-05-suspicious-ip.md
- incident-investigation-template.md

---

These are lab-based investigations and study exercises, not production SOC incidents.

Progress still ongoing.
