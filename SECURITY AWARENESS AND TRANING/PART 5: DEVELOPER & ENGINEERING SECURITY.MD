## **PART 5: DEVELOPER & ENGINEERING SECURITY (10 Slides)**

**Slide 1: Code is Power — and Responsibility**
* "Every line of code can protect or expose your organization"
* Small mistakes can expose entire systems
* Real case: AWS keys in GitHub → complete S3 data leakage in 24 hours

**Slide 2: Secure Coding Mindset (Shift Left Security)**
| Stage | Secure Practice |
|-------|----------------|
| Design | Threat modeling, data classification |
| Development | Input validation, least privilege code |
| Testing | SAST/DAST scanning, secure unit tests |
| Deployment | Hardening, secret management |
| Maintenance | Patch dependencies, monitor CVEs |

**Slide 3: Common Vulnerabilities (OWASP Top 10)**
| Vulnerability | Example | Prevention |
|---------------|---------|------------|
| Injection | SQL: ' OR 1=1-- | Use prepared statements |
| Broken Auth | Weak login logic | JWT + bcrypt |
| Sensitive Data Exposure | Unencrypted DB | Encrypt at rest/transit |
| XXE | XML parser attack | Disable external entities |
| Security Misconfiguration | Default creds, open S3 | Harden configurations |
| XSS | `<script>alert(1)</script>` | Sanitize inputs |

**Slide 4: Secret Management**
* **Don't:** Store API keys in code, commit .env files to Git
* **Do:** Use secret vaults (HashiCorp Vault, AWS Secrets Manager)
* **Don't:** Share secrets in Slack/email
* **Do:** Use password vault or secure channels
* **Don't:** Use same key for all services
* **Do:** Rotate keys regularly
* Example: `config.js` with `db_password = "admin123"` → scanned by bots in minutes

**Slide 5: Dependency & Package Security**
* "You inherit every vulnerability your library has"
* Use trusted repos only (npm, Maven Central)
* Pin exact versions in package-lock.json or pom.xml
* Run npm audit, mvn dependency:check, or Snyk
* Regularly patch and test dependencies
* Maintain SBOM (Software Bill of Materials)
* **Never use "latest" tag in Dockerfiles**

**Slide 6: Secure DevOps & CI/CD Practices**
| Area | Secure Practice |
|------|----------------|
| Pipeline Security | Isolated runners |
| Code Signing | Sign artifacts before release |
| Static Analysis (SAST) | SonarQube/CodeQL in pipeline |
| Dependency Scanning | Snyk, Dependabot automation |
| Container Security | Trivy or Clair for image scanning |
| Secrets in Pipelines | Use vaults, not env variables |
| Access Control | Least privilege for build agents |

**Slide 7: Vulnerability Prevention Checklist**
| Area | Checklist Item | Status |
|------|----------------|--------|
| Input Validation | All inputs validated & sanitized | ☐ |
| Authentication | Strong password & MFA logic | ☐ |
| Authorization | Role-based access enforced | ☐ |
| Error Handling | No sensitive info in errors | ☐ |
| Secrets | Stored in vault, not code | ☐ |
| Logging | Secure, centralized, non-repudiable | ☐ |
| Dependencies | Regularly scanned & updated | ☐ |

**Slide 8: Code Review & Peer Validation**
* "Two eyes see bugs, four eyes prevent breaches"
* Use code review templates with security checkpoints
* Focus on: Input/output handling, Authentication logic, Access control, Data encryption, Logging
* Automate code review for secrets using GitGuardian/TruffleHog
* Security bugs = Functional bugs — equal priority

**Slide 9: Secure Build and Deployment**
| Phase | Key Action |
|-------|-----------|
| Build | Sign packages, hash verify outputs |
| Deploy | Secured pipelines with MFA |
| Environment Config | .env files managed by vault |
| Rollback Plan | Maintain secure version rollback |
| Post-Deploy Monitoring | Monitor anomalies and abuse |

**Slide 10: Developer Security Checklist**
- [ ] Enable SAST/DAST scanning in CI/CD
- [ ] Use secret vault for all keys and tokens
- [ ] Enforce code review for security issues
- [ ] Scan all containers and dependencies
- [ ] Avoid hardcoding credentials or URLs
- [ ] Use HTTPS/TLS for all endpoints
- [ ] Apply input validation and encoding
- [ ] Perform threat modeling per module
- [ ] Implement security logging
- [ ] Patch third-party libraries monthly

---
