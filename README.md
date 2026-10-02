# Incident Response Planning and Investigation

## Project Overview

This project combines two parts of incident response work:

1. A structured Incident Response Plan for Capybara Unlimited
2. Hands-on investigation notes from a separate WordPress brute-force incident

Together, these materials show both the planning side of incident response and the investigation side of analyzing suspicious activity and documenting evidence.

## Incident Response Plan

The Capybara Unlimited Incident Response Plan was designed to provide a structured process for detecting, responding to, and recovering from cybersecurity incidents.

The plan includes:

- Incident response objectives
- Scope and coverage
- Roles and responsibilities
- Incident response lifecycle
- Communication procedures
- Key performance indicators
- Common response mistakes and mitigations
- Tools and techniques
- Review and maintenance procedures
- Incident-specific playbooks

## Incident Response Lifecycle

The plan follows these phases:

### Preparation

- Define incident types and severity levels
- Train personnel
- Maintain security tools
- Develop response playbooks

### Detection and Analysis

- Review SIEM, EDR, and network data
- Classify incidents by type and severity
- Collect evidence
- Escalate high-impact incidents when necessary

### Containment

- Isolate affected systems
- Block malicious traffic
- Preserve forensic evidence
- Apply short-term and long-term containment measures

### Eradication

- Remove malware or other malicious activity
- Identify the root cause
- Remove persistence mechanisms
- Address exploited weaknesses

### Recovery

- Restore systems from clean backups
- Verify system integrity
- Monitor for reinfection or continued activity

### Post-Incident Analysis

- Build an incident timeline
- Document findings
- Record lessons learned
- Update response procedures
- Test improvements

## Roles and Responsibilities

The plan defines responsibilities for:

- Incident command
- SOC analysts
- Forensic specialists
- IT administrators
- Legal and compliance
- Public relations and communications
- Executive leadership
- Threat intelligence teams
- Security awareness personnel
- General employees

## Incident Response Playbooks

The plan includes detailed playbooks for:

- Malware infection
- Phishing
- Denial-of-Service attacks

Each playbook follows a structured process for identification, containment, investigation, eradication, recovery, and reporting.

## Investigation Notes

The second part of the project documents an investigation into automated login activity targeting a WordPress authentication portal.

The investigation used packet capture data and SIEM information to identify:

- The targeted WordPress service
- Repeated authentication requests
- Hydra-related activity
- Successful authentication events
- Attack timing
- A timeline of major events
- Evidence from HTTP responses and packet analysis

The investigation concluded that the activity was consistent with an automated brute-force attack against the WordPress login portal.

## Skills Demonstrated

- Incident response planning
- Incident lifecycle development
- SOC roles and escalation planning
- Incident classification
- Evidence collection
- Network traffic analysis
- Authentication event analysis
- Timeline reconstruction
- PCAP analysis
- SIEM-based investigation
- Malware response planning
- Phishing response planning
- DoS response planning
- Incident documentation
- Post-incident review

## Takeaway

This project demonstrates both sides of incident response: preparing an organization before an incident occurs and investigating activity after suspicious behavior is detected.

Combining planning, playbooks, evidence review, and timeline development provides a more complete view of how incident response supports security operations.
