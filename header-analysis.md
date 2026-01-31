# Email Header Analysis

Email headers provide critical metadata about the origin and delivery path of an email.


## Key Headers Reviewed

- `From`
- `To`
- `Reply-To`
- `Return-Path`
- `Message-ID`
- `Received`
- `Authentication-Results`


## Received Header Analysis

- Emails may contain multiple `Received` headers
- Headers are added by each Mail Transfer Agent (MTA)
- Headers are read bottom-up to trace the sender origin
- Only headers added by trusted MTAs should be trusted


## Authentication Results

- SPF validates sending server authorization
- DKIM validates message integrity
- DMARC defines handling policy

Passing authentication checks does **not** guarantee the email is legitimate.
