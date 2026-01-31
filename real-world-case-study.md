# Real-World Phishing Email Case Study (Sanitized)

This document presents a **sanitized real-world phishing email analysis** performed during SOC operations.

All sensitive information has been modified or redacted.


## Incident Context

- Detection Source: User-reported email
- Email Type: Credential harvesting
- Target: Corporate mailbox
- Severity: Medium


## Initial Triage

- User reported suspicious login request email
- No attachment present
- Embedded URL observed
- User interaction status: Confirmed click, no credential submission


## Header Analysis Summary

Key observations:
- Display name impersonated internal IT team
- Sender domain did not match internal domain
- SPF: Pass
- DKIM: Pass
- DMARC: Pass

**Note:** Authentication passing does not imply legitimacy.


## URL Analysis

- URL used a look-alike domain
- Domain recently registered
- Hosted on shared infrastructure
- Sandbox analysis showed credential harvesting page


## Threat Intelligence Correlation

- Domain observed in multiple phishing campaigns
- Indicators matched existing threat intelligence entries
- No prior sightings within the organization


## Verdict

**Confirmed Phishing – Credential Harvesting**


## Defensive Actions Taken

- Email removed from user inbox
- Domain blocked at email gateway
- User educated on phishing indicators
- Monitoring enabled for related activity
