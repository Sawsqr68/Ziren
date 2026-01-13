# Security Policy

## 🔒 Reporting Security Vulnerabilities

**⚠️ CRITICAL: Do NOT open public issues for security vulnerabilities**

### How to Report

1. **Email**: Send details to security@zkm.io
2. **PGP Encryption**: Use our PGP key for sensitive reports
3. **GitHub Security Advisories**: Use [Private Security Advisory](https://github.com/Sawsqr68/Ziren/security/advisories/new)

### What to Include

- Detailed description of the vulnerability
- Steps to reproduce
- Potential impact assessment
- Suggested fix (if available)
- Your contact information

## 🛡️ Security Measures

### Automated Security Scanning

We run comprehensive security scans:

- **Daily**: Full dependency audit, unsafe code detection
- **Weekly**: Comprehensive security report with issue creation
- **Per PR**: Quick security check with automated comments
- **Per Commit**: Pre-commit hooks with Gitleaks

### Tools in Use

| Tool | Purpose | Frequency |
|------|---------|-----------|
| cargo-audit | Dependency vulnerabilities | Daily |
| cargo-deny | License & policy compliance | Daily |
| cargo-geiger | Unsafe code detection | Daily |
| Clippy | Security lints | Per commit |
| Semgrep | SAST analysis | Daily |
| Gitleaks | Secret scanning | Per commit |
| Trivy | Vulnerability scanning | Daily |
| CodeQL | Code analysis | Daily |
| Dependabot | Dependency updates | Daily |

## 📊 Response SLA

| Severity | Initial Response | Fix Timeline |
|----------|-----------------|--------------|
| **Critical** | 6 hours | 24-48 hours |
| **High** | 24 hours | 3-7 days |
| **Medium** | 72 hours | 1-2 weeks |
| **Low** | 1 week | 1 month |

## 🔍 Security Best Practices

### For Contributors

1. Never commit secrets or API keys
2. Use pre-commit hooks
3. Run `cargo audit` before submitting PR
4. Follow secure coding guidelines
5. Review unsafe code blocks carefully

### For Users

1. Always use the latest stable version
2. Review SECURITY_AUDIT.md regularly
3. Subscribe to security advisories
4. Report any suspicious behavior

## 📜 Compliance

- Apache-2.0 / MIT License
- SBOM generation enabled
- Regular security audits
- Transparent disclosure policy

## 🏆 Hall of Fame

We acknowledge security researchers who responsibly disclose vulnerabilities:

- [Future contributors will be listed here]

## 📞 Contact

- Security Email: security@zkm.io
- Response Time: Within 48 hours
- Public Disclosure: After coordinated fix

## 🔐 Cryptographic Library Patches

This project uses patched versions of certain cryptographic libraries for ZKM-specific optimizations. All patches are:

- Publicly available in the `ziren-patches` GitHub organization
- Subject to regular security audits
- Documented in SECURITY_AUDIT.md
- Applied only for performance optimizations without altering cryptographic primitives

If you have concerns about any cryptographic modifications, please report them following our security disclosure process.

---

**Last Updated**: 2026-01-13
**Version**: 2.0
