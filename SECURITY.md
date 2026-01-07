# 🔐 Security Policy

## Our Commitment

Prime Directive Labs takes security seriously. We're building critical infrastructure, and we recognize that the security of our systems is paramount to our mission.

## Supported Versions

| Repository | Version | Supported |
|------------|---------|:---------:|
| primedir-contracts | Latest | ✅ |
| primedir-api | Latest | ✅ |
| primedir-app | Latest | ✅ |
| primedir-web | Latest | ✅ |

## Reporting a Vulnerability

### ⚠️ Do NOT Create a Public Issue

If you discover a security vulnerability, **please do not create a public GitHub issue**. Instead, follow our responsible disclosure process.

### 📧 Report Privately

Send your report to:

**security@primedir.ai**

### What to Include

Please include the following information:

1. **Description** — A clear description of the vulnerability
2. **Impact** — What an attacker could achieve
3. **Reproduction Steps** — How to reproduce the issue
4. **Affected Component** — Which repository/contract/endpoint
5. **Suggested Fix** — If you have one (optional)

### Example Report

```
Subject: [SECURITY] SQL Injection in /api/v1/sentinels/

Description:
The sentinel search endpoint is vulnerable to SQL injection.

Impact:
An attacker could extract sensitive data from the database.

Steps to Reproduce:
1. Navigate to /api/v1/sentinels/
2. Set the 'search' parameter to: ' OR 1=1 --
3. Observe unauthorized data access

Affected: primedir-api, ecosystem/views.py

Suggested Fix:
Use parameterized queries instead of string concatenation.
```

## Response Timeline

| Phase | Timeline |
|-------|----------|
| **Acknowledgment** | Within 24 hours |
| **Initial Assessment** | Within 72 hours |
| **Status Update** | Within 7 days |
| **Resolution Target** | Within 30 days (critical) |

## Security Measures

### Smart Contracts

- **Audits** — All production contracts undergo third-party security audits
- **Bug Bounty** — We participate in bug bounty programs (coming soon)
- **Formal Verification** — Critical functions are formally verified
- **Upgrade Patterns** — Transparent, time-locked upgrades only

### Backend

- **Authentication** — SIWE (Sign-In With Ethereum) for secure auth
- **Rate Limiting** — API rate limiting to prevent abuse
- **Input Validation** — All inputs are validated and sanitized
- **Encryption** — TLS everywhere, sensitive data encrypted at rest

### Frontend

- **CSP** — Content Security Policy headers
- **XSS Protection** — React's built-in XSS protection
- **Dependencies** — Regular dependency audits with `npm audit`

## Bug Bounty Program

We're planning a formal bug bounty program. Until then, we offer:

| Severity | Reward Range |
|----------|--------------|
| **Critical** | $1,000 - $10,000 |
| **High** | $500 - $2,000 |
| **Medium** | $100 - $500 |
| **Low** | Recognition |

*Note: Rewards are at our discretion based on impact and quality of report.*

## Safe Harbor

We consider security research conducted in accordance with this policy to be:

- **Authorized** under the Computer Fraud and Abuse Act
- **Exempt** from DMCA restrictions on circumvention
- **Lawful** and not grounds for legal action against researchers

We will not pursue legal action against researchers who:

- Act in good faith
- Avoid privacy violations
- Don't destroy or modify data
- Report findings responsibly

## Contact

- **Security Issues**: security@primedir.ai
- **General Questions**: hello@primedir.ai
- **Discord**: [Join our community](https://discord.gg/primedir)

---

*"We engineer civilization, not just code."*

**Prime Directive Labs** 🛡️

