---
name: legal-essentials
description: Legal templates and compliance checklists for startups. Use when user needs terms of service, privacy policy, contractor agreements, or compliance guidance. Triggers on "terms of service", "privacy policy", "ToS", "GDPR", "SOC2", "compliance", "legal", "contractor agreement", "NDA", or /legal commands. NOT legal advice — templates and checklists that point founders to the right conversations with lawyers.
---

# Legal Essentials Skill

Legal templates and compliance checklists for startups. Every template includes "TALK TO A LAWYER ABOUT" flags for items that require professional review.

**Disclaimer:** This skill generates templates and checklists, NOT legal advice. Always have a qualified attorney review legal documents before publishing or signing them.

## Commands

| Command | What it does |
|---------|-------------|
| `/legal:terms` | Terms of Service template with customization |
| `/legal:privacy` | Privacy Policy generator (GDPR, CCPA, LGPD aware) |
| `/legal:contracts` | Contractor/advisor agreement templates |
| `/legal:compliance` | Compliance checklist (GDPR, SOC2, HIPAA, PCI) |
| `/legal:help` | Command reference |

---

## Stage 1: Terms of Service (`/legal:terms`)

**Goal:** Generate a ToS template customized to the product type.

### ToS Template Structure

```
TERMS OF SERVICE TEMPLATE
===========================
Customize for: [SaaS / Marketplace / API / Mobile App / E-commerce]

SECTION 1: ACCEPTANCE OF TERMS
  - Who can use the service (age, jurisdiction)
  - How acceptance works (checkbox, continued use)
  - Authority to accept on behalf of organization

SECTION 2: SERVICE DESCRIPTION
  - What the service does (plain language)
  - What it does NOT do (limitations)
  - Service availability commitment (uptime target)

SECTION 3: ACCOUNTS
  - Registration requirements
  - Account security responsibility
  - Account termination (by user and by you)

SECTION 4: ACCEPTABLE USE
  - Prohibited activities (abuse, scraping, illegal use)
  - Content guidelines (if UGC)
  - Rate limits / fair use

SECTION 5: PAYMENT TERMS (if applicable)
  - Pricing and billing cycle
  - Free trial terms
  - Refund policy
  - Price change notification period
  ⚠ TALK TO A LAWYER: Auto-renewal laws vary by jurisdiction
    (CA, EU have specific requirements)

SECTION 6: INTELLECTUAL PROPERTY
  - Your IP (service, brand, content)
  - User's IP (their data, their content)
  - License grants (both directions)
  ⚠ TALK TO A LAWYER: IP ownership for AI-generated content
    is still evolving legally

SECTION 7: DATA AND PRIVACY
  - Reference to Privacy Policy
  - Data processing summary
  - Data portability (can users export?)

SECTION 8: DISCLAIMERS AND LIABILITY
  - "AS IS" disclaimer
  - Limitation of liability
  - Indemnification
  ⚠ TALK TO A LAWYER: Liability caps and enforceability
    vary significantly by jurisdiction

SECTION 9: TERMINATION
  - How either party can terminate
  - What happens to data after termination
  - Surviving provisions

SECTION 10: DISPUTES
  - Governing law (jurisdiction)
  - Dispute resolution (arbitration vs courts)
  - Class action waiver (if applicable)
  ⚠ TALK TO A LAWYER: Arbitration clauses and class action
    waivers have different enforceability globally

SECTION 11: CHANGES TO TERMS
  - How you'll notify users of changes
  - Minimum notice period (30 days recommended)
  - Continued use = acceptance

SECTION 12: CONTACT
  - Legal contact email
  - Physical address (required in some jurisdictions)
```

### Output
Deliver: Customized ToS template + "talk to a lawyer" flags + jurisdiction-specific notes.

---

## Stage 2: Privacy Policy (`/legal:privacy`)

**Goal:** Generate a privacy policy that covers GDPR, CCPA, and general best practices.

### Privacy Policy Template

```
PRIVACY POLICY TEMPLATE
=========================
Customize for: [Jurisdictions served: US / EU / UK / AU / Global]

SECTION 1: WHAT WE COLLECT
  Personal information:
    [ ] Name, email (account registration)
    [ ] Payment info (processed by [Stripe/etc] — we don't store cards)
    [ ] IP address, device info (automatic)
    [ ] Usage data, analytics (automatic)
    [ ] Cookies and tracking (see Cookie section)
    [ ] User-generated content
    [ ] Other: ___

  Sensitive data:
    [ ] None collected
    [ ] Health data → HIPAA considerations
    [ ] Financial data → PCI considerations
    [ ] Children's data → COPPA considerations
    ⚠ TALK TO A LAWYER if collecting any sensitive data category

SECTION 2: HOW WE USE IT
  - Provide and improve the service
  - Process payments
  - Send transactional emails (receipts, password resets)
  - Send marketing emails (with opt-out)
  - Analytics and product improvement
  - Legal compliance
  ⚠ AI/ML: If you train models on user data, disclose this explicitly

SECTION 3: HOW WE SHARE IT
  - Service providers (list categories: hosting, analytics, payment)
  - Legal requirements (subpoena, court order)
  - Business transfer (acquisition, merger)
  - With user consent
  - We do NOT sell personal data [if true]

SECTION 4: DATA RETENTION
  - Active account data: retained while account is active
  - After deletion: [30/60/90] days then permanently deleted
  - Backups: purged within [X] days of deletion
  - Legal holds: retained as required by law

SECTION 5: YOUR RIGHTS
  GDPR (EU/UK users):
    [ ] Right to access
    [ ] Right to rectification
    [ ] Right to erasure ("right to be forgotten")
    [ ] Right to restrict processing
    [ ] Right to data portability
    [ ] Right to object
    [ ] Right to withdraw consent
    Contact: [DPO email or privacy@company.com]

  CCPA (California users):
    [ ] Right to know what's collected
    [ ] Right to delete
    [ ] Right to opt-out of sale
    [ ] Right to non-discrimination
    Contact: [privacy@company.com]

SECTION 6: COOKIES
  Essential cookies: [always on, required for service]
  Analytics cookies: [opt-in in EU, list tools: GA4, Mixpanel, etc.]
  Marketing cookies: [opt-in, list tools]
  Cookie consent: [banner/tool used]

SECTION 7: SECURITY
  - Encryption in transit (TLS)
  - Encryption at rest
  - Access controls
  - Incident response plan
  ⚠ Don't over-promise. "Industry-standard security measures" is safer
    than specific claims you might not maintain.

SECTION 8: INTERNATIONAL TRANSFERS
  - Where data is stored (region/country)
  - Transfer mechanisms (SCCs, adequacy decisions)
  ⚠ TALK TO A LAWYER: EU→US data transfers require specific
    legal mechanisms post-Schrems II

SECTION 9: CHILDREN
  - Service is not directed at children under [13/16]
  - COPPA compliance statement (if US users)
  ⚠ TALK TO A LAWYER if any users might be under 16

SECTION 10: CHANGES AND CONTACT
  - Notification method for policy changes
  - Effective date
  - Contact: [privacy email, physical address]
```

### Output
Deliver: Customized privacy policy template + jurisdiction flags + "talk to a lawyer" items.

---

## Stage 3: Contracts (`/legal:contracts`)

**Goal:** Templates for the most common startup contracts.

### Contractor Agreement

```
CONTRACTOR AGREEMENT TEMPLATE
================================
⚠ TALK TO A LAWYER: Misclassifying employees as contractors
  has significant legal and tax consequences.

KEY SECTIONS:
  1. Scope of work (specific deliverables, not open-ended)
  2. Compensation (rate, payment schedule, invoicing process)
  3. Term (start date, end date or termination notice)
  4. IP assignment (work product belongs to company)
  5. Confidentiality (NDA built in)
  6. Non-compete / non-solicit (if applicable, jurisdiction-dependent)
  7. Independent contractor status (not an employee)
  8. Insurance and liability
  9. Termination (notice period, payment for completed work)

CONTRACTOR vs EMPLOYEE CHECKLIST:
  Contractor signals:
    [ ] Sets own schedule
    [ ] Uses own equipment
    [ ] Works for multiple clients
    [ ] Paid per project, not salary
    [ ] No benefits provided

  Employee signals (even if called "contractor"):
    [ ] Company sets hours
    [ ] Company provides equipment
    [ ] Works exclusively for you
    [ ] Paid regular salary
    [ ] Integrated into team structure

  If 3+ employee signals: ⚠ RECLASSIFICATION RISK — talk to a lawyer.
```

### Advisor Agreement

```
ADVISOR AGREEMENT TEMPLATE
=============================
KEY TERMS:
  Role:           [Advisor type: strategic, technical, industry]
  Time commitment: [X hours/month — typically 2-5 for startups]
  Term:           [1-2 years with renewal option]
  Compensation:   [Equity: 0.1-0.5% typical for advisors, 4-year vest]

  Vesting schedule:
    Standard: 4-year vest, 1-year cliff
    Advisor-specific: 2-year vest, no cliff (more common)

SECTIONS:
  1. Role and expectations (specific, not vague)
  2. Equity grant (amount, vesting, exercise terms)
  3. Confidentiality
  4. IP assignment (if they create anything)
  5. Non-compete (usually light or none for advisors)
  6. Termination (what happens to vested equity)
```

### NDA (Mutual)

```
MUTUAL NDA TEMPLATE
=====================
KEY SECTIONS:
  1. Definition of confidential information
  2. Obligations (protect, don't disclose, limit access)
  3. Exclusions (public info, independently developed, required by law)
  4. Term (2-3 years typical)
  5. Return/destruction of information
  6. Remedies (injunctive relief)

⚠ VCs rarely sign NDAs. Don't send one before a pitch meeting.
   NDAs are for: partnerships, vendor evaluations, acquisitions.
```

### Output
Deliver: Requested contract template + customization prompts + "talk to a lawyer" flags.

---

## Stage 4: Compliance (`/legal:compliance`)

**Goal:** Checklists for common compliance frameworks. NOT certification — awareness of what's needed.

### Compliance Framework Selector

```
WHICH COMPLIANCE DO YOU NEED?
================================
Serving EU customers?           → GDPR (mandatory)
Serving California customers?   → CCPA (if >$25M revenue or >50K users)
Processing health data?         → HIPAA (mandatory in US)
Processing payment cards?       → PCI DSS (mandatory)
Selling to enterprise?          → SOC 2 (expected by buyers)
Serving UK customers?           → UK GDPR (similar to EU GDPR)
Serving Brazil customers?       → LGPD (similar to GDPR)
Serving Australia customers?    → APPs (Privacy Act 1988)
```

### GDPR Checklist

```
GDPR COMPLIANCE CHECKLIST
============================
LEGAL BASIS
  [ ] Identified legal basis for each processing activity
      (consent, contract, legitimate interest, legal obligation)
  [ ] Consent mechanism is opt-in, not opt-out
  [ ] Consent is specific, informed, and freely given
  [ ] Users can withdraw consent easily

DATA RIGHTS
  [ ] Process for handling access requests (30-day deadline)
  [ ] Process for handling deletion requests
  [ ] Data portability (export in machine-readable format)
  [ ] Right to object mechanism

DOCUMENTATION
  [ ] Data processing register (what, why, how, how long)
  [ ] Privacy impact assessment (for high-risk processing)
  [ ] Data protection officer appointed (if required)
  [ ] Sub-processor list published

TECHNICAL
  [ ] Encryption at rest and in transit
  [ ] Access controls and audit logs
  [ ] Data breach notification process (72-hour deadline)
  [ ] Data minimization (only collect what you need)
  [ ] Cookie consent banner (with reject option)

VENDOR
  [ ] Data Processing Agreements with all sub-processors
  [ ] Sub-processors listed in privacy policy
  [ ] Transfer mechanisms for non-EU data flows

⚠ TALK TO A LAWYER: GDPR fines can be up to 4% of global revenue.
  Get professional review before launching in EU.
```

### SOC 2 Readiness Checklist

```
SOC 2 READINESS (Type II)
===========================
SOC 2 isn't legally required, but enterprise customers expect it.
Type II = audited over time (6+ months). More credible than Type I.

TRUST CRITERIA:
  Security (required):
    [ ] Access controls (MFA, role-based access)
    [ ] Network security (firewalls, VPN)
    [ ] Change management process
    [ ] Incident response plan
    [ ] Vulnerability management (scanning, patching)
    [ ] Encryption (at rest + in transit)

  Availability (if SaaS):
    [ ] Uptime monitoring
    [ ] Disaster recovery plan
    [ ] Backup and restore tested
    [ ] Capacity planning

  Confidentiality:
    [ ] Data classification policy
    [ ] NDA with employees/contractors
    [ ] Data retention and destruction policy

  Processing Integrity:
    [ ] Input validation
    [ ] Error handling
    [ ] Quality assurance process

  Privacy:
    [ ] Privacy policy published
    [ ] Consent management
    [ ] Data subject rights process

TIMELINE: 3-6 months to prepare, 6-12 months for Type II audit.
COST: $20-50K for small startups (audit + tooling).

⚠ Don't pursue SOC 2 until enterprise customers are asking for it.
  It's expensive and time-consuming for early-stage startups.
```

### Output
Deliver: Applicable compliance frameworks identified + relevant checklists + "talk to a lawyer" flags + timeline and cost estimates.

---

## Integration Notes

- **Feeds from GTM:** `/gtm:launch` checklist includes legal readiness → `/legal:terms` and `/legal:privacy` fill those gaps
- **Feeds from Startup:** `/startup:ready` flags legal gaps → `/legal:compliance` identifies what's needed
- **Feeds to Pitch:** Having compliance sorted strengthens `/pitch:deck` and reduces VC risk concerns

## Principles

1. **This is NOT legal advice.** Every template says this. Every output flags items for lawyer review.
2. **Good enough to start, not good enough to finish.** Templates get you 80% there. A lawyer gets you to 100%.
3. **Jurisdiction matters.** A US ToS doesn't work in the EU. Always ask where users are.
4. **Legal debt compounds.** Fixing compliance after scaling is 10x harder than doing it early.
5. **Don't over-engineer early.** A simple ToS and privacy policy are fine at seed stage. SOC 2 can wait until enterprise asks.
