Case 03 — Suricata Web Login Alert

Lab Context

OWASP Juice Shop was used as the target application in my security monitoring lab.

Detection

POST /rest/user/login

Threshold

5 attempts within 30 seconds

Suricata SID

1000001

Investigation

- Review the Suricata alert.
- Identify the source address.
- Confirm the HTTP request and timestamp.
- Review related eve.json events.
- Search for related activity in Splunk.
- Check whether the behaviour continues after the alert.

Outcome

This exercise connected web activity with IDS detection and SIEM investigation.

Progress still ongoing.
