# User Stories and Acceptance Criteria Guide

How to write requirements that engineers can build, QA can test, and stakeholders can understand.

---

## 1. The user story format

> As a **[persona]**, I can **[action]** so that **[benefit]**.

| Part | What to write | Common mistake |
|------|---------------|----------------|
| **Persona** | A specific role (Agent, Admin, Customer) | "As a user" for everything |
| **Action** | What the person does, in plain language | Describing the solution or the technology |
| **Benefit** | Why it matters to them | Leaving it out, or repeating the action |

### Good vs. bad

| ❌ Weak | ✅ Better |
|---------|----------|
| As a user, I can use the dashboard. | As a **support agent**, I can see all my open cases sorted by urgency so that I handle the most critical customers first. |
| As a developer, I need an API endpoint for cases. | As an **admin**, I can connect our CRM to the platform so that case data appears automatically during interactions. |
| As a user, I want the system to be fast. | As an **agent**, I can see customer details within 2 seconds of an interaction starting so that I can greet the customer by context. *(Non-functional requirement, with a measurable target.)* |

---

## 2. INVEST checklist

A good story is:

| Letter | Meaning | Ask yourself |
|--------|---------|--------------|
| **I** | Independent | Can it be built without waiting on another story? |
| **N** | Negotiable | Is it about the outcome, leaving room for how? |
| **V** | Valuable | Does a real user or the business benefit? |
| **E** | Estimable | Can the team size it? If not, is it too vague? |
| **S** | Small | Can it be finished in one sprint? If not, split it. |
| **T** | Testable | Can we tell, clearly, when it's done? |

---

## 3. Acceptance criteria

Acceptance criteria define **when the story is done**. Write them before development starts.

### Format A: Given / When / Then (best for flows and behavior)

> **Given** [starting context], **when** [action], **then** [expected result].

**Example**
- **Given** an agent is on an active interaction, **when** the CRM returns a matching customer, **then** the customer's name and open cases appear in the side panel.
- **Given** the CRM is unavailable, **when** an interaction starts, **then** the agent sees a "Customer data unavailable" message and can still handle the interaction.

### Format B: Checklist (best for simple or UI-focused stories)

- [ ] The panel shows name, account status and the last 5 cases
- [ ] Cases are sorted by most recent
- [ ] The panel loads within 2 seconds
- [ ] Works in supported browsers: [list]

### Rules of thumb
- 3–7 criteria per story. More than that usually means the story is too big.
- Each criterion must be **testable**: a yes or no answer, not "should be intuitive".
- Cover the **happy path**, the **error path** and the **empty state**.
- Include **permissions** (who can and cannot do this).
- State **measurable** targets for performance, not adjectives.

---

## 4. Story template

| Field | Content |
|-------|---------|
| **ID / Title** | [AREA-123] [Short name] |
| **Story** | As a **[persona]**, I can **[action]** so that **[benefit]**. |
| **Context** | [Why now, links to PRD, research or designs] |
| **Acceptance criteria** | 1. Given ... when ... then ...<br>2. Given ... when ... then ... |
| **Out of scope** | [What this story does not cover] |
| **Dependencies** | [Other stories, partners, teams] |
| **Design / assets** | [Link] |
| **Analytics / success signal** | [Event or metric that tells us it works] |
| **Priority** | Must / Should / Could |

---

## 5. Splitting large stories

If a story won't fit in a sprint, split by:

| Split by | Example |
|----------|---------|
| **Workflow step** | "Connect CRM" → authenticate, map fields, test connection |
| **User type** | Admin setup vs. agent usage |
| **Happy path first** | Core flow now, edge cases and error handling in later stories |
| **Data variation** | One data source first, others later |
| **Simple to complex** | Read-only view first, editing later |

Avoid splitting by technical layer ("backend", then "frontend"). It delivers no user value until both are finished.

---

## 6. Epics, stories and tasks

| Level | What it is | Example |
|-------|-----------|---------|
| **Epic** | A large outcome spanning many stories | CRM integration |
| **Story** | One user-visible piece of value | Agent sees customer context during an interaction |
| **Task** | Technical work to deliver a story | Build the API call, write tests |

Product owns epics and stories. Engineering usually owns the tasks.

---

## 7. Quick quality check before handing over

- [ ] Could someone unfamiliar with the project understand the story?
- [ ] Is the benefit clear?
- [ ] Are the acceptance criteria testable?
- [ ] Are error and empty states covered?
- [ ] Is it small enough for one sprint?
- [ ] Are designs and dependencies linked?
