# founder-ops

The boring stuff that kills startups.

Legal templates, hiring frameworks, and retention playbooks as Claude Code skills. 15 slash commands that generate customized documents, checklists, and strategies using YOUR context.

## What's inside

### Legal (4 commands + help)

| Command | What it does |
|---------|-------------|
| `/legal:terms` | Terms of Service template (SaaS, marketplace, API, app) |
| `/legal:privacy` | Privacy Policy generator (GDPR, CCPA, LGPD aware) |
| `/legal:contracts` | Contractor/advisor agreements and NDAs |
| `/legal:compliance` | Compliance checklists (GDPR, SOC2, HIPAA, PCI) |

### Hiring (4 commands + help)

| Command | What it does |
|---------|-------------|
| `/hire:jd` | Job description writer (bias-checked) |
| `/hire:scorecard` | Interview scorecard (consistent evaluation) |
| `/hire:interview` | Structured interview questions by competency |
| `/hire:offer` | Offer letter template with equity benchmarks |

### Retention (4 commands + help)

| Command | What it does |
|---------|-------------|
| `/retain:emails` | Lifecycle email sequences (onboarding, engagement, win-back) |
| `/retain:nps` | NPS/CSAT survey design with segmentation |
| `/retain:cohort` | Cohort analysis framework and pattern diagnosis |
| `/retain:playbook` | Full retention playbook (audit + prioritized actions) |

## Install

```bash
npx skills add ORBWEVA/founder-ops
```

Or manually copy:
- `skills/` -> `~/.claude/skills/`
- `commands/` -> `~/.claude/commands/`

## Example output

### `/legal:terms` for a SaaS product

```
TERMS OF SERVICE TEMPLATE
===========================
Customize for: SaaS (B2B)
Jurisdictions: US + EU

SECTION 5: PAYMENT TERMS
  Billing cycle: Monthly/annual, auto-renewal
  Free trial: 14 days, no CC required
  Refund: Pro-rata for annual, none for monthly

  ⚠ TALK TO A LAWYER: Auto-renewal laws vary by jurisdiction
    (CA, EU have specific notification requirements)

SECTION 8: DISCLAIMERS AND LIABILITY
  Liability cap: 12 months of fees paid
  ⚠ TALK TO A LAWYER: Liability caps have different
    enforceability in EU vs US

4 items flagged for lawyer review.
```

### `/hire:jd` for a first engineering hire

```
JOB DESCRIPTION
================
Title: Senior Backend Engineer
Hook: "You'll build the API layer that powers 2,000+ teams.
       Our infra handles 50K concurrent connections and
       you'll take it to 500K."

BIAS CHECK: ✓ PASSED
  ✓ No gendered language
  ✓ No degree requirements (skill-tested instead)
  ✓ Experience listed as "significant" not "7+ years"
  ✓ "Culture add" not "culture fit"

REQUIRED: 4 items (hard filters)
NICE TO HAVE: 3 items (not disguised requirements)
```

### `/retain:cohort` with retention data

```
COHORT RETENTION TABLE
========================
Cohort     | M0    | M1   | M2   | M3   | M4   | M5
───────────┼───────┼──────┼──────┼──────┼──────┼──────
Jan (n=84) | 100%  | 62%  | 41%  | 38%  | 37%  | 36%
Feb (n=97) | 100%  | 58%  | 43%  | 40%  | 39%  |
Mar (n=112)| 100%  | 71%  | 52%  | 48%  |      |

PATTERN: "The Plateau" — curves flatten at ~37%
TREND: Newer cohorts retain better (product improving)
CRITICAL DROP: M0→M1 (38% lost) — onboarding problem

ACTION: Fix first-run experience. The 37% who stay have PMF.
Get more users to look like them.
```

## Pairs with other ORBWEVA skills

```
/dt:empathize        → understand the user
/startup:pmf         → validate product-market fit
/gtm:positioning     → articulate who it's for
/startup:unit        → prove the economics
/legal:terms         → protect the business
/legal:privacy       → protect user data
/hire:jd             → build the team
/hire:scorecard      → evaluate consistently
/retain:emails       → keep users engaged
/retain:cohort       → measure what's working
/startup:runway      → how long you have
```

Install the full founder stack:
```bash
npx skills add ORBWEVA/dt-skill           # Design thinking
npx skills add ORBWEVA/gtm-skills         # Go-to-market + GEO + SEO
npx skills add ORBWEVA/founder-metrics    # Startup metrics
npx skills add ORBWEVA/founder-ops        # Legal + hiring + retention
npx skills add ORBWEVA/pitch-skill        # Pitch decks (coming soon)
```

## Security

Zero executable code. Pure markdown — structured prompts that guide Claude's thinking. No scripts, no dependencies, no API calls, no shell commands.

```
skills/legal-essentials/SKILL.md   # Legal templates + compliance
skills/hiring/SKILL.md             # JDs, scorecards, interviews, offers
skills/retention/SKILL.md          # Emails, NPS, cohorts, playbooks
commands/legal/*.md                # 5 slash commands
commands/hire/*.md                 # 5 slash commands
commands/retain/*.md               # 5 slash commands
package.json                       # metadata only
```

## License

MIT
