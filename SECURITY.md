# Security Policy

Security, privacy and trust are core parts of nVibes.

nVibes is a social-tech platform for real-world human connection. Security issues can affect not only digital accounts, but also trust, safety, location context, chats, events and real-life interactions.

---

## Reporting a Vulnerability

Please do not publish exploit details, secrets, tokens, private keys, database credentials or personal data in public issues.

For non-critical security concerns, use the **Security Concern** issue template and avoid sensitive details.

For critical vulnerabilities, contact the maintainer privately before creating a public issue.

Critical examples:

- authentication bypass
- admin access bypass
- token or session compromise
- private user data exposure
- chat or media data exposure
- location or MeetNow abuse path
- production infrastructure exposure
- database credential or backup exposure
- exploitable upload or file handling issue

---

## What to Include

When reporting, include only safe, high-level information:

- affected area, for example App, Api, Infrastructure, Auth, Chat, Uploads or Deployment
- severity estimate
- impact summary
- affected environment, if known
- whether active exploitation is suspected
- suggested mitigation, if available

Do not include:

- real secrets
- tokens
- private SSH keys
- database passwords
- raw private user data
- step-by-step exploit instructions in public issues

---

## Security Principles

nVibes prioritizes:

- least privilege
- privacy by design
- secure authentication
- explicit authorization
- input validation
- safe error handling
- logging without sensitive data
- controlled database migrations
- secure deployment practices
- review before production changes
- trust and safety for real-world interactions

---

## Production-Sensitive Areas

The following areas require careful review before changes:

- Auth, Passkeys, MFA and JWT handling
- password reset flows
- user deletion and account lifecycle
- chat, groups and media
- QR, MeetNow and real-world verification
- location, Nearby and Inspire
- Prisma schema and migrations
- Azure, Nginx, Cloudflare and VMSS deployment
- Key Vault, secrets and environment configuration
- admin routes and audit logs

---

## Response Expectations

Security reports should be triaged by severity:

```txt
P0 - critical, production or user safety at immediate risk
P1 - high, security-sensitive and should be prioritized
P2 - medium, should be planned and fixed
P3 - low, hardening or best-practice improvement
```

Production-sensitive fixes should include:

- risk assessment
- test or validation plan
- rollback plan
- deployment impact
- documentation impact

---

## nVibes Repository Steward Rule

The nVibes Repository Steward must never store or expose secrets and must not perform production deployments, production database migrations or risky infrastructure changes without explicit human approval.
