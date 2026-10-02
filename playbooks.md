# Incident Response Playbooks

## Malware Infection

### Identify and Contain

- Identify affected systems
- Isolate infected hosts from the network
- Preserve forensic evidence
- Collect indicators such as suspicious files, processes, connections, and hashes
- Compare indicators against threat intelligence sources

### Analyze the Malware

Static analysis may include:

- Reviewing file properties and metadata
- Extracting readable strings
- Identifying suspicious code or embedded indicators

Dynamic analysis may include:

- Executing the sample in an isolated sandbox
- Observing registry, file system, and process changes
- Capturing network traffic
- Identifying possible command-and-control or exfiltration activity

### Investigate Persistence

Review the system for persistence methods such as:

- Registry modifications
- Scheduled tasks
- Startup files
- Hidden services
- DLL hijacking

### Eradication and Recovery

- Remove the malware
- Restore systems from verified clean backups
- Address the vulnerability or weakness that allowed the infection
- Validate system integrity before returning systems to service

### Post-Incident Actions

- Document findings and response actions
- Update security policies and controls
- Patch identified vulnerabilities
- Provide additional user training where needed

## Phishing

### Identify and Verify

- Review email headers
- Inspect sender and reply-to information
- Check links and attachments
- Compare the message against common phishing indicators

### Contain the Threat

- Warn employees about the phishing message
- Quarantine or flag the email
- Notify the security or IT team

### Investigate Impact

- Determine whether users interacted with the message
- Review affected endpoints with security monitoring tools
- Identify whether credentials or other information were submitted

### Eradicate and Secure

- Preserve the phishing email for analysis
- Reset compromised credentials when necessary
- Monitor affected accounts for suspicious activity
- Contact external service providers if their accounts were affected

### Prevention and Follow-Up

- Notify employees of lessons learned
- Conduct phishing-awareness training
- Review email security policies
- Monitor for recurring activity
- Document the incident

## Denial-of-Service

### Identify and Characterize

- Detect unusual traffic volume
- Identify abnormal packet or request patterns
- Determine whether activity is consistent with a DoS attack
- Classify the type of attack when possible

### Measure Impact

- Review traffic volume and bandwidth consumption
- Identify affected services
- Determine which systems are experiencing the greatest impact
- Prioritize critical services

### Investigate Sources

- Identify patterns in source IPs or traffic origins
- Review suspicious ranges or repeated sources
- Document observed attack patterns

### Mitigate the Attack

- Apply firewall rules or rate limits
- Monitor whether mitigation is reducing malicious traffic
- Use threat intelligence integrations where appropriate
- Preserve network and firewall configurations before making major changes

### Post-Mitigation Actions

- Continue monitoring for residual activity
- Document what occurred and which controls were effective
- Review opportunities to improve defenses
- Test response procedures through future simulations
