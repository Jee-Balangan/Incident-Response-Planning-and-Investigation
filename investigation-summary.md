# Investigation Summary

## Incident Overview

This investigation reviewed packet capture data and SIEM information related to suspicious authentication activity targeting a WordPress login portal.

The goal was to identify the source and target of the activity, determine whether successful authentication occurred, and reconstruct the sequence of events.

## Scope of Analysis

The investigation focused on:

- Repeated requests to the WordPress login page
- Automated authentication activity
- HTTP request and response behavior
- Successful login indicators
- Event timing and sequence
- Evidence from packet captures and SIEM data

## Key Findings

### Automated Login Activity

The traffic showed repeated requests to the WordPress login endpoint.

The HTTP headers included a Hydra-related user-agent string, which supported the conclusion that the activity was automated rather than normal user behavior.

### Successful Authentication

Packet analysis showed HTTP `302` responses and redirects to the WordPress administrative area.

These responses were used as evidence that at least some authentication attempts were successful.

### Credential Exposure

The original investigation identified credentials within the packet captures.

Those credential values are intentionally omitted from this public portfolio version.

### Timeline Reconstruction

The investigation used packet timestamps and event sequencing to reconstruct the attack timeline.

The activity occurred over a short period and included repeated authentication attempts followed by successful login events.

## Evidence Sources

Evidence reviewed during the investigation included:

- PCAP files
- HTTP request and response data
- Packet timestamps
- TCP streams
- SIEM information
- WordPress login traffic
- Authentication redirects

## Analysis Approach

The investigation process included:

1. Identifying the targeted WordPress service
2. Reviewing repeated login requests
3. Inspecting HTTP headers for automation indicators
4. Checking response codes for successful authentication
5. Following TCP streams for additional context
6. Comparing timestamps across events
7. Building a chronological incident timeline

## Conclusion

The investigation identified activity consistent with an automated brute-force attack against a WordPress login portal.

Packet analysis showed repeated authentication attempts, Hydra-related activity, and successful authentication events.

The investigation demonstrated how network evidence and authentication behavior can be combined to determine the scope and sequence of suspicious activity.
