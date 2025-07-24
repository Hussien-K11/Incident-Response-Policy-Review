# Phishing Alert Simulation

## ➀ Scenario Overview

A user from the finance department reports a suspicious email with the subject line:  
**"Urgent: Invoice Payment Overdue – Click to Review"**  
The email contains a link and a ZIP attachment (`invoice2024.zip`). The user did not click the link but forwarded the email to the SOC team.

---

## ➁ Initial Investigation

**Steps Taken:**
- Reviewed email headers for spoofed sender domain  
- Scanned attachment hash using [VirusTotal](https://www.virustotal.com)  
- Inspected embedded link in a sandboxed browser  
- Queried logs for outbound HTTP requests matching the link’s domain

**Findings:**
- The link resolves to an IP flagged for phishing by multiple engines  
- The ZIP attachment hash is known malware (`Emotet` variant)  
- No user in the environment clicked the link (confirmed via proxy logs)

---

## ➂ Policy Reference Check

| IR Phase            | Policy Coverage | Analyst Notes |
|---------------------|------------------|----------------|
| **Identification**  | ✔️ Covered | Policy instructs prompt reporting — user complied |
| **Containment**     | ❌ Not defined clearly | No guidance on isolating a potentially exposed machine |
| **Eradication**     | ❌ Not applicable here | Since no action was taken, no eradication necessary |
| **Recovery**        | ❌ Not referenced | No mention of restoring systems or verifying integrity |
| **Communication**   | ⚠️ Partially covered | Policy says notify IR Lead, but doesn't mention users, management, or external parties |
| **Documentation**   | ⚠️ Mentioned briefly | Lacks detail on how or where incidents should be logged |

---

## ➃ Analyst Action Summary

As the assigned junior analyst, I:
- Logged the alert in the incident tracking system  
- Updated the alert with VirusTotal hash report and domain WHOIS  
- Tagged the user’s device for continued monitoring  
- Notified the IR Lead for awareness (per policy)  
- Recommended no further action since there was no execution

---

## ➄ Recommendations

| Area | Suggested Improvement |
|------|------------------------|
| Containment | Add protocol for temporary isolation of reported endpoints |
| Communication | Include guidance for user notification and stakeholder escalation |
| Documentation | Specify how and where alerts should be recorded (e.g., ticketing, SIEM) |
| Evidence Handling | Add steps for preserving and storing evidence in case of delayed malware execution |

---

> **Analyst Note:**  
> This simulation demonstrates how even a simple phishing case can expose key policy weaknesses. While the policy covered reporting and general roles, it lacked operational guidance on containment and documentation workflows. A SOC analyst in this scenario would need to rely heavily on team experience or external protocols.
