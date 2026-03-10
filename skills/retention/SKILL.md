---
name: retention
description: Customer retention and lifecycle skill. Use when user needs lifecycle email sequences, NPS/CSAT survey design, cohort analysis, or churn reduction strategies. Triggers on "retention", "lifecycle email", "NPS", "CSAT", "customer success", "onboarding emails", "win-back", or /retain commands.
---

# Retention & Lifecycle Skill

Keep the customers you worked so hard to acquire. Lifecycle email sequences, satisfaction surveys, and retention strategies.

## Commands

| Command | What it does |
|---------|-------------|
| `/retain:emails` | Lifecycle email sequences (onboarding, engagement, win-back) |
| `/retain:nps` | NPS/CSAT survey design and analysis |
| `/retain:cohort` | Cohort analysis framework and interpretation |
| `/retain:playbook` | Full retention playbook with prioritized actions |
| `/retain:help` | Command reference |

---

## Stage 1: Lifecycle Emails (`/retain:emails`)

**Goal:** Design email sequences for every stage of the customer lifecycle.

### Onboarding Sequence (Days 0-14)

```
ONBOARDING EMAILS
==================
Goal: Get user to aha moment as fast as possible.
Aha moment: [define — e.g., "completed first project", "invited a teammate"]

DAY 0 — Welcome (immediate)
  Subject: "Welcome to [Product] — here's your first step"
  Content:
    - What they can do RIGHT NOW (one specific action)
    - Link to that action (not to docs, not to a tour — the action itself)
    - Set expectation: "Over the next week, I'll send you 3 tips to get the most out of [Product]"
  CTA: [Single action that leads to aha moment]

DAY 1 — Quick win
  Subject: "[First name], try this in 2 minutes"
  Content:
    - One specific feature that delivers immediate value
    - Screenshot or GIF showing the result
    - Social proof: "[X users] did this in their first day"
  CTA: [Try this feature]

DAY 3 — Core value
  Subject: "The one thing power users do differently"
  Content:
    - The #1 behavior that correlates with retention
    - How to do it (step by step)
    - Before/after comparison
  CTA: [Do the thing]

DAY 7 — Check-in
  Subject: "How's it going with [Product]?"
  Content:
    - IF activated: "You've done [X] — here's what's next"
    - IF not activated: "I noticed you haven't tried [aha action] yet. Here's why it matters."
    - Personal tone (from founder, not "the team")
  CTA: [Next step or reply to this email]

DAY 14 — Expand or recover
  Subject (activated): "3 things you might not know about [Product]"
  Subject (not activated): "Can I help?"
  Content:
    - Activated: Advanced features, integrations, invite teammates
    - Not activated: Direct ask — "What's blocking you? Reply and I'll help."
  CTA: [Expand usage or reply for help]
```

### Engagement Sequence (ongoing)

```
ENGAGEMENT EMAILS
==================
Goal: Keep active users engaged and expanding.
Trigger: Usage-based, not time-based.

MILESTONE EMAIL
  Trigger: User hits a usage milestone
  Subject: "You just hit [milestone] — here's what that means"
  Content: Celebrate + show next level + social comparison

USAGE DROP EMAIL
  Trigger: Activity drops >50% from average for 2+ weeks
  Subject: "We miss you at [Product]"
  Content: NOT guilt. Show what they're missing (new features, team activity).
  CTA: One-click return to their workspace

FEATURE ANNOUNCEMENT
  Trigger: Ship something relevant to their usage pattern
  Subject: "New: [Feature] — built for users like you"
  Content: What it does + why it matters to THEM (based on usage)
  CTA: Try it now

EXPANSION TRIGGER
  Trigger: Approaching plan limit or team size threshold
  Subject: "[First name], your team is growing"
  Content: Show usage approaching limit + what the next tier unlocks
  Tone: Helpful, not salesy
```

### Win-Back Sequence (post-churn)

```
WIN-BACK EMAILS
=================
Goal: Re-engage churned users with new value.

DAY 30 (after churn)
  Subject: "What's changed since you left"
  Content:
    - 2-3 specific improvements since they churned
    - Acknowledge their reason for leaving (if captured)
    - Special offer: [discount / free month / extended trial]
  CTA: Come back and try [specific new thing]

DAY 90 (after churn)
  Subject: "[Product] update — thought of you"
  Content:
    - Major feature announcement or milestone
    - Customer success story relevant to their use case
  CTA: See what's new

DAY 180 (after churn) — final attempt
  Subject: "Last one from us"
  Content:
    - Respect their decision
    - Leave the door open
    - Unsubscribe option prominent
  CTA: If you ever want to come back, [link]
```

### Email Anti-Patterns

```
EMAIL MISTAKES
===============
[ ] Sending from "noreply@" — kills replies and trust
[ ] Daily emails in week 1 — overwhelming, causes unsubscribe
[ ] Feature lists instead of outcomes
[ ] Same email to activated and non-activated users
[ ] No personalization beyond first name
[ ] "Just checking in" with no value
[ ] Marketing emails to users who haven't activated yet
```

### Output
Deliver: Complete email sequence for requested lifecycle stage + subject lines + trigger conditions + anti-pattern check.

---

## Stage 2: NPS/CSAT Surveys (`/retain:nps`)

**Goal:** Measure satisfaction and identify at-risk customers.

### NPS Survey

```
NPS (NET PROMOTER SCORE)
==========================
THE QUESTION:
  "On a scale of 0-10, how likely are you to recommend [Product]
  to a friend or colleague?"

  Follow-up (required): "What's the primary reason for your score?"

SCORING:
  9-10: Promoters (loyal, will refer)
  7-8:  Passives (satisfied but not enthusiastic)
  0-6:  Detractors (at risk, may churn or badmouth)

  NPS = %Promoters - %Detractors (range: -100 to +100)

BENCHMARKS:
  >50:   Excellent (world-class)
  30-50: Great
  0-30:  Good (room to improve)
  <0:    Concerning (more detractors than promoters)

WHEN TO SEND:
  - After [X days/weeks] of active use (not immediately)
  - Quarterly for ongoing measurement
  - NOT after a support interaction (biased)
  - NOT during onboarding (too early)

SEGMENTATION:
  Always segment NPS by:
    [ ] Plan tier (free vs paid)
    [ ] Usage level (power user vs casual)
    [ ] Tenure (new vs long-term)
    [ ] Industry / role (if B2B)

  The overall NPS is less useful than the segment analysis.
```

### CSAT Survey

```
CSAT (CUSTOMER SATISFACTION SCORE)
====================================
THE QUESTION:
  "How satisfied are you with [specific interaction/feature]?"
  Scale: Very satisfied / Satisfied / Neutral / Dissatisfied / Very dissatisfied

  CSAT = (Satisfied + Very Satisfied) / Total responses × 100

WHEN TO USE CSAT vs NPS:
  NPS:  Overall relationship health (quarterly)
  CSAT: Specific touchpoint quality (after support, after feature use)

BEST PRACTICES:
  [ ] Ask about specific interactions, not the product generally
  [ ] Send within 24 hours of the interaction
  [ ] Keep to 1-2 questions max
  [ ] Always include open-text follow-up
  [ ] Act on feedback visibly ("You asked, we built")
```

### Output
Deliver: Survey design + sending triggers + scoring setup + segmentation plan + action framework for each score band.

---

## Stage 3: Cohort Analysis (`/retain:cohort`)

**Goal:** Understand retention trends over time by grouping users into cohorts.

### Cohort Table

```
COHORT RETENTION TABLE
========================
Cohort     | M0    | M1    | M2    | M3    | M4    | M5    | M6
───────────┼───────┼───────┼───────┼───────┼───────┼───────┼──────
Jan (n=__) | 100%  | ___%  | ___%  | ___%  | ___%  | ___%  | ___%
Feb (n=__) | 100%  | ___%  | ___%  | ___%  | ___%  | ___%  |
Mar (n=__) | 100%  | ___%  | ___%  | ___%  | ___%  |       |
Apr (n=__) | 100%  | ___%  | ___%  | ___%  |       |       |
May (n=__) | 100%  | ___%  | ___%  |       |       |       |
Jun (n=__) | 100%  | ___%  |       |       |       |       |

WHAT TO LOOK FOR:
  ✓ Newer cohorts retain better than older ones → product improving
  ✓ Curves flatten after Month X → retained core exists
  ✗ Newer cohorts retain worse → product or market degrading
  ✗ No flattening → no retained core (PMF issue)
  ✗ Big drop at Month 1 → onboarding problem
```

### Interpretation Guide

```
COMMON COHORT PATTERNS
========================
Pattern: "The Cliff"
  Shape: Sharp drop in M1, then gradual decline
  Meaning: Onboarding failure — users don't reach aha moment
  Fix: Improve first-run experience, reduce time-to-value

Pattern: "The Plateau"
  Shape: Moderate drop, then flattens at X%
  Meaning: You have a retained core. Those users have PMF.
  Fix: Get MORE users to look like the retained segment.

Pattern: "The Smile"
  Shape: Drop, then curve back up
  Meaning: Re-engagement is working (emails, notifications, new features)
  Fix: Double down on re-engagement. Investigate what brings them back.

Pattern: "The Slide"
  Shape: Continuous decline, never flattens
  Meaning: No PMF. Users try it and leave permanently.
  Fix: Go back to /discovery:interview. Something fundamental is wrong.
```

### Output
Deliver: Cohort table + pattern identification + root cause analysis + specific actions.

---

## Stage 4: Retention Playbook (`/retain:playbook`)

**Goal:** Prioritized retention strategy customized to the product.

### Retention Audit

```
RETENTION AUDIT
================
Current metrics:
  Monthly churn rate:            ___%
  NPS score:                     ___
  Activation rate:               ___%
  Time to aha moment:            ___
  DAU/MAU ratio:                 ___

HEALTH CHECK:
  [ ] Onboarding emails set up and personalized
  [ ] Usage-drop detection and alert system
  [ ] NPS/CSAT survey running quarterly
  [ ] Cohort analysis reviewed monthly
  [ ] Churn reasons categorized and tracked
  [ ] Win-back sequence active
  [ ] Expansion triggers identified

Missing items: ___/7 — prioritize in this order.
```

### Retention Priority Stack

```
RETENTION PRIORITIES (fix in this order)
==========================================
1. ACTIVATION (if activation rate < 40%)
   → Users who don't activate WILL churn. Fix this first.
   → Actions: /retain:emails (onboarding sequence)

2. INVOLUNTARY CHURN (if failed payments > 2% of churn)
   → Easiest win. Set up dunning emails and card retry.
   → Actions: Payment retry logic + dunning sequence

3. EARLY CHURN (if M1 drop > 40%)
   → Onboarding isn't working. Users don't see value fast enough.
   → Actions: Reduce time-to-value, improve first-run experience

4. MID-TERM CHURN (if M3-6 retention declining)
   → Users saw value but it faded. Feature depth or habit issue.
   → Actions: Engagement emails, feature discovery, usage milestones

5. EXPANSION (if NRR < 100%)
   → Existing users aren't growing. Upsell opportunities missing.
   → Actions: Usage-based upgrade triggers, team invite flows
```

### Output
Deliver: Retention audit + prioritized action plan + specific email/survey/process recommendations.

---

## Principles

1. **Retention is the foundation.** Acquiring users into a leaky bucket is expensive waste.
2. **Activate before you engage.** No amount of lifecycle emails fixes a broken onboarding.
3. **Segment everything.** Overall retention hides segment-level truths.
4. **Ask, then act visibly.** Surveys without follow-through erode trust.
5. **Win-back is cheaper than acquisition.** Churned users already know your product.
