# Policy Gap Analysis – Incident Response Policy

## ➀ Overview

This document reviews the organisation’s current Incident Response Policy to identify potential gaps, ambiguities, or areas lacking in clarity or completeness. The analysis is based on best practices from frameworks such as NIST SP 800-61 and CIS Controls.

---

## ➁ Key Observations

| Section Reviewed            | Observation |
|----------------------------|-------------|
| Scope                      | Clearly defines users and systems in scope. No reference to third-party vendor procedures. |
| Roles & Responsibilities   | Core roles identified (IR Lead, IT, Analyst), but lacks contact procedures or on-call hierarchy. |
| Incident Categories        | Categories are realistic but could include severity levels or examples. |
| Phases of Response         | Follows NIST lifecycle. Some detail is thin (e.g., containment not split into short/long term). |
| Documentation              | Mentions evidence, but no reference to chain of custody, legal standards, or format. |
| Review Cycle               | Policy review noted annually — no mention of version control or audit trails. |

---

## ➂ Summary of Gaps Identified

- Missing mention of how and where to **log incidents** (ticketing system, SIEM, shared drive?)
- No defined **incident severity levels** or escalation criteria
- Chain of custody and evidence handling needs clearer detail
- Doesn’t define **who communicates** to external stakeholders during a breach

---

## ➃ Recommendations for Improvement

1. Add **severity classification table** to prioritise response time and escalation.
2. Include **chain of custody procedures** for preserving digital evidence.
3. Specify **communication protocols**, including who informs leadership and regulators.
4. Reference a **central logging or ticketing system** to ensure auditability.
5. Include policy versioning and change history for better traceability.

---

> **Analyst Note:**  
> This review was conducted from the perspective of a junior SOC analyst evaluating the policy’s clarity and usability in real-time response. While the core structure is sound, several areas would benefit from additional specificity to support consistent action during high-pressure incidents.
