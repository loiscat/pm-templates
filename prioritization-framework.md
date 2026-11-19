# Prioritization Framework (RICE + MoSCoW)

Use **RICE** to rank a long list of ideas with numbers. Use **MoSCoW** to decide what goes into a specific release. They work well together: RICE ranks, MoSCoW draws the line.

---

## 1. RICE

**Score = (Reach × Impact × Confidence) ÷ Effort**

| Factor | Question | How to score |
|--------|----------|--------------|
| **Reach** | How many users or customers will this affect in a given period? | A real number (e.g. 500 customers per quarter) |
| **Impact** | How much will it move the goal for each person reached? | 3 = massive, 2 = high, 1 = medium, 0.5 = low, 0.25 = minimal |
| **Confidence** | How sure are we about Reach and Impact? | 100% = solid data, 80% = some evidence, 50% = gut feeling |
| **Effort** | How much work across product, design and engineering? | Person-months (or sprints) |

### Template

| # | Idea / Feature | Reach | Impact | Confidence | Effort | RICE score | Notes |
|---|----------------|-------|--------|------------|--------|------------|-------|
| 1 | [Name] | [..] | [..] | [..%] | [..] | [calc] | [Evidence, dependencies] |
| 2 | [Name] | [..] | [..] | [..%] | [..] | [calc] | [..] |

### Worked example (fictional product: "Acme Support Hub")

| # | Idea | Reach | Impact | Confidence | Effort | RICE score |
|---|------|-------|--------|------------|--------|------------|
| 1 | Saved reply suggestions | 800 | 1 | 80% | 2 | **320** |
| 2 | Custom dashboard colors | 1,000 | 0.25 | 100% | 1 | **250** |
| 3 | CRM sync for open cases | 400 | 2 | 50% | 4 | **100** |

Reading it: idea 1 wins because it reaches many people, has decent impact and is cheap. Idea 3 has the biggest impact per user, but low confidence and high effort pull it down. The right next step may be to **raise confidence** (interviews, a prototype), not to build it.

### Tips
- Fix the time period for Reach (per quarter, per month) and use it for every row.
- Score as a group (product, design, engineering). Disagreements are useful information.
- RICE is an input to the decision, not the decision. Strategic bets and dependencies can override a score, but say so explicitly.

---

## 2. MoSCoW

Use it to scope a release.

| Category | Meaning | Rule of thumb |
|----------|---------|---------------|
| **Must have** | Without it, the release has no value or cannot ship (legal, security, core flow) | Keep to about 60% of the effort |
| **Should have** | Important, but there is a workaround if it slips | About 20% |
| **Could have** | Nice to have, first to be cut | About 20% |
| **Won't have (this time)** | Agreed as out of scope for this release | Write it down to avoid scope creep |

### Template

| Requirement | Category | Why | Owner |
|-------------|----------|-----|-------|
| [Requirement] | Must | [Reason] | [Name] |
| [Requirement] | Should | [Reason] | [Name] |
| [Requirement] | Could | [Reason] | [Name] |
| [Requirement] | Won't (this time) | [Reason / revisit date] | [Name] |

---

## 3. Putting them together

1. List all ideas and score them with RICE.
2. Sort by score and review the top of the list against strategy and dependencies.
3. Pick the release scope and label each item with MoSCoW.
4. Share the Won't-haves with stakeholders so expectations are clear.
5. Revisit the scores each quarter, since reach, confidence and effort change.
