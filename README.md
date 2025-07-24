---
# Incident Response Policy Review & Simulation

![Status](https://img.shields.io/badge/status-Completed-brightgreen)
![Focus](https://img.shields.io/badge/focus-Policy%20Audit%20%26%20SOC%20Simulation-blueviolet)
![Role Simulated](https://img.shields.io/badge/role-Junior%20SOC%20Analyst-lightgrey)
![License: MIT](https://img.shields.io/badge/license-MIT-blue)

**Status:** Completed 
**Focus:** Policy Audit, SOC Simulation, Documentation & Analysis  
**Role Simulated:** Junior SOC Analyst

---

## ➀ Project Overview

This project simulates a task commonly assigned to entry-level SOC Analysts: reviewing an organisation’s Incident Response Policy (IRP) and evaluating its effectiveness in guiding real-time incident response.

The focus is not only on identifying policy gaps, but also on applying the policy to a simulated phishing alert to assess whether the documented procedures are actionable and effective in a realistic SOC environment.

---

## ➁ Real-World Objectives

This project is designed to build practical SOC skills in policy literacy, documentation analysis, and incident handling simulation. Specific objectives include:

- Understanding the structure and function of an IR policy
- Identifying strengths and weaknesses through structured review
- Simulating a common phishing scenario and walking through response phases
- Suggesting improvements based on observed limitations
- Practising clear documentation, critical thinking, and post-incident reflection

> **Analyst Note:**  
> This project was created to mirror the type of review and response task a new SOC analyst might perform during onboarding. It challenges me to not only understand policy documentation, but to think critically about how it translates into action — and whether it holds up during high-pressure incidents.

--- 


## ➂ Policy Gap Analysis

The current IR policy was evaluated for completeness, clarity, and usability. Key strengths included clear incident categories and defined roles. However, several weaknesses were found:

- No detailed containment guidance (short-term or long-term)
- Lacks severity levels or escalation procedures
- No steps for chain of custody or forensically-sound evidence handling
- Ambiguous communication paths for internal and external stakeholders

Improvements were suggested in a separate [Policy Gap Analysis](analysis/policy_gap_analysis.md) report.

---

## ➃ Simulated Phishing Incident Response

To test the policy, a phishing alert simulation was conducted. This included a suspicious ZIP attachment and a flagged malicious link. The steps followed:

- Header inspection and sandboxed link review
- VirusTotal scan of attachment hash
- Internal log correlation to confirm no execution

During this simulation, the policy was helpful in identifying roles and requiring user reporting — but lacked containment steps, communication flow, and detailed documentation procedures.

Full documentation is available in the [Phishing Simulation](simulation/phishing_alert_simulation.md) report.

---


## ➄ Final Reflection & Takeaways

This project gave me insight into an often-overlooked SOC task: evaluating the quality and applicability of internal security documentation. While policy analysis isn’t as flashy as malware reversing or log correlation, it’s a foundational skill — because weak policy leads to weak response.

By simulating a phishing alert and walking through the incident lifecycle, I learned how real-world decisions often depend on policy clarity. The simulation revealed several gaps that could delay response or create uncertainty for a junior analyst in a live environment without strong team support.

Key lessons included:

- How to think critically about incident response beyond the textbook lifecycle
- Where policies tend to fall short — and how to document those weaknesses clearly
- The value of structured, clear communication in a real security workflow

> **Analyst Note:**  
> This wasn’t just an academic exercise — it was an opportunity to practise the real mindset expected in a SOC. Document-driven thinking, self-sufficiency, and the ability to improve existing processes are what I aim to bring to every alert I touch.

---

## 🧾 About the Author

**Hussien Kofi**  
Aspiring SOC Analyst | Policy-Aware | Alert-Focused  

📧 [Hussienkofi@gmail.com](mailto:Hussienkofi@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/hussien-kofi-99a012330/)  
💻 [GitHub Portfolio](https://github.com/Hussien-K11)

**This project is part of an ongoing cybersecurity portfolio focused on practical, entry-level SOC analyst responsibilities — from threat detection and policy analysis to documentation and simulation.**
