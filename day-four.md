# Day 4 Study Summary — Business Case Development for IT Projects
## Topic block: Public Sector decision-making + ECO / Sustainability

*University of Twente — covers the public-sector material from the Governance lecture (Harmelink, Lecture 07, drawing on Winkler 2013 and Sethibe et al. 2007), the ECO/sustainability content from the Ethics lecture (Effing, on the UN SDGs and ethical-impact analysis), the Herath et al. (2019) green-computing CSR paper, and the public-sector findings woven through Ryan & Gregory (2019) and Nelson (2008). This is everything you need for the public-sector and sustainability sides of a business case.*

---

## How to use this summary

Same approach as Days 1–3: read it through once, then self-test by covering the explanations and reproducing the key tables, lists, and distinctions from memory. **"Exam angle"** flags the points most likely to be tested, and sources are attributed inline (e.g. *(Winkler, 2013)*, *(Herath et al., 2019)*) with a full list at the end.

**Why these two topics share a day.** They're paired because they're the two "context" topics that make an IT business case *more than a spreadsheet* — and they're deeply linked through the **UN Sustainable Development Goals**, which are both the public-responsibility yardstick (ECO) and a major concern of public-sector decision-making. Between them they carry real exam weight: **Public Sector is 10% of the individual exam** (tied with Ethics as the single heaviest topic), and **ECO/Sustainability is 5%**. So together this day is ~15% of your written exam.

**The connections to earlier days.** Public sector was foreshadowed twice already: **Nelson (2008)** noted that *half* of the ten most infamous IT failures (>$100m losses) came from the **public sector** (Day 1), and the course manual's business-case outline tells you to **"focus on public sector problems"** (Days 1–2). Sustainability is the direct continuation of Day 3's **ethical impact analysis**, which ends by telling you to *"look at the UN sustainability goals and explicitly reflect on potential negative and positive external effects."* So the SDGs are the hinge between Day 3's ethics and Day 4's ECO.

---

# PART 1 — PUBLIC SECTOR DECISION-MAKING

The learning goal is precise: *"understand the **characteristics and complexity** of public sector decision making regarding IT"* *(Course manual, test matrix)*. The exam isn't asking you to take a side on public vs. private — it wants you to *understand why the public sector is different and harder*. The centrepiece is a comparison table; learn it well.

## 1.1 What counts as "public sector"?

First, the basic taxonomy *(Harmelink, Lecture 07, citing Sethibe, Campbell & McDonald, 2007)*. Organizations split into:

- **Private sector** → **for-profit organisations** (the private sector proper) and **non-profit organisations (NPOs)**.
- **Public sector** → **government agencies** (public service) and **semi-government agencies** (semi-government).

So "public sector" spans pure government bodies and semi-government agencies that deliver public services. This matters because public-sector business cases serve **public value**, not shareholder profit — which drives every difference below.

## 1.2 Private vs. public sector — the comparison table (Winkler, 2013) — HIGH PRIORITY

This is the single most exam-relevant artifact in the public-sector block: a table contrasting private and public sector across ten attributes, with the implications for **IT governance (ITG)** *(Harmelink, Lecture 07, citing Winkler, 2013)*. Learn the attributes and the contrast on each:

| Attribute | Private sector | Public sector |
|---|---|---|
| **Goals** | Shareholder value | **Public value / multifaceted** |
| **Stakeholders** | Few | **Many / potentially conflicting goals** |
| **Environment** | Less regulated | **Legal and formal constraints** |
| **Incentives** | High / market | **Low / "soft budgets" / scrutiny** |
| **Risks** | Lower aversion | **High aversion** |
| **Competition** | High competition | **Low / intergovernmental cooperation** |
| **IT innovation** | Competitive advantage | **Treated as a necessity** |
| **IT competencies** | Varying | **Generally lower** |
| **IT sourcing** | Flexible contracting | **Complex tendering processes** |
| **IT resources** | Proprietary IT | **Shared IT resources** |

How to read each row (and why it makes public-sector IT *harder*):

- **Goals — public value, multifaceted.** A private firm optimizes a single, clear metric (shareholder value). The public sector pursues **multiple, sometimes competing public values** (equity, access, transparency, service quality), which can't be reduced to one number. *This is why financial metrics alone never settle a public-sector business case.*
- **Stakeholders — many, potentially conflicting.** Private firms answer to relatively few stakeholders; the public sector answers to citizens, politicians, oversight bodies, other agencies — whose goals can **directly conflict**. (Recall Nelson: stakeholder management is the #2 failure cause — and the public sector has the hardest version of it.)
- **Environment — legal and formal constraints.** The public sector operates under heavy law, regulation, and procedure; it can't just move fast.
- **Incentives — low, "soft budgets," scrutiny.** Public bodies face weaker market incentives, **"soft budgets"** (budgets that can be topped up rather than hard financial discipline), and intense public/political **scrutiny** of how money is spent.
- **Risks — high aversion.** Because failures are public and politically costly, the public sector is **highly risk-averse**, which can stifle innovation.
- **Competition — low; intergovernmental cooperation.** Instead of competing, public bodies often **cooperate** across government — a different dynamic from market competition.
- **IT innovation — treated as a necessity.** Private firms use IT for **competitive advantage**; the public sector treats it as a **necessity** to deliver services, not a weapon to beat rivals.
- **IT competencies — generally lower.** Public bodies often have weaker in-house IT capability.
- **IT sourcing — complex tendering.** This is huge: the public sector can't just sign a flexible contract; it must run **formal, complex tendering/procurement processes** (legally mandated, transparent, slow).
- **IT resources — shared.** Public IT resources are often **shared** across agencies rather than proprietary to one organization.

The right-hand column of Winkler's table lists the **IT governance implications**: IT goals, alignment, **procedural mechanisms, structural mechanisms, relational mechanisms**, and **sourcing governance** — i.e., the public sector needs distinct governance mechanisms to cope with all of the above.

**Exam angle:** This is a textbook "characteristics and complexity" question. If asked how public-sector IT decision-making differs from private, structure your answer around these attributes — emphasizing the most consequential ones: **multifaceted public value (not profit), many conflicting stakeholders, heavy legal/regulatory constraints, soft budgets and scrutiny, high risk-aversion, and complex tendering/procurement.** You don't need all ten verbatim, but be able to give ~5–6 with the public-side contrast and explain *why* each adds complexity. Cite **Winkler (2013)**.

## 1.3 The complexity in practice (Ryan & Gregory's public-sector findings)

The smart-city paper from Day 3 gives concrete, citable illustrations of public-sector dynamics *(Ryan & Gregory, 2019)* — useful because they show the table's abstractions in real cases:

- **Public bodies prioritize citizen value over profit.** A telling contrast from the City Data Exchange (Copenhagen): public entities **focus on providing value to citizens**, which sometimes *hinders* the economic development a private partner (Hitachi) wanted — the private partner would have terminated the project as loss-making, but public funding kept it going beyond commercial logic. This is the "public value vs. shareholder value" row, live.
- **Job protection over pure efficiency.** The **Helsinki municipality** has an obligation to **ensure job security for staff regardless of SIS efficiency** — so its chat-bots are designed to *take strain off* employees and reallocate them to higher-value work, **not** to cut jobs. A private firm under market incentives would more likely cut. (This is the "incentives / risk-aversion / public value" rows combined.)
- **Collaboration and bottom-up.** Smart cities work best through a **public-private collaborative model** and a **bottom-up** approach with **citizen/municipal data ownership** — reflecting the public sector's many-stakeholder, cooperation-over-competition character.

**Exam angle:** If a public-sector exam question gives you a case (the example exam uses "PublicCo … digitally transforming the city of Enschede"), use these dynamics: public value over profit, many conflicting stakeholders, legal/tendering constraints, risk-aversion, job/social obligations. Concrete examples (Helsinki job protection; Copenhagen public-vs-private tension) make a stronger answer than abstractions alone.

## 1.4 Why this matters for the business case

The course manual bakes the public sector into the business-case structure: the problem/opportunity section says to **"focus on public sector problems,"** and the assessment criteria explicitly ask whether **"idiosyncrasies of the public sector are considered"** and whether the case is **"feasible for the public sector company"** *(Course manual)*. So the public-sector lens isn't a side topic — it's a quality criterion applied across the whole business case. The practical upshot: in a public-sector case you must justify value in **non-financial, multifaceted public-value terms**, account for **conflicting stakeholders and legal/procurement constraints**, and respect **risk-aversion and scrutiny** — you can't simply argue "positive NPV, therefore do it."

---

# PART 2 — ECO / SUSTAINABILITY

The learning goal: *"understand the United Nations sustainability and public responsibility goals and are able to **map them on a project**"* *(Course manual, test matrix)*. Note the verb — **map** — the exam wants you to connect an IT project to specific SDGs and reflect on its external effects, exactly the method introduced in Day 3's ethical-impact analysis.

## 2.1 The UN Sustainable Development Goals (SDGs)

The foundation *(Effing, Ethics lecture; Ryan & Gregory, 2019, citing UN 2018)*: in **2015 the UN General Assembly established 17 Sustainable Development Goals** to be reached by **2030**. They range from eliminating poverty to universal education, gender equality, and climate action. The full 17, as shown in the lecture:

1. No Poverty
2. Zero Hunger
3. Good Health and Well-being
4. Quality Education
5. Gender Equality
6. Clean Water and Sanitation
7. Affordable and Clean Energy
8. Decent Work and Economic Growth
9. Industry, Innovation and Infrastructure
10. Reduced Inequalities
11. **Sustainable Cities and Communities**
12. Responsible Consumption and Production
13. Climate Action
14. Life Below Water
15. Life on Land
16. Peace, Justice and Strong Institutions
17. Partnerships for the Goals

You don't need to memorize all 17 word-perfect, but you **should** know there are **17**, that they target **2030**, that they were set in **2015**, and you should be able to name a representative spread (poverty, education, gender equality, clean energy, reduced inequalities, sustainable cities, climate action) — and especially **Goal 11 (Sustainable Cities and Communities)**, which is the one Ryan & Gregory hang the whole smart-city case on.

**Why Goal 11 is central:** the urban population will grow by **1.5 billion by 2030** (to ~5 billion), straining resources, infrastructure, jobs and healthcare — so the UN calls for creative approaches to **reduce ecological harm, pollution and injustice** while **increasing affordable housing, infrastructure and safety**. The **smart city** is one such approach *(Ryan & Gregory, 2019, citing UN 2018)*. This is the explicit bridge between the SDGs (ECO) and smart cities (Ethics, Day 3).

**Exam angle:** For "map the SDGs to a project," the method is: pick the **specific, relevant** SDGs your IT project touches (not all 17), and reflect on **both positive and negative** external effects against each. *Example:* a smart-city sensor network maps to **Goal 11** (sustainable cities) and **Goal 7/13** (clean energy/climate) on the positive side, but might create tension with **Goal 10** (reduced inequalities — digital divide) on the negative side. Showing both directions is what scores.

## 2.2 "Public responsibility" and CSR

The learning goal pairs sustainability with **"public responsibility goals."** The conceptual backing comes from the Herath et al. (2019) green-computing paper and the CSR literature it draws on *(Herath et al., 2019)*:

- The **principle of public responsibility** (Preston & Post, 1975) holds that businesses have an **interpenetrating relationship with society** — each influences the other — so business decision-makers must take into account the **public consequences** of their decisions, including effects on the natural environment.
- **Corporate Social Responsibility (CSR)** is defined (Aguinis & Glavas, 2012) as *"context-specific organizational actions and policies that take into account stakeholders' expectations and the **triple bottom line of economic, social, and environmental performance**."* CSR is the firm's consideration of, and response to, issues **beyond the narrow economic, technical, and legal requirements** of the firm (Davis, 1973).
- The **triple bottom line** — **economic, social, environmental** — is the key memorable concept: sustainability means performing well on all three, not just the financial one.

Note this connects straight back to Day 3's **ethical strategists** (Noland & Phillips), who reject the **separation thesis** — business value and stakeholder/social value can't be cleanly separated. CSR/public responsibility is the practical expression of that idea.

**Exam angle:** Know the **triple bottom line (economic, social, environmental)** as the definition of what sustainability/CSR optimizes, and the **principle of public responsibility** (business and society interpenetrate, so decisions must weigh public/environmental consequences). These are clean, citable points.

## 2.3 The Herath et al. (2019) green-computing paper — making the business case for sustainability

This is the dedicated ECO paper, and it's important because it shows **how to put sustainability *into* a business case** rather than treating it as a moral add-on *(Herath et al., 2019)*. The paper's title is "Profit-Driven Corporate Social Responsibility as a Bayesian Real Option in Green Computing." Key ideas:

### Green computing and why it matters

**Green computing** = efficient and ecologically friendly computing practices aimed at **reducing IT costs *and* environmental impact**. The motivation: IT consumes huge amounts of electricity (a single PC can generate ~1 ton of CO₂/year), strains electric grids, adds greenhouse gases, and creates hazardous e-waste *(Herath et al., 2019)*. Practices include: proper **e-waste disposal**, **virtualization** and **cloud computing**, **reducing energy consumption**, **server consolidation/reengineering**, and futuristic ideas (carbon-free, solar, lead-free computing). Brooks et al. identify eco-goals like **eco-capacity, eco-efficiency, eco-effectiveness, eco-collaboration**.

### Profit-driven CSR: the key reframing

The central argument: green/CSR investments need **not** be seen as pure cost or charity. Following Husted (2005) and van Marrewijk (2003), the paper treats environmentally-friendly investment as a **profit-driven CSR strategy** — a **strategic investment that creates value for the firm *and* society** (a **win-win**: positive economic rewards for the business, reduced environmental harm for society). The IBM survey finding captures the shift: CSR is **no longer viewed as just a regulatory or discretionary cost, but as an investment that brings financial returns** *(Herath et al., 2019)*.

### The method: real options + Bayesian updating (links to Day 5)

This is where ECO connects to the **Tools** topic (real options, Day 5). The paper argues that a **traditional NPV** approach **ignores strategic flexibility**, so it values the green investment as a **real option**:

- A simple NPV says: if positive, invest now. In the paper's **server-consolidation case** (a university upgrading its data centre), the NPV of moving to the energy-efficient system was **positive (~$257k)**, so the naive conclusion is "invest immediately."
- But the **real option** lens captures the value of **waiting for information** — here, uncertainty about the future **carbon tax** (its level and how strictly it's enforced). The **Bayesian** twist lets the firm **update its probability estimates as new information arrives**, rather than treating uncertainty as fixed. The **strategic NPV (SNPV) = NPV + option value**, where the option value reflects exploiting the upside (e.g. carbon-tax savings) while avoiding the downside.
- Practical conclusion in the case: because the immediate CSR option value was positive and larger than the value of waiting, the university should invest **now** — but in other scenarios (e.g. strict carbon tax + low cost of capital) **waiting for more information** is worthwhile.

**Exam angle:** You likely won't need to reproduce the Bayesian maths, but you *should* be able to explain the paper's core message: **sustainability/green IT can be justified in a business case as a profit-driven CSR investment** (win-win, not just cost), and that **viewing it as a real option** (NPV + the value of flexibility/waiting for information, e.g. on carbon tax) captures strategic value that plain NPV misses. This also previews the real-options logic you'll meet fully on Day 5 — note the shared **decision-tree** technique with the risk EMV analysis from Day 2.

## 2.4 How to do the ECO part of a business case (the practical method)

This is the actionable recipe, carried over from Day 3's **ethical-impact analysis** *(Effing, Ethics lecture)*:

1. **Orientation (Step 1):** Who are the stakeholders? Are there clear dilemmas? Is technology the answer? *(Effing lecture's "Step 1 Orientation" slide.)*
2. Examine **ethical/sustainability implications** — recognizing these are **not necessarily a particular risk** and that there are **various, potentially opposing views**.
3. **Temporarily set aside your own opinions** and reason from multiple perspectives.
4. **Look at the UN SDGs and explicitly reflect on potential negative *and* positive external effects** of the IT innovation — i.e., **map the project to the relevant SDGs.**
5. Where possible, **frame sustainability investments as profit-driven CSR / real options** so they earn a place in the financial argument, not just the ethics section (Herath et al.).

The business-case outline's section 9 ties it together: a **reflection on moral consequences using philosophical angles** (Day 3) *plus* an explanation of **how the case maps to the UN sustainability and public-responsibility goals** (Day 4) *(Course manual, suggested outline)*.

**Exam angle:** If asked how to address sustainability/public responsibility in a business case, give the method: identify stakeholders and dilemmas, set aside personal bias, **map the project to specific relevant SDGs reflecting on positive and negative external effects**, and frame green investment as **profit-driven CSR** (triple bottom line; win-win) — ideally valued with real-options thinking to capture strategic flexibility.

---

# PART 3 — TYING IT TOGETHER (THE DAY 4 STORY IN ONE PASS)

Here's the connected narrative to hold for the exam:

A business case doesn't exist in a vacuum — it sits in a **sector** and has **public/environmental consequences**, and both make it harder than a private financial calculation. The **public sector** (government and semi-government bodies serving public value) differs from the private sector across ten attributes **(Winkler, 2013)**: it pursues **multifaceted public value** not shareholder profit, answers to **many conflicting stakeholders**, works under **heavy legal/regulatory constraints**, faces **soft budgets and public scrutiny**, is **highly risk-averse**, **cooperates rather than competes**, treats **IT as a necessity** not a weapon, has **lower IT competencies**, must use **complex tendering/procurement**, and relies on **shared IT resources**. This is why public-sector IT projects are so failure-prone (half of Nelson's infamous failures were public-sector) and why the business case must justify **multifaceted public value** rather than just NPV — seen live in Ryan & Gregory's cases (Helsinki protecting jobs over efficiency; Copenhagen's public-value-vs-profit tension).

The **ECO/sustainability** lens adds the duty to weigh **public and environmental consequences** — the **principle of public responsibility** (business and society interpenetrate; Preston & Post) and **CSR**, optimizing the **triple bottom line of economic, social, and environmental** performance. The concrete tool is the **17 UN SDGs** (set 2015, target 2030; especially **Goal 11, Sustainable Cities**), which you **map** to a project, reflecting on **both positive and negative external effects** — the continuation of Day 3's ethical-impact analysis. And **Herath et al. (2019)** show sustainability can earn its place in the *financial* argument: green computing as a **profit-driven CSR real option** (a win-win, valued as **NPV + the option value of flexibility/waiting** under carbon-tax uncertainty, via Bayesian updating) — which previews the real-options thinking of Day 5 and shares the decision-tree technique with Day 2's risk EMV.

---

# QUICK-FIRE SELF-TEST (cover the answers)

1. **What are the four organisation types in the public/private taxonomy?** → Private: for-profit organisations and non-profit organisations (NPOs). Public: government agencies (public service) and semi-government agencies. *(Sethibe et al. 2007 / Harmelink L07)*
2. **Private vs. public — name 5 attribute contrasts (Winkler).** → Goals: shareholder value vs. multifaceted public value; Stakeholders: few vs. many/conflicting; Environment: less regulated vs. legal/formal constraints; Incentives: high/market vs. low/soft budgets/scrutiny; Risks: lower vs. high aversion (also: competition, IT innovation, IT competencies, complex tendering, shared resources). *(Winkler 2013)*
3. **Why is public-sector IT decision-making more complex (one line)?** → It serves multifaceted public value (not profit) for many conflicting stakeholders under heavy legal/budgetary/scrutiny constraints, with high risk-aversion and complex tendering. *(Winkler 2013)*
4. **Give a concrete public-sector example of "public value over profit."** → Helsinki municipality protects staff jobs regardless of SIS efficiency (chat-bots reallocate, not replace); or Copenhagen kept the City Data Exchange running for citizen value beyond what a private partner would. *(Ryan & Gregory 2019)*
5. **How many UN SDGs, set when, target when?** → 17 SDGs, established 2015, target 2030. *(Ryan & Gregory 2019 / Effing lecture)*
6. **Which SDG is central to smart cities, and why?** → Goal 11, Sustainable Cities and Communities — urban population grows by 1.5bn by 2030, straining resources, so smart cities are proposed as a creative response. *(Ryan & Gregory 2019)*
7. **Define the triple bottom line.** → Economic, social, and environmental performance — what CSR/sustainability optimizes, not just the financial line. *(Herath et al. 2019, citing Aguinis & Glavas)*
8. **What is the principle of public responsibility?** → Business and society interpenetrate (each influences the other), so decision-makers must weigh the public/environmental consequences of their decisions. *(Preston & Post 1975, via Herath et al. 2019)*
9. **What is green computing?** → Efficient, ecologically friendly computing aimed at reducing both IT costs and environmental impact (e.g. virtualization, cloud, server consolidation, e-waste disposal, energy reduction). *(Herath et al. 2019)*
10. **What's the core reframing in Herath et al. (2019)?** → Green/CSR investment is not pure cost or charity but a profit-driven CSR strategy — a win-win that creates value for firm and society — best valued as a real option (NPV + flexibility value), not plain NPV. *(Herath et al. 2019)*
11. **How do you "map SDGs to a project"?** → Select the specific relevant SDGs the project touches and reflect on both positive and negative external effects against each (not all 17). *(Effing lecture / Course manual)*
12. **How does the public sector show up as a quality criterion in the business case?** → The outline says "focus on public sector problems," and assessment asks whether public-sector idiosyncrasies are considered and the case is feasible for a public-sector organisation. *(Course manual)*

---

## Sources used in this summary

- **Harmelink (2026), Lecture 07 — "From Business Case to IT Governance"** — the private/public taxonomy (Sethibe et al. 2007) and the private-vs-public comparison table with ITG implications (Winkler 2013). *(Source for §1.1–§1.2.)*
- **Winkler, T. J. (2013), "IT governance mechanisms and administration/IT alignment in the public sector"** — the ten-attribute public-vs-private comparison table (goals, stakeholders, environment, incentives, risks, competition, IT innovation, IT competencies, IT sourcing, IT resources) and the ITG implications. *(Source for §1.2.)*
- **Sethibe, T., Campbell, J. & McDonald, C. (2007), "IT governance in public and private sector organisations"** — the public/private organisation taxonomy (for-profit/NPO; government/semi-government). *(Source for §1.1.)*
- **Ryan, M. & Gregory, A. (2019), "Ethics of Using Smart City AI and Big Data"** — public-sector dynamics in practice (Helsinki job protection, Copenhagen public-vs-private tension, collaborative bottom-up models); UN SDGs and Goal 11; the 1.5-billion urban-growth figure. *(Source for §1.3 and §2.1.)*
- **Nelson, R. R. (2008), "IT Project Management: Infamous Failures, Classic Mistakes, and Best Practices"** — half of the most infamous IT failures came from the public sector. *(Cross-referenced in §1 intro.)*
- **Effing (2026), Ethics lecture** — the 17 UN SDGs slide; the ethical-/sustainability-impact analysis method (orientation step, set aside own views, map to SDGs, reflect on positive and negative external effects). *(Source for §2.1 and §2.4.)*
- **Herath, H. S. B., Herath, T. C. & Dunn, P. (2019), "Profit-Driven Corporate Social Responsibility as a Bayesian Real Option in Green Computing," *Journal of Business Ethics* 158(2)** — green computing; profit-driven CSR; triple bottom line and the principle of public responsibility (Aguinis & Glavas 2012; Preston & Post 1975); the server-consolidation case; valuing green/CSR investment as a Bayesian real option (NPV + option value under carbon-tax uncertainty). *(Source for §2.2–§2.3.)*
- **Course manual — test matrix, suggested outline, and assessment criteria** — the PUBLIC and ECO learning goals and weights; "focus on public sector problems"; the section-9 requirement to map the case to UN sustainability and public-responsibility goals; the public-sector idiosyncrasy assessment criterion. *(Framing throughout.)*

---

*End of Day 4 summary. Next up (Day 5): Tools — Real Options Theory and the PRINCE2 business case, plus Governance — where the real-options/NPV/Bayesian thinking previewed in §2.3 here gets developed in full (with decision trees, option premiums, and the static-NPV-vs-flexibility contrast), and the IT-governance mechanisms from Winkler's table (§1.2) connect to portfolio management and the strategic grid.*
