Case 01 — Repeated SSH Authentication Failures

Scenario

Multiple failed SSH login attempts are detected against a Linux system.

Initial Triage

- Confirm the alert time and affected host.
- Identify the source IP.
- Review the number and frequency of failed attempts.
- Check the authentication logs for related events.

Evidence

- Syslog / sshd events
- Source IP
- Target host
- Timestamps
- Authentication result

Investigation

Review whether the same source generated repeated failures and search for successful authentication or other activity around the same time.

Decision

Repeated failures can indicate a mistyped password, automated scanning, or an attempted credential attack. The surrounding evidence determines whether escalation is required.

Progress still ongoing.
