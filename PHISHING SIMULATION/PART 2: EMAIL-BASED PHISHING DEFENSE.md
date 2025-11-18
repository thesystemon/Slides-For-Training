## **PART 2: EMAIL-BASED PHISHING DEFENSE (20 Slides)**

**Slide 1: Email - The Primary Attack Vector**
* 96% of phishing attacks start with email
* Average employee receives 14 malicious emails per year
* Email remains most effective attack method

**Slide 2: Anatomy of a Phishing Email**
* **Header:** Spoofed sender information
* **Subject:** Urgent call-to-action
* **Body:** Emotional manipulation with fake legitimacy
* **Links:** Disguised malicious URLs
* **Attachments:** Malware-loaded files
* **Footer:** Fake contact information

**Slide 3: Email Safety Checklist - Part 1 (Sender Analysis)**
* Who is the sender? Check full email address
* Is the domain correct? Look for typos (micros0ft.com)
* Does reply-to match sender? Mismatch is major red flag
* Is there [External] tag? Treat with increased caution
* Did you expect this email? Unexpected requires verification

**Slide 4: Email Safety Checklist - Part 2 (Content Analysis)**
* What's the tone? Urgent, threatening, too-good-to-be-true
* Are there grammar errors? Poor language indicates scam
* Is branding consistent? Logos, colors, fonts should match
* Are there suspicious elements? Strange formatting, broken images

**Slide 5: Email Safety Checklist - Part 3 (Technical Analysis)**
* Hover over links - don't click! Preview true destination
* Check attachments before opening - dangerous file types
* Is it asking for credentials? Legitimate services don't ask via email
* Are there unusual send times? Strange hours indicate compromise

**Slide 6: Email Safety Checklist - Part 4 (Relationship Analysis)**
* Does greeting match relationship? Generic from colleague is suspicious
* Look for unexpected BCC/mass recipients - broad campaign indicator
* Verify with another channel! Call or message using known contact
* Is request appropriate for relationship? Question mismatches

**Slide 7: Safe Link-Hovering Demonstration**
* **Visual Guide:** Show email with "View Document" button
* **Hover Action:** Mouse over reveals true destination
* **Mismatch Example:** http://phishy-site.net/login vs sharepoint.company.com
* **Visual Cue:** Red "X" appears with "URL MISMATCH! DO NOT CLICK"
* **Good Example:** Clean company-domain URL appears
* 💡 **Trainer Tip:** "Practice hovering every time"

**Slide 8: Attachment Safety Protocol**
* **Never Open:** .EXE, .SCR, .BAT, .MSI, macro-enabled files
* **Extreme Caution:** .ZIP, .RAR, .ISO from unknown senders
* **Safe Practices:**
  - Confirm expected attachments via alternate channel
  - Scan with antivirus before opening
  - Use sandbox for suspicious files
  - Company policy: All attachments scanned by security

**Slide 9: The Attacker's Toolbox: Spoofing vs Compromise**
* **Email Spoofing:** Faking "From" address to look trusted
  - Example: Email from CEO sent from hacker's server
* **Legitimate Account Compromise:** Using real hacked account
  - Example: Vendor email account used to send fake invoices
* **More Dangerous:** Comes from trusted source, passes technical checks
* 💡 **Trainer Tip:** "If email from known contact seems 'off', verify even if address is correct"

**Slide 10: Header Analysis for Advanced Detection**
* **From vs Return-Path:** Mismatch indicates spoofing
* **SPF/DKIM/DMARC:** Technical authentication checks
* **Received Headers:** Trace email path for anomalies
* **Message-ID:** Patterns indicating mass sending

**Slide 11: Brand Impersonation Techniques**
* **Logo Theft:** Copying official branding
* **Domain Spoofing:** Similar-looking domains
* **Template Copying:** Mimicking official email templates
* **Signature Forgery:** Fake executive signatures
* **Language Mimicry:** Copying writing style

**Slide 12: Real-World Example 1 - Fake Invoice**
* **Scenario:** Finance receives email from known vendor
* **Subject:** Invoice #INV-98432 - Payment Required
* **Sender:** accounting@legit-vend0r.com (zero instead of 'o')
* **Body:** "Please process payment for attached invoice. Due today."
* **Red Flags:** Spoofed domain, urgent deadline, unexpected attachment
* **Lesson:** Always verify payment changes via known phone number

**Slide 13: Real-World Example 2 - CEO Fraud**
* **Scenario:** Urgent email from "CEO"
* **Subject:** URGENT - Confidential
* **Sender:** ceo@yourcompany.com (spoofed to look real)
* **Body:** "I'm in a meeting. Need gift cards for team ASAP. Text codes."
* **Red Flags:** Unusual request, high urgency, secrecy, untraceable payment
* **Lesson:** Authority doesn't bypass procedure - verify unusual financial requests

**Slide 14: Real-World Example 3 - Password Reset**
* **Scenario:** Email from "IT Department"
* **Subject:** Password Expiration Notice
* **Sender:** it-support@corp-portal.net
* **Body:** "Your password expires in 2 hours. Click here to reset now."
* **Red Flags:** External domain, artificial urgency, fake login page
* **Lesson:** IT never sends direct password reset links - go to portal directly

**Slide 15: Business Email Compromise (BEC) Deep Dive**
* **Targets:** Finance, HR, Executive Assistants
* **Methods:** Executive impersonation, vendor email compromise
* **Red Flags:**
  - Last-minute invoice changes
  - New payment instructions
  - Pressure to keep requests secret
  - Bypassing normal procedures
* **Losses:** Average $130,000 per incident

**Slide 16: Advanced BEC Detection**
* **Language Analysis:** Unusual phrasing for supposed sender
* **Request Analysis:** Abnormal payment amounts or recipients
* **Timing Analysis:** Unusual send times for relationship
* **Procedure Analysis:** Bypassing standard approval workflows
* **Verification:** Multi-channel confirmation required

**Slide 17: Credential Phishing Pages**
* **Appearance:** Perfect copies of real login pages
* **URL Tricks:** Subdomains (yourcompany.secure-login.com)
* **SSL Certificates:** Attackers now use HTTPS too
* **Redirection:** Legitimate site after credential capture
* **Detection:** Check URL carefully before entering credentials

**Slide 18: Malware Delivery via Email**
* **Macro-Enabled Documents:** .DOCM, .XLSM files
* **PDF with Links:** Malicious links in PDF documents
* **Archive Files:** ZIP with executable content
* **OneNote Files:** Increasingly used for malware
* **ISO Images:** Bypass some security controls

**Slide 19: Email Client Security Features**
* **Report Phishing Buttons:** One-click reporting
* **Safe Links:** URL scanning before opening
* **Attachment Sandboxing:** Safe opening environment
* **External Tagging:** Automatic external sender identification
* **Spoof Intelligence:** AI-based sender verification

**Slide 20: Email Defense Commitment**
* "I will use the email safety checklist for every suspicious email"
* "I will hover before clicking any link"
* "I will verify unexpected attachments"
* "I will report phishing attempts immediately"

---
