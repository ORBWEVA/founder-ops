---
name: hiring
description: Hiring skill for startups. Use when user needs job descriptions, interview scorecards, structured interview questions, or offer letter templates. Triggers on "job description", "hiring", "interview questions", "scorecard", "offer letter", "JD", or /hire commands.
---

# Hiring Skill

Your first 5 hires make or break the company. Structured frameworks for writing JDs, scoring candidates, running interviews, and closing offers.

## Commands

| Command | What it does |
|---------|-------------|
| `/hire:jd` | Job description writer (role-specific, bias-checked) |
| `/hire:scorecard` | Interview scorecard (Topgrading-style) |
| `/hire:interview` | Structured interview questions by role and competency |
| `/hire:offer` | Offer letter template with comp structure |
| `/hire:help` | Command reference |

---

## Stage 1: Job Description (`/hire:jd`)

**Goal:** Write JDs that attract the right people and filter the wrong ones.

### JD Template

```
JOB DESCRIPTION TEMPLATE
==========================

TITLE: [Specific role — "Senior Backend Engineer" not "Ninja Rockstar"]

HOOK (2-3 sentences):
  What's exciting about this role? What will they BUILD?
  NOT: "We're a fast-paced, dynamic company looking for..."
  YES: "You'll build the real-time collaboration engine that
       powers 2,000+ teams. Our infra handles 50K concurrent
       connections and you'll take it to 500K."

ABOUT US (3-4 sentences):
  What the company does, stage, traction, mission.
  Include: team size, funding stage, notable metrics.

WHAT YOU'LL DO (5-7 bullets):
  Specific outcomes, not vague responsibilities.
  NOT: "Manage engineering projects"
  YES: "Ship the v2 API migration that unblocks our enterprise tier"

WHAT YOU BRING (5-7 bullets):
  Split into REQUIRED (hard filters) and NICE TO HAVE.
  Required: Only list what's truly non-negotiable.
  Nice to have: Everything else (don't disguise requirements here).

  ⚠ BIAS CHECK:
  [ ] No gendered language ("ninja", "rockstar", "aggressive")
  [ ] No unnecessary degree requirements
  [ ] No years-of-experience gatekeeping (test for skill instead)
  [ ] No "culture fit" (use "culture add" instead)

COMP & BENEFITS:
  [ ] Salary range (required by law in many jurisdictions)
  [ ] Equity (range or "competitive")
  [ ] Benefits summary
  [ ] Remote/hybrid/onsite

HOW TO APPLY:
  Simple. Email with resume + [one specific ask].
  The ask should filter: "Send us a link to something you've built
  and tell us what you'd do differently" > "Cover letter"
```

### Output
Deliver: Complete JD + bias check results + suggested distribution channels.

---

## Stage 2: Interview Scorecard (`/hire:scorecard`)

**Goal:** Score candidates consistently across competencies.

### Scorecard Template

```
INTERVIEW SCORECARD
=====================
Candidate: ___
Role: ___
Interviewer: ___
Date: ___

COMPETENCIES (score 1-5):

Technical Skills
  [Competency 1]: ___/5  Notes: ___
  [Competency 2]: ___/5  Notes: ___

Problem Solving
  Analytical thinking:    ___/5  Notes: ___
  System design:          ___/5  Notes: ___

Communication
  Clarity:                ___/5  Notes: ___
  Collaboration:          ___/5  Notes: ___

Culture Add
  Values alignment:       ___/5  Notes: ___
  Growth mindset:         ___/5  Notes: ___

Role-Specific
  [Custom 1]:             ___/5  Notes: ___
  [Custom 2]:             ___/5  Notes: ___

OVERALL: ___/5
RECOMMENDATION: [ ] Strong Hire  [ ] Hire  [ ] No Hire  [ ] Strong No Hire

RED FLAGS:
  [ ] None observed
  [ ] ___

SCORING GUIDE:
  5 = Exceptional (top 5% of candidates)
  4 = Strong (would compete for this role anywhere)
  3 = Meets bar (competent, no concerns)
  2 = Below bar (gaps that would need addressing)
  1 = Significant concern (clear miss on this dimension)
```

### Output
Deliver: Role-specific scorecard with customized competencies + scoring guide.

---

## Stage 3: Interview Questions (`/hire:interview`)

**Goal:** Structured questions that assess real competency, not interview polish.

### Question Bank by Competency

```
BEHAVIORAL (past behavior predicts future behavior)
  "Tell me about a time you [relevant situation]."
  "What happened? What did you do? What was the result?"
  Follow up: "What would you do differently?"

TECHNICAL (role-specific, hands-on)
  "Walk me through how you'd architect [relevant system]."
  "Here's a problem we're actually facing: [real problem]. How would you approach it?"
  "Show me code/design/copy you're proud of. Walk me through your decisions."

PROBLEM SOLVING
  "You join on Monday. By Friday, what do you want to understand?"
  "Here's a constraint: [real business constraint]. How do you work within it?"
  "What's the hardest technical/business problem you've solved? Walk me through it."

CULTURE ADD
  "What kind of team environment brings out your best work?"
  "Tell me about a time you disagreed with a decision. What happened?"
  "What's something you believe about [field] that most people disagree with?"

MOTIVATION
  "Why this company, at this stage?"
  "What does the ideal version of this role look like in 6 months?"
  "What are you optimizing for in your next role?"

⚠ ILLEGAL / AVOID:
  Never ask about: age, marital status, children, religion,
  disability, nationality, pregnancy, sexual orientation.
  When in doubt, ask: "Is this relevant to the job?"
```

### Output
Deliver: Role-specific interview questions organized by round + scoring criteria per question.

---

## Stage 4: Offer Letter (`/hire:offer`)

**Goal:** Template for extending offers that close candidates.

### Offer Template

```
OFFER LETTER TEMPLATE
======================
ROLE: [Title]
REPORTING TO: [Manager]
START DATE: [Date]
LOCATION: [Remote/Hybrid/Onsite + location]

COMPENSATION:
  Base salary:    $___/year
  Equity:         ___ shares ([X%] of company), 4-year vest, 1-year cliff
  Signing bonus:  $___  (if applicable)
  Target bonus:   ___% of base (if applicable)

BENEFITS:
  [List actual benefits — health, dental, PTO, equipment, etc.]

EQUITY DETAILS:
  Share type:      [ISO / NSO / RSU]
  Exercise price:  $___ per share (current 409A)
  Vesting:         4 years, 1-year cliff, monthly thereafter
  Acceleration:    [Single/double trigger on acquisition, if any]

  ⚠ TALK TO A LAWYER: Equity terms have tax and legal implications.
    ISO vs NSO matters. 409A valuation must be current.

CONDITIONS:
  [ ] Background check (if applicable)
  [ ] Reference check
  [ ] Signed IP assignment agreement
  [ ] Signed confidentiality agreement

EXPIRATION: This offer expires on [date — 5-7 business days typical]
```

### Startup Equity Guide

```
EQUITY BENCHMARKS (early stage)
=================================
Role                    | Seed stage  | Series A
────────────────────────┼─────────────┼──────────
CTO / Co-founder        | 10-25%      | 2-5%
VP Engineering          | 1-3%        | 0.5-1.5%
Senior Engineer         | 0.3-1%      | 0.1-0.5%
First Sales Hire        | 0.5-1.5%    | 0.1-0.5%
First Marketing Hire    | 0.3-1%      | 0.1-0.3%
Designer                | 0.2-0.5%    | 0.05-0.2%
Operations / Admin      | 0.1-0.3%    | 0.02-0.1%
Advisor                 | 0.1-0.5%    | 0.05-0.25%

These are GUIDELINES. Adjust for: market, candidate strength,
how critical the role is to your next milestone.
```

### Output
Deliver: Customized offer letter + equity benchmarks + "talk to a lawyer" flags.

---

## Principles

1. **Write JDs for the job, not the ideal human.** Over-specifying filters out great candidates.
2. **Score before you discuss.** Fill out scorecards independently before debrief to avoid groupthink.
3. **Structured > unstructured.** Same questions, same order, same scoring for every candidate.
4. **First hires set the culture.** Hire for values and capability, not just skills.
5. **Close fast.** Good candidates have options. Extend offers within 48 hours of final interview.
