# Partner Integration Brief

A short document to align product, engineering and the partner on what an integration should do, who owns what, and how success is measured. Replace everything in [brackets].

| | |
|---|---|
| **Integration name** | [Our product ↔ Partner system] |
| **Partner** | [Company, product/module] |
| **Version / date** | 0.1 / [YYYY-MM-DD] |
| **Product owner** | [Name] |
| **Partner contact** | [Name, role] |
| **Technical lead(s)** | [Our side / partner side] |
| **Status** | Discovery / In design / In build / In test / Live |

---

## 1. Why this integration

- **Customer problem:** [What customers cannot do today because the systems are separate]
- **Business value for us:** [Differentiation, pipeline, retention, vertical strategy]
- **Business value for the partner:** [What they gain, so the partnership is mutual]
- **Target customers:** [Segment and examples of who will use it]

## 2. Scope

**In scope (v1)**
1. [Use case, e.g. look up a customer record while handling an interaction]
2. [Use case, e.g. create or update a case from within our product]

**Out of scope (v1)**
1. [Deferred use case]
2. [Deferred use case]

## 3. User scenarios

| # | Persona | Scenario | Trigger | Outcome |
|---|---------|----------|---------|---------|
| 1 | [Agent] | [..] | [Incoming interaction] | [Data shown / action taken] |
| 2 | [Admin] | [..] | [Setup] | [Integration connected] |

## 4. What each side provides

| | We provide | Partner provides |
|---|-----------|------------------|
| **Data** | [Events, interaction data] | [Customer, account, case data] |
| **Actions** | [UI components, triggers] | [APIs, webhooks] |
| **Documentation** | [Setup guide] | [API docs, sandbox access] |
| **Support** | [Tier-1 support, escalation] | [Technical contact, SLA] |

## 5. Technical overview

- **Architecture:** [Direct API / middleware / marketplace connector / webhook]. Add a simple diagram.
- **Authentication and permissions:** [OAuth 2.0 / API key / SSO; scopes and roles required]
- **Data flow:**

| Data | Direction | Frequency / trigger | Format |
|------|-----------|---------------------|--------|
| [Customer record] | Partner → Us | On demand | [JSON / REST] |
| [Case update] | Us → Partner | On event | [..] |

- **Environments:** [Sandbox available? Test accounts? Who provisions them?]
- **Rate limits and performance:** [Known limits, expected volume, latency target]
- **Error handling:** [Retries, fallbacks, what the user sees when the partner is down]

## 6. Security, privacy and compliance

- **Data handled:** [Types of data; flag any personal or regulated data]
- **Data residency and retention:** [Where stored, for how long]
- **Compliance requirements:** [Industry and regional rules that apply]
- **Review needed:** [Security review, legal/DPA, partner agreement]

## 7. Commercial and legal (high level)

- **Partnership type:** [Technology partner / reseller / marketplace listing]
- **Agreements required:** [NDA, partner agreement, data processing agreement]
- **Pricing / packaging impact:** [Included, add-on, partner-billed]
- **Co-marketing:** [Joint messaging, listing, event presence]

## 8. Dependencies and risks

| Dependency / risk | Impact | Mitigation | Owner |
|-------------------|--------|------------|-------|
| [Partner API not ready] | [Delay] | [Mock the API; phase delivery] | [..] |
| [Customer needs custom fields] | [Scope creep] | [Standard fields in v1, extensibility later] | [..] |
| [Partner roadmap change] | [Breaking change] | [Versioned API, change notification process] | [..] |

## 9. Success metrics

| Metric | Target | Timeframe |
|--------|--------|-----------|
| [Customers with the integration live] | [..] | [..] |
| [Active usage by eligible users] | [..%] | [..] |
| [Time saved per interaction] | [..] | [..] |
| [Integration error rate] | [<..%] | [..] |

## 10. Milestones

| Milestone | Date | Owner |
|-----------|------|-------|
| Discovery and scope agreed | [..] | [..] |
| Technical design approved | [..] | [..] |
| Sandbox integration working | [..] | [..] |
| Pilot customer live | [..] | [..] |
| General availability | [..] | [..] |

## 11. Open questions

| # | Question | Owner | Needed by | Answer |
|---|----------|-------|-----------|--------|
| 1 | [..] | [..] | [..] | [Pending] |
