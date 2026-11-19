# [Product / Feature Name] — Product Requirements Document (PRD)

| | |
|---|---|
| **Version** | 0.1 (Draft) |
| **Date** | [YYYY-MM-DD] |
| **Author(s)** | [Name, role] |
| **Contributors** | [Design, Engineering, Partner/Integration, Customer Success, Legal/Compliance] |
| **Status** | Draft / In review / Approved |
| **Target release** | [Quarter or date] |

> **How to use this template:** Replace everything in [brackets]. Delete sections that don't apply. Keep each section short; if a section needs more than a page, link to a separate document. Never include customer data or confidential company information in a public copy.

---

## 1. Purpose of this document

[2–3 sentences: what this document defines, who it is for, and what decision or alignment it should unlock. State whether it is a discussion artifact open for input or a final specification.]

## 2. Keywords and definitions

| Term | Definition |
|------|------------|
| [Term] | [Plain-language definition] |
| [Term] | [Plain-language definition] |

## 3. Executive summary

- **Job to be done:** [What the user is trying to get done, in one sentence.]
- **Pain:** [What makes it hard today: fragmented systems, manual work, missing visibility, risk.]
- **Gain:** [What changes for the user and for the business if we solve it.]
- **Why now:** [Market, customer, partner or strategic trigger.]

## 4. Goals and non-goals

**Goals**
1. [Outcome the release must achieve]
2. [Outcome the release must achieve]

**Non-goals (explicitly out of scope)**
1. [Thing people might expect but we are not doing]
2. [Thing deferred to a later phase]

## 5. Personas and target customers

### [Persona 1, e.g. Agent / Advisor / Operator]
- **Motivations:** [What they care about]
- **Pain points:** [What blocks them today]
- **How they will use this:** [Context and frequency]

### [Persona 2, e.g. End customer / Admin / Partner]
- **Motivations:** [...]
- **Pain points:** [...]
- **How they will use this:** [...]

### Target segment (vertical)
[Industry, company size, region, and the buying/decision roles involved.]

## 6. User journey

[Insert a simple journey map or diagram showing the key steps for each persona. A few boxes and arrows is enough.]

| Step | Persona | What they do | What the product does | Pain removed |
|------|---------|--------------|-----------------------|--------------|
| 1 | [..] | [..] | [..] | [..] |
| 2 | [..] | [..] | [..] | [..] |

## 7. Solution overview and feature list

| # | Feature | Description | Priority (Must / Should / Could) | Phase |
|---|---------|-------------|----------------------------------|-------|
| 1 | [Feature] | [One sentence] | Must | MVP |
| 2 | [Feature] | [One sentence] | Should | MVP |
| 3 | [Feature] | [One sentence] | Could | Later |

## 8. Use cases and requirements

> Tip: if you manage stories in Jira (or similar), keep one line per story here and link to the ticket.

### 8.1 [Feature area A]
| ID | User story | Acceptance criteria | Link |
|----|------------|---------------------|------|
| A-1 | As a **[persona]**, I can **[action]** so that **[benefit]**. | [Testable condition] | [Ticket] |
| A-2 | As a **[persona]**, I can **[action]** so that **[benefit]**. | [Testable condition] | [Ticket] |

### 8.2 [Feature area B]
| ID | User story | Acceptance criteria | Link |
|----|------------|---------------------|------|
| B-1 | As a **[persona]**, I can **[action]** so that **[benefit]**. | [Testable condition] | [Ticket] |

### 8.3 Admin and setup
| ID | User story | Acceptance criteria | Link |
|----|------------|---------------------|------|
| S-1 | As an **admin**, I can **[configure ...]** so that **[...]**. | [Testable condition] | [Ticket] |

## 9. Integrations and partner dependencies

| System / partner | What we need from it | What we provide | Owner | Status / risk |
|------------------|----------------------|-----------------|-------|---------------|
| [e.g. CRM, ERP, EHR] | [APIs, data, auth] | [Events, UI, actions] | [Name] | [Not started / In progress / Blocked] |

- **Authentication and permissions:** [OAuth scopes, roles, SSO]
- **Data flow:** [What data moves, in which direction, how often]

## 10. Non-functional requirements

- **Security and privacy:** [Data handling, PII, retention, access control]
- **Compliance:** [Industry regulations that apply, e.g. HIPAA, GDPR, SOC 2]
- **Performance and reliability:** [Latency, availability, scale expectations]
- **Accessibility and localization:** [Languages, accessibility standards]

## 11. Rollout and launch plan

- **Release strategy:** [Feature flag, beta customers, phased rollout, general availability]
- **Prerequisites:** [Account settings, flags, configuration needed before use]
- **Enablement:** [Documentation, training, demo environment, sales and support readiness]
- **Go-to-market:** [Positioning, announcement channel, event or launch moment]

## 12. Success metrics

| Metric | Baseline | Target | Timeframe | How measured |
|--------|----------|--------|-----------|--------------|
| [Adoption, e.g. % of eligible users active] | [..] | [..] | [e.g. 6 months] | [Tool / report] |
| [Efficiency, e.g. time per task] | [..] | [..] | [..] | [..] |
| [Business, e.g. pipeline, revenue, retention] | [..] | [..] | [..] | [..] |
| [Validation, e.g. number of design partners live] | [..] | [..] | [..] | [..] |

## 13. Competitive analysis (optional)

| Capability | Us | Competitor A | Competitor B |
|------------|----|--------------|--------------|
| [Capability] | [..] | [..] | [..] |

**Where we differentiate:** [One or two sentences.]

## 14. Assumptions, risks and limitations

**Assumptions**
- [What we believe to be true but have not validated]

**Risks and mitigations**
| Risk | Likelihood / Impact | Mitigation | Owner |
|------|---------------------|------------|-------|
| [Customization requests delay delivery] | Medium / High | [Standardize core features; set clear boundaries with partners] | [Name] |
| [Dependency on partner API] | [..] | [..] | [..] |

**Limitations**
- [Known constraints of the MVP]

## 15. Open questions

| # | Question | Owner | Needed by | Answer |
|---|----------|-------|-----------|--------|
| 1 | [Question] | [Name] | [Date] | [Pending] |

## 16. Acceptance criteria for the release

- [ ] Functionality validated by [partner users / pilot customers]
- [ ] All Must-have requirements delivered and tested
- [ ] Security, privacy and compliance review completed
- [ ] Documentation and enablement materials ready
- [ ] Feedback from internal stakeholders and partners incorporated

## 17. Appendix

- Links: [designs, Jira epic, research, related PRDs]
- Revision history:

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 0.1 | [Date] | [Name] | Initial draft |
