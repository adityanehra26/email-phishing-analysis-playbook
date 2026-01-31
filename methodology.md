# Phishing Email Analysis Methodology

This document outlines a structured methodology used to analyze phishing emails in a SOC environment.

The objective is to determine **malicious intent, impact, and required defensive actions** using evidence-based analysis.

---

## 1. Initial Triage

The purpose of triage is to quickly assess risk and prioritize analysis.

Key questions:
- Was the email reported by a user or detected automatically?
- Did the user interact with the email?
- Are credentials or systems potentially compromised?


## 2. Header and Sender Examination

- Review sender address and display name
- Identify spoofing or impersonation attempts
- Analyze `Received` headers to understand mail flow
- Validate sender IP reputation


## 3. Content Examination

- Review subject line and message body
- Identify social engineering techniques:
  - Urgency
  - Authority
  - Trust
  - Scarcity
- Check for mismatched branding or language inconsistencies


## 4. URL and Web Artifacts

- Extract URLs from email body
- Expand shortened URLs
- Inspect domains for look-alike or typosquatting
- Perform reputation and sandbox checks


## 5. Attachment Examination

- Extract attachments from the email
- Calculate file hashes
- Perform static analysis
- Perform dynamic analysis if required


## 6. Contextual Analysis

- Correlate indicators with recent incidents
- Check threat intelligence sources
- Look for patterns related to known campaigns


## 7. Verdict and Documentation

- Classify the email as malicious, suspicious, or benign
- Document findings and artifacts
- Recommend defensive actions where applicable
