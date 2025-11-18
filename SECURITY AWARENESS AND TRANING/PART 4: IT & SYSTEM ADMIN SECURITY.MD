

## **PART 4: IT & SYSTEM ADMIN SECURITY (10 Slides)**

**Slide 1: Admins Hold the Keys to the Kingdom**
* "With great power comes great responsibility"
* Privileged accounts = prime targets for attackers
* Real case: Admin reused password → complete domain compromise

**Slide 2: Core IT Admin Responsibilities**
| Area | Objective | Risk if Ignored |
|------|-----------|----------------|
| Access Control | Limit rights to need | Privilege abuse, insider threat |
| Patch Management | Keep systems updated | Exploited vulnerabilities |
| System Hardening | Disable unnecessary services | Backdoors & lateral movement |
| Monitoring & Logs | Detect abnormal activities | Missed breach indicators |
| Backup & Recovery | Ensure data availability | Ransomware loss |

**Slide 3: Access Control Best Practices**
* **Least Privilege:** Minimum rights needed
* **Role-Based Access (RBAC):** Group by job function
* **Multi-Factor Authentication (MFA):** Required for all admin logins
* **Privileged Access Management (PAM):** Control privileged credentials
* **Account Review:** Disable unused admin accounts monthly
* **Logging & Audit:** Track every admin action

**Slide 4: Patching & Vulnerability Management**
1. **Inventory Systems:** Know every device, OS, app
2. **Monitor CVEs:** Subscribe to security bulletins
3. **Prioritize by Risk:** Critical vulnerabilities first (CVSS ≥ 8)
4. **Automate Patching:** Use WSUS, SCCM, Ansible
5. **Verify & Report:** Log success, validate via scanners

**Slide 5: Privilege Misuse & Insider Risk Prevention**
| Risk | Example | Defense |
|------|---------|---------|
| Overprivileged Accounts | Developers with domain admin | Role-based access control |
| Shared Admin Passwords | One password for all admins | PAM or password vault |
| Command Abuse | Admin installs unauthorized tools | Monitoring + approval policy |
| Log Tampering | Admin clears logs after changes | Centralized logging (SIEM) |
| Shadow IT | Unapproved SaaS tools | Whitelisting policy |

**Slide 6: Remote Access & Endpoint Security**
* **RDP Access:** Use VPN + MFA, disable if not required
* **SSH/Telnet:** Allow SSH only with key-based auth
* **Admin Workstations:** Separate from regular desktops
* **Portable Devices:** Encrypt drives (BitLocker/LUKS)
* **USB Devices:** Restrict or log all connections
* **Network Segmentation:** Isolate admin networks from users

**Slide 7: Patch Policy & Vulnerability Scanner Setup**
* Monthly patch window (e.g., second Saturday)
* Maintain patch log & report exceptions
* **Tools:** Qualys/OpenVAS/Nessus for scans, WSUS/Ansible for patching
* Quarterly system hardening audit
* Automated patch rollout with verification

**Slide 8: Incident Response for Admins**
1. Disconnect system from network immediately
2. Inform Security/SOC team — don't fix silently
3. Preserve logs for forensics
4. Change passwords post-incident
5. Document everything for audit and RCA
* **Never hide admin errors — early reporting prevents escalation**

**Slide 9: IT Admin Security Checklist**
- [ ] Maintain inventory of all admin accounts
- [ ] Enforce MFA for privileged access
- [ ] Patch OS and software monthly
- [ ] Disable unused services and ports
- [ ] Use PAM or vault for credentials
- [ ] Log and audit all admin actions
- [ ] Segregate admin network from user LAN
- [ ] Regular vulnerability scans
- [ ] Test backups quarterly
- [ ] Remove access of ex-employees

**Slide 10: IT Admin Key Takeaways**
* Admin credentials = crown jewels — protect accordingly
* Unpatched systems = open doors for attackers
* Least privilege prevents 90% of insider threats
* Monitoring and logging are non-negotiable
* Early incident reporting saves careers and companies

---
