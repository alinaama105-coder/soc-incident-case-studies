SOC Incident Case Studies

SOC investigation case studies based on my cybersecurity labs and security monitoring practice.

The cases document how I approach alerts from initial triage through investigation, escalation, containment and closure.

---

Investigation Process

Alert
↓
Initial Triage
↓
Review Evidence
↓
Investigate Activity
↓
Determine Risk
↓
Escalate or Contain
↓
Document and Close

---

Case Studies

Case 01 — Repeated SSH Authentication Failures

Multiple failed SSH login attempts are detected against a Linux system.

Investigation includes:

- Source IP
- Target host
- Timestamp
- Number of attempts
- Authentication logs
- Related activity

---

Case 02 — Successful SSH Login After Failures

A successful SSH authentication occurs following repeated failed attempts.

Investigation includes:

- Previous failed attempts
- Source IP comparison
- Username
- Target system
- Timing between events
- Additional activity after authentication

This type of sequence was used during my Microsoft Sentinel lab.

---

Case 03 — Suricata Web Login Alert

Suricata detects repeated login requests against the OWASP Juice Shop lab.

Lab detection:

POST /rest/user/login

Threshold:

5 attempts within 30 seconds

Investigation includes:

- Source address
- HTTP request
- Timestamp
- Alert signature
- Suricata event data
- Related events in Splunk

---

Case 04 — Microsoft Entra ID Sign-In Failure

A failed sign-in is identified in Microsoft Entra ID logs.

Investigation includes:

- User account
- Sign-in result
- Timestamp
- Source IP
- Error code
- Previous failures
- Successful sign-ins
- Account status

My Entra ID practice included reviewing successful and failed sign-ins and account lockout behaviour.

---

Case 05 — Suspicious IP Investigation

A suspicious IP address is identified during log analysis.

Investigation includes:

- Search for additional events from the IP
- Systems contacted
- Authentication attempts
- Event frequency
- Successful activity
- Watchlist comparison
- Possible containment requirements

During my Sentinel practice I created a watchlist called:

Malicious SSH IPs

---

Triage Questions

When reviewing an alert I ask:

- What triggered the alert?
- Which system is affected?
- Which user is involved?
- What is the source IP?
- When did the activity begin?
- Is the activity repeated?
- Was authentication successful?
- Is there related activity?
- Is the behaviour expected?
- Does the incident require escalation?

---

Evidence

Evidence may include:

- SIEM logs
- Syslog
- Authentication logs
- Source and destination IPs
- User accounts
- Hostnames
- Timestamps
- Suricata alerts
- Microsoft Sentinel incidents
- Entra ID sign-in logs

---

Escalation

An incident may require escalation when evidence indicates suspicious or potentially malicious activity beyond the scope of initial triage.

Information passed during escalation should include:

- Alert summary
- Affected user/system
- Source IP
- Timeline
- Evidence reviewed
- Findings
- Actions already taken
- Recommended next steps

---

Containment

Depending on the evidence and authorised procedures, containment could include:

- Blocking a malicious IP
- Disabling or restricting an account
- Isolating an affected system
- Revoking active sessions
- Escalating to the appropriate security team

Containment actions should follow organisational procedures and authorisation.

---

Incident Closure

Before closing an incident:

- Confirm investigation is complete
- Record findings
- Record actions taken
- Document the timeline
- Confirm escalation where required
- Record the reason for closure

The incident record should allow another analyst to understand what happened and how the alert was handled.

---

Tools Used in My Labs

- Microsoft Sentinel
- KQL
- Microsoft Entra ID
- Kali Linux
- Suricata
- Splunk
- Syslog
- OWASP Juice Shop

---

Current Focus

Alert Triage • Incident Investigation • Evidence Analysis • Authentication Monitoring • Escalation • Containment • Incident Documentation

Progress still ongoing.
