# Security Policy

## Reporting Security Vulnerabilities

We take security seriously. If you discover a security vulnerability in PowerApps Components, please report it responsibly and confidentially.

### Do Not

- ❌ Do not open public issues for security vulnerabilities
- ❌ Do not disclose vulnerabilities on social media
- ❌ Do not share vulnerability details in discussions or forums

### How to Report

Please email security vulnerabilities to:

**📧 security@programmingcorporate.com**

Include in your report:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if available)

**Expected Response Time:**
- Initial acknowledgment: Within 48 hours
- Investigation: Within 7 days
- Fix release: Within 30 days (for critical issues)

## Security Standards

### Code Review

All code changes undergo security review by maintainers including:
- Static code analysis
- Dependency vulnerability scanning
- Authorization and access control verification

### Dependency Management

- Regular updates to dependencies
- Monitoring for known vulnerabilities via GitHub Dependabot
- Security alerts enabled for all repositories

### Data Protection

- Sensitive information never committed to repository
- .gitignore configured to exclude credentials
- Environment variables for secrets in development

### Access Control

- Branch protection rules enabled
- Required pull request reviews
- Signed commits recommended
- Administrators only can merge code

## Vulnerability Disclosure Timeline

1. **Day 1:** Acknowledge receipt and begin investigation
2. **Day 3-7:** Investigate and develop fix
3. **Day 8-14:** Create patch and test thoroughly
4. **Day 15-30:** Release patch version with security update
5. **Day 30:** Publicly disclose vulnerability (coordinated disclosure)

## Security Best Practices for Users

### Component Usage

- Update to the latest version regularly
- Review component properties and events
- Test components in development environment before production
- Monitor for security updates

### Integration

- Validate input data from users
- Use authorization and authentication controls
- Never hardcode secrets in applications
- Follow principle of least privilege

### Reporting Application Vulnerabilities

If you discover a vulnerability in your application using PowerApps Components:

1. Check if it's a vulnerability in PowerApps Components or your implementation
2. If in PowerApps Components, report to security@programmingcorporate.com
3. If in your application, fix in your codebase

## Supported Versions

Security updates are provided for:

| Version | Status | Support Ends |
|---------|--------|-------------|
| 1.x     | Active | Dec 31, 2026 |
| 0.x     | Legacy | Dec 31, 2025 |

Upgrade to latest version for security patches.

## Security Advisories

Security advisories are published in:
- GitHub Security Advisories
- Release notes with security updates
- Email notifications (for major issues)

Subscribe to releases for security updates.

## PII and Sensitive Data

Never include in issues, PRs, or discussions:
- Personal information
- API keys or tokens
- Database connection strings
- Private credentials
- Customer data

Use `[REDACTED]` if discussing security issues.

## Compliance

This project adheres to:
- Microsoft PowerApps Security Guidelines
- OWASP Top 10 Security Principles
- Industry security best practices

## Questions?

- 📧 Email: security@programmingcorporate.com
- 🐛 Report: [GitHub Issues](https://github.com/programmingcorporate/PowerAppsComponents/issues)
- 💬 Discuss: [GitHub Discussions](https://github.com/programmingcorporate/PowerAppsComponents/discussions)

---

**Last Updated:** February 2026

Thank you for helping keep PowerApps Components secure!
