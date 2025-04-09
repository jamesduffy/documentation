# Runbook

> [!NOTE]
> This document goes together with the [Incident Response Plan]('../Incident+Response/README.md'). This document is organized that for each incident you start at the top of this document and work your way down.

## Initial Response

- [ ] Acknowledge the Alert
  > Confirm receipt of the alert in the monitoring tool (e.g., PagerDuty, Slack, email).
  >
  > Notify the team if not already done by the alerting system.
- [ ] Assign an Incident Commander (IC)
  > The first responder assumes the role of IC until it’s reassigned.
- [ ] Create a communication channel (e.g., Slack channel) and name it `#incident-YYYY-MM-DD`.
- [ ] Declare Incident Severity
  > Use the following criteria to determine severity:
  > - Low: Minor issue, no immediate impact, business continues as usual.
  > - Medium: Limited user impact, non-critical systems affected.
  > - High: Critical systems affected, major user impact, or security issue.

## Assessment & Identification

- [ ] Assess Impact
  > Identify which systems or services are affected
  >
  > Determine if there is ongoing damage (e.g., data loss, security breach).

- [ ] Gather Initial Information
  > Check logs, alerts, and dashboards for anomalies.
  >
  > Answer these questions:
  > - [ ] What is currently not working?
  > - [ ] What was the last change made?
  > - [ ] What is the scope of the issue (single service or multiple)?

- [ ] Create Incident Ticket
  > Document the incident details in the ticketing system (e.g., JIRA). Include the following:
  > - Incident description.
  > - Systems/services impacted.
  > - Current status.

If root cause is identified, proceed to [Containment](#containment). If not, escalate to additional responders for help.

## Containment

- [ ] Implement Short-Term Containment
  > Isolate the affected systems or services to prevent further impact. (Disable access, apply firewall rules, or shut down impacted processes as necessary.)
- [ ] Document Containment Actions
  > Record each action taken in the incident ticket with timestamps.
Notify stakeholders of the containment status.

If containment is successful and impact is stopped, move to Mitigation & Resolution.

## Mitigation & Resolution

- [ ] Mitigate the Impact
  > Apply temporary fixes to mitigate the impact if a full resolution is not possible immediately.
  >
  > Examples: Redirect traffic, increase resource limits, revert recent changes.

- [ ] Implement Full Resolution
  > Apply the permanent fix or patch to resolve the root cause of the incident.
  >
  > Monitor the systems to ensure stability and that the issue does not recur.

- [ ] Verify Resolution
  > Ensure that all affected services are restored and functioning as expected.
  >
  > Confirm with stakeholders that the issue is resolved.

Once the resolution is verified, proceed to Post-Incident Review.

## Post-Incident Review

- [ ] Schedule a Post-Incident Review

  > Within 24-48 hours of incident resolution, schedule a review meeting.
  >
  > Include all responders and relevant stakeholders.

- [ ] Create Post-Incident (Postmortem) Report

  > Document the incident timeline, root cause, actions taken, and resolution.
  >
  > Identify areas for improvement and update the runbook if necessary.
