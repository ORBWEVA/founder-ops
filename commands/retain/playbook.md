---
name: retain playbook
description: Full retention playbook — audit, prioritize, and act
---

Run the Retention Playbook exercise from `~/.claude/skills/retention/SKILL.md` (Stage 4: Retention Playbook).

1. Run the retention audit: collect current churn rate, NPS, activation rate, time to aha, DAU/MAU
2. Walk through the health check (onboarding emails, usage-drop detection, surveys, cohort review, churn tracking, win-back, expansion triggers)
3. Count missing items and prioritize using the retention priority stack:
   - Activation first (if rate < 40%)
   - Involuntary churn (failed payments)
   - Early churn (M1 drop > 40%)
   - Mid-term churn (M3-6 declining)
   - Expansion (NRR < 100%)
4. For their top priority, generate specific actions with timelines
5. Reference other retain commands for implementation (/retain:emails, /retain:nps, /retain:cohort)

Retention is the foundation. Acquiring users into a leaky bucket is expensive waste.
