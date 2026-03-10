---
name: legal compliance
description: Compliance checklists — GDPR, SOC2, HIPAA, PCI DSS
---

Run the Compliance exercise from `~/.claude/skills/legal-essentials/SKILL.md` (Stage 4: Compliance).

1. Ask what they sell and who they sell to (determines applicable frameworks)
2. Run the compliance framework selector to identify which apply
3. For each applicable framework, walk through the full checklist:
   - GDPR: legal basis, data rights, documentation, technical, vendor
   - SOC 2: trust criteria (security, availability, confidentiality, privacy)
   - HIPAA: if health data is involved
   - PCI DSS: if payment card data is processed
4. Identify gaps and prioritize by risk (legal exposure, customer requirements)
5. Provide timeline and cost estimates for each framework
6. Flag "TALK TO A LAWYER" items

Don't encourage over-engineering. SOC 2 can wait until enterprise customers ask. GDPR can't wait if you serve EU users.
