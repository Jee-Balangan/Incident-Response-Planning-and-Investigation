# Incident Response Lifecycle

## Preparation

Preparation focuses on making sure the organization is ready before an incident occurs.

Key activities include:

- Define incident types
- Establish severity levels
- Create escalation paths
- Train personnel
- Conduct tabletop exercises
- Maintain tools such as SIEM, IDS/IPS, and backups
- Develop playbooks for common incidents

## Detection and Analysis

The goal of detection and analysis is to identify suspicious activity, determine whether it represents an incident, and understand its scope.

Activities include:

- Review SIEM dashboards
- Monitor EDR alerts
- Analyze network logs
- Classify incidents by type and severity
- Collect evidence such as logs, malware samples, and email headers
- Escalate High and Critical incidents when needed

## Containment

Containment focuses on limiting the spread and impact of the incident.

Actions may include:

- Isolate affected systems
- Preserve forensic evidence
- Block malicious IP addresses or URLs
- Disable infected devices
- Redirect traffic to unaffected systems
- Apply longer-term controls such as patching and stronger segmentation

## Eradication

Eradication focuses on removing the cause of the incident.

Activities include:

- Remove malware
- Identify how the threat bypassed defenses
- Remove persistence mechanisms
- Address exploited vulnerabilities
- Apply security updates or other corrective actions

## Recovery

Recovery focuses on safely restoring normal operations.

Actions include:

- Restore systems from clean backups
- Validate system integrity
- Return systems to service
- Monitor for reinfection or continued suspicious activity
- Improve detection rules where needed

## Post-Incident Analysis

Post-incident analysis focuses on improving future response.

Activities include:

- Build a timeline of events
- Document response actions
- Record lessons learned
- Update incident response procedures
- Strengthen defensive controls
- Test changes through tabletop exercises or simulations
