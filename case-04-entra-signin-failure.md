Case 04 — Microsoft Entra ID Sign-In Failure

Scenario

A failed sign-in is identified in Microsoft Entra ID logs.

Initial Triage

Review:

- User account
- Timestamp
- Sign-in result
- Source IP
- Failure reason
- Error code

Investigation

Check for repeated failures, successful sign-ins around the same period, and changes in account status.

Lab Context

My Entra ID practice included successful and failed sign-ins, authentication errors and account lockout behaviour.

Decision

The sign-in result alone is not enough to determine malicious activity. The event should be reviewed in context with surrounding authentication activity.

Progress still ongoing.
