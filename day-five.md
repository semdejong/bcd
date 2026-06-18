# Day 5 Study Summary — Business Case Development for IT Projects
## Topic block: Tools (Real Options + PRINCE2) + Governance

*University of Twente — covers the Real Options Theory lecture (Harmelink, Lecture 06), Lee & Shin (2018) on fintech/real options, the PRINCE2 business case (Harmelink, Lecture 01), and the Governance lecture (Harmelink, Lecture 07, drawing on Ward & Daniel 2012, Ward & Peppard 2002, Lycett et al. 2004, and the example exam). This is everything you need for the tools and governance sides of a business case — and it's the most computational day, so it pairs concepts with a worked decision-tree example.*

---

## How to use this summary

Same approach as Days 1–4: read it through once, then self-test by covering the explanations and reproducing the definitions, the strategic grid, the node rules, and the worked computation from memory. **"Exam angle"** flags the points most likely to be tested, sources are attributed inline, and there's a full source list at the end.

**Why this is the make-or-break computational day.** Unlike the other topics, **Real Options can appear as a calculation question** — the example exam's Question 5 literally says *"Draw a decision tree and compute the expected value. Should PublicCo develop the SmartMesh?"* So you must be able to *do* the maths, not just describe the theory. The Governance side (IT portfolio, the Strategic Grid, programmes vs projects) is also directly examined — example-exam Question 1 asks you to define "IT portfolio" and apply the Strategic Grid. Together, **Tools is 5% and Governance is 5%** of the individual exam, but the calculation question makes this day high-stakes per point.

**The connections to earlier days.** Real options is the natural extension of the **NPV/financial-appraisal** thinking introduced with Costs (Day 2) and previewed in the **green-computing CSR real option** (Day 4) — and it shares the exact **decision-tree** technique used for **risk EMV** (Day 2). Governance closes the loop opened on Day 1 (the business case as "part of the IT governance toolbox") and builds on the **drivers → objectives → benefits** chain (Day 1) and the **public-sector** governance mechanisms from Winkler (Day 4).

---

# PART 1 — REAL OPTIONS THEORY

## 1.1 The problem real options solves

Start with *why* the tool exists *(Harmelink, Lecture 06, citing Mun 2002)*:

- IT projects are **complex** and need financial/statistical information to decide on.
- That information is **not precise upfront and may change** — the future is uncertain.
- **Traditional methods** (e.g. **NPV — Net Present Value**, **IRR — Internal Rate of Return**) treat value as a **single, time-value-discounted result** — a **static view** of uncertainty. They compute one number now and assume the plan is fixed.
- The problem: this static view **ignores flexibility**. In reality managers can wait, expand, abandon, or switch as information arrives — and that flexibility has value. NPV alone **undervalues** uncertain, risky projects.

The fix — the **expanded view**:

> **Real options value = Static NPV + Option Premium**, where the **option premium = the value of being flexible in your decisions** *(Harmelink, Lecture 06)*.

In Lee & Shin's words, NPV *"ignores flexibility in investment such as deferment and expansion,"* tends to undervalue projects with a high discount rate, and is **not suitable for highly uncertain, risky technology projects** — so a real-options approach is more appropriate for experimental projects in fluid economic/regulatory environments *(Lee & Shin, 2018)*.

**Exam angle:** The cleanest, most likely conceptual question is the **NPV vs. real options** contrast. Your answer: traditional NPV/IRR gives a **static, single-number** view that ignores managerial flexibility and undervalues uncertain projects; real options add the **option premium** (the value of flexibility), giving **NPV + option value** — a **dynamic** view that treats uncertainty as a potential opportunity. Cite Mun (2002) for the static-view critique.

## 1.2 The definition of real options theory

The definition to know *(Harmelink, Lecture 06, citing Amram, Kulatilaka & Henderson, 1999)*:

> *"Viewed **narrowly**, the Real-Options approach is the **extension of financial option-pricing models to the valuation of options on real (that is, non-financial) assets**. More **broadly**, the Real-Options approach is **a way of thinking that helps managers formulate their strategic options** — the future opportunities that are created by today's investments."*

Two halves to remember: **narrow** = applying financial-option pricing to *real* (physical/business) assets; **broad** = a strategic *mindset* about future opportunities created by today's investments. And the lecture's framing of what real options does *(Amram et al. 1999)*: it **incorporates flexibility** by linking IT investment to business risks, turning the financial decision into a **roadmap for managing IT**, **creating value by treating uncertainty as a potential opportunity**, and **changing the static view into a dynamic view.**

Crucially, the lecture stresses: **Real Options Theory is about long-term strategic decisions, not short-term operational ones** *(Harmelink, Lecture 06)*.

**Exam angle:** Be ready to give the narrow-and-broad definition and attribute it to Amram et al. (1999), and to state that it's for **long-term strategic** decisions. The "uncertainty as opportunity / static → dynamic" phrasing is worth memorizing.

## 1.3 Financial options (the foundation)

Because real options extend *financial* options, know the basics *(Harmelink, Lecture 06)*:

- **Call option** = the right (not obligation) to **buy** an asset at a certain price.
- **Put option** = the right (not obligation) to **sell** an asset at a certain price.
- **Long** = you **buy** the option; **Short** = you **sell** the option.
- You **pay for the right, not for the asset itself** — and the appeal is **hedging (financial) risk.**

The key parallel: like financial options, **real options are the right, but not the obligation, to take an action** (wait, expand, abandon) during a period or by an expiration date *(Lee & Shin, 2018)*. One important difference for *internal* IT projects (R&D, technology development): the **option buyer and seller are the same entity**, so any returns belong to the investor *(Lee & Shin, 2018)*.

## 1.4 The types of real options

Mun (2012) lists the strategic options a business case might contain *(Harmelink, Lecture 06, citing Mun 2012)*. Know a representative set:

- Option for **future growth**
- Option to **wait and see** / **delay** (defer)
- Option to **expand**
- Option to **contract**
- Option to **choose**
- Option to **switch resources**
- Option for **phased and sequential investments**

Lee & Shin (2018) emphasize four for tech projects: **defer** (wait/learn whether it'll be profitable), **expand** (invest more in a profitable project), **abandon** (exit a loss-making project, sell/redeploy assets), and **contract** (scale back).

**Exam angle:** Be able to name several option types and explain at least **defer/wait, expand, abandon** with a one-line meaning each, since these are the most common and appear in both the lecture and Lee & Shin.

## 1.5 Decision trees — the tool you must be able to USE

This is the computational heart of the day. The lecture's intended learning outcomes are explicit: **recognise the added value of real options, construct a simple model (decision tree), and analyse it with backward induction** *(Harmelink, Lecture 06)*.

### The two node types

A decision tree has two kinds of nodes — and the rule for valuing each is different *(Harmelink, Lecture 06)*:

- **Probability / uncertainty node** — outcomes happen by **random events with known probabilities** (the decision-maker does *not* control which branch occurs). **Value = the expected value of all possibilities** (probability-weighted average of the branches). *Probabilities on the branches must sum to 1.*
- **Decision node** — the **decision-maker chooses** among alternatives. **Value = the maximum value of the options available** (you'll pick the best one). This is where the *option* lives — the freedom to choose the best branch is exactly what creates the option's value.

*(Memory hook: chance node → average/expected value; choice node → take the max. The decision node uses "max" because a rational manager exercises the option only when it's worth it — e.g. you abandon only if abandoning beats continuing.)*

### Backward induction (the method)

To compute the value *(Harmelink, Lecture 06)*:

1. **Start at the end** of the time horizon (e.g. year 2).
2. **Compute the value of each preceding node** — expected value at probability nodes, maximum at decision nodes.
3. **Check** that probabilities at each chance node sum to 1.
4. **Continue working backwards** until you reach the starting node.
5. The result is the **expected value over the whole time horizon** of the project.

### The lecture's worked example (learn the logic)

A new operating system is in development costing **$705m** (developing = –750 in the simplified tree). Development can be **successful (80%)** or **less successful (20%)**. Launch costs depend on success (**–2000** if successful, **–3000** if less successful). The market can be **large or small (50% each)**, with product NPV **3500 or 2500** *(Harmelink, Lecture 06)*. Working backward through the expected-value (chance) and max (decision) nodes:

- **Without** the extra flexibility, the project value comes out to **50**.
- **With** an added decision point — the **option to abandon** ("stop = 0" branches, so you never accept a negative payoff) — the value becomes **100**.
- Therefore **the value of adding the option to abandon is 100 − 50 = 50.** You check the traditional value by *deleting* the second decision moment.

This captures the whole point: **the option (the freedom to abandon a bad outcome) is worth 50** — that's the **option premium**, the value that static NPV would have missed.

### How to answer a "draw a decision tree and compute expected value" question

For the example-exam Q5 type (e.g. PublicCo's SmartMesh) *(Example exam)*, the method is:

1. Draw the **decision node** (develop vs. not develop).
2. On the "develop" branch, draw the **probability node** with the outcome branches and their probabilities (each return × its probability).
3. Compute the **expected value** of the develop branch = Σ(probability × return), then subtract the development cost.
4. Compare against the "not develop" value.
5. **Recommend** the higher-value branch.

*Worked illustration using the example-exam numbers:* Not developing → expected revenue **500k**. Developing costs **750k**; with **65%** you get **1650k** and with **35%** you get **850k**. Expected return if developing = (0.65 × 1650) + (0.35 × 850) = 1072.5 + 297.5 = **1370k**. Net of the 750k cost → **620k**. Since **620k > 500k**, **PublicCo should develop the SmartMesh.** (Always show the probability-weighting, subtract the cost, and state the recommendation explicitly.)

**Exam angle — this is the highest-value practical skill of the day.** Practice until you can: (1) draw a clean tree with decision vs. probability nodes, (2) apply **expected value at chance nodes and max at decision nodes**, (3) use **backward induction**, (4) **subtract costs** on the relevant branch, and (5) **give a clear recommendation**. Always check probabilities sum to 1. The option's value = (value with the option) − (value without it).

## 1.6 Applying real options to your business case

The four questions to ask *(Harmelink, Lecture 06)*:

1. Which **strategic opportunities/risks** exist, realistically?
2. Which **options** would you have at certain moments in time?
3. How would you **value** these options?
4. Which **information** would you need to get an accurate value?

And the standing reminder: real options is for **long-term strategic** decisions, not short-term operational ones. (Recall Day 4's Herath et al. green-computing case: the green investment was valued as a **real option** capturing the value of *waiting for information* on the carbon tax — a concrete application of exactly this.)

---

# PART 2 — THE PRINCE2 BUSINESS CASE

PRINCE2 (PRojects IN Controlled Environments) is the second "tool" named in the learning goal *(Course manual: "know the added value of business case tools such as real options and PRINCE II business case")* *(Harmelink, Lecture 01, citing Prince2primer.com)*.

The core idea the lecture conveys: the **PRINCE2 business case weighs Benefits against Cost and Risk** — it's literally depicted as a scale balancing **Benefits** on one side against **Cost** and **Risk** on the other *(Harmelink, Lecture 01)*. This embodies the central logic of the whole course: a justified investment is one where the expected **benefits outweigh the costs and risks.**

The PRINCE2 business case is a **living document** used to justify the project and confirm **continued business justification** throughout its life — if the justification disappears, the project should stop. A standard PRINCE2 business case contains: **expected benefits** (and **dis-benefits** — negative outcomes a stakeholder considers undesirable), **costs**, **timescale**, **risks**, and an **investment appraisal** weighing it all up. The defining principle is **continued business justification** — the case is checked at each stage, not written once and filed.

**Exam angle:** For "what is the added value of the PRINCE2 business case?" → it provides a **structured way to justify an IT investment by balancing benefits against costs and risks**, and enforces **continued business justification** across the project's life (stop if justification is lost). The benefits-vs-cost-and-risk balance is the memorable image. Know that it sits alongside real options as the two named business-case *tools*.

---

# PART 3 — IT GOVERNANCE

This is where the course comes full circle: the business case was introduced on Day 1 as **"part of the IT governance toolbox."** Governance is about making sure the *right* IT investments are chosen and steered well.

## 3.1 What is governance, and IT governance?

Definitions *(Harmelink, Lecture 07, citing Cambridge Dictionary 2022 and Ward & Daniel 2012)*:

- **Governance** (Cambridge Dictionary) = *"the way that organizations or countries are managed at the highest level, and the systems for doing this."*
- **IT governance** extends this to IT decisions. The Ward & Daniel (2012) rationale captures *why* it matters: *"Effective governance is required to ensure that the organization does not waste its funds and resources on investments that do not adequately contribute to the business."*
- A nice supporting idea (Weill & Aral, 2006): *successful IT portfolio management techniques change the conversation from technical to strategic considerations* — i.e. governance lifts IT decisions out of "which technology?" up to "which investments serve the strategy?"

**Exam angle:** Define IT governance as the high-level management and systems for ensuring IT investments **contribute to the business** and don't waste resources. Link it explicitly to the business case as the instrument that justifies and monitors those investments.

## 3.2 Projects vs. programmes vs. portfolios — the three levels

This is a core governance distinction and an exam favourite (example-exam Q1 and Q2 hinge on it). The course defines a hierarchy *(Harmelink, Lecture 07)*:

- **IT project** = a **single investment** to be implemented, achieving a result of specified quality within defined **time, resource, and cost** constraints. **Finite** (months to ~1 year+). Managed by a project manager. Success = **narrowly defined** (time, cost, quality).
- **IT programme** = a **set of interrelated IT projects** (plus organizational-development measures) that collectively implement a **big strategic initiative** with a common, superordinate goal (Pellegrinelli 2002). **Finite but often several years.** Supervised by a programme manager who heads the **PMO** and reports to top management. Success = **broadly defined** (e.g. **benefits delivered to stakeholders**).
- **IT portfolio** = the **entirety of an organization's IT investments** (all projects *and* programmes). The job is to **select and prioritise investments for the best benefit of the organization.** **Enduring** (ongoing, reviewed regularly). Managed by a **(chief) investment controller, e.g. the CFO.** Success = **aggregated performance** of all investments.

The progression: **project → programme → portfolio** moves from a single deliverable, to a strategic initiative of related projects, to the whole investment landscape. *(Ward & Daniel devote a chapter to exactly this: "From projects to programmes to portfolios.")*

**Why programmes exist:** strategic decisions **can't be translated directly** into a single piece of software or one task; large strategic change needs a set of **interdependent projects and measures** — and programme management makes that change happen *(Harmelink, Lecture 07)*.

**Exam angle:** Be able to define all three levels and contrast them on **objective, scope, duration, manager, and success measure** (the comparison-table dimensions). The key contrasts: project = single deliverable/narrow success/short; programme = strategic initiative of related projects/benefits-based success/multi-year; portfolio = all investments/prioritisation/aggregated performance/enduring.

## 3.3 IT programme management — goals and execution issues

**Programme management defined** *(Harmelink, Lecture 07)*: a **high-level, long-term occupation** of planning and supervising a programme to **assure the realization of business benefits**, taking account of the **superordinate goal/mission, the functional/technical/resource dependencies among projects, the overall schedule, and the overall costs, benefits, and risks.**

**Programme management goals (Lycett et al. 2004)** split into two types *(Harmelink, Lecture 07)*:

- **Efficiency and effectiveness goals:** improved coordination; improved **dependency management**; more effective resource utilisation; more effective knowledge transfer; greater senior-management visibility.
- **Business focus goals:** more coherent communication; improved project definition; **better alignment with business drivers, goals, and strategy.**

**Key issues in programme *execution*** (example-exam Q2 asks for "two key issues of IT program delivery") *(Harmelink, Lecture 07)*: **keeping motivation alive**; **staying on track**; **shifting, reallocating and prioritizing resources**; and **communicating between projects, setting expectations.** Each can be resolved through stronger programme governance — e.g. a PMO for coordination, clear dependency management, and regular reprioritisation.

**Exam angle:** If asked for "key issues of IT programme delivery and how to resolve them," draw from this list (motivation, staying on track, resource reallocation/prioritisation, inter-project communication) and resolve each via programme-management mechanisms (PMO, dependency management, senior-management visibility, clear communication/expectation-setting). The **Lycett et al. (2004)** efficiency-vs-business-focus split is a citable framework.

## 3.4 The IT portfolio and the Strategic Grid — HIGH PRIORITY

The **IT portfolio** is the entirety of an organization's IT investments, managed to **select and prioritise** for best organizational benefit *(Harmelink, Lecture 07)*. The tool for assessing/balancing it is the **Strategic Grid** *(Ward & Peppard 2002, originally McFarlan 1983)* — a 2×2 classifying applications/investments by their contribution to the business. The four quadrants:

| | (contribution to future) | |
|---|---|---|
| **STRATEGIC** — applications **critical to sustaining future business strategy** | | **HIGH POTENTIAL** — applications that **may be important in achieving future success** |
| **KEY OPERATIONAL** — applications on which the organization **currently depends for success** | | **SUPPORT** — applications that are **valuable but not critical** to success |

How to read it:

- **Strategic** — critical to **future** strategy (high current and future importance). *Invest to win.*
- **High potential** — **may** be important to future success (uncertain, innovation-based). *These are the natural home of **real options thinking** — experiment, wait-and-see, and expand if they prove out.*
- **Key operational** — the organization **currently depends** on these (run-the-business systems). *Maintain and protect.*
- **Support** — **valuable but not critical**. *Minimize cost.*

This connects straight to Day 1's portfolio categories (strategic / high potential / key operational / support) and to **drivers** — investments should map back to business drivers and strategy.

**Exam angle (likely calculation-adjacent conceptual question, per example-exam Q1):** Be able to (1) **define "IT portfolio"** (the entirety of an org's IT investments, selected and prioritised for best benefit), (2) **explain the Strategic Grid** and its four quadrants with what each means, and (3) state the **decision options** for investments — typically: **invest/prioritise** (strategic, key operational), **experiment/option** (high potential — pilot, wait, expand or drop), and **minimise/maintain or divest** (support). Attribute the grid to **Ward & Peppard (2002), originally McFarlan (1983).**

## 3.5 Governance and portfolio management together

The synthesis *(Ward & Daniel 2012; Harmelink, Lecture 07)*: governance ensures resources aren't wasted on investments that don't contribute to the business; **portfolio management** is how governance operationalises that — selecting, prioritising, and monitoring the whole set of projects and programmes, linking each back to **drivers and strategy**, and setting priorities across them. This is the GOVERNANCE learning goal almost verbatim: *"develop and monitor a portfolio plan of projects and show the relationships and surplus meaning of its underlying entities for governance purposes"* *(Course manual)*. The "underlying entities" are the projects and programmes; the "surplus meaning" is the strategic value that emerges from managing them as a coordinated portfolio rather than in isolation.

---

# PART 4 — TYING IT TOGETHER (THE DAY 5 STORY IN ONE PASS)

Here's the connected narrative to hold for the exam:

The course's **tools** sharpen how you justify an investment under uncertainty. Traditional appraisal (**NPV/IRR**) gives a **static** single number that **ignores managerial flexibility** and undervalues risky IT projects **(Mun 2002)**. **Real Options Theory** fixes this: **value = static NPV + option premium**, the premium being the **value of flexibility** — narrowly, extending financial-option pricing to real assets; broadly, a strategic way of thinking about future opportunities created by today's investments **(Amram et al. 1999)**. Like financial **call/put** options, real options are a **right, not an obligation** to **defer, expand, abandon, or contract** **(Mun 2012; Lee & Shin 2018)**. You model and value them with **decision trees**: **expected value at probability (chance) nodes, maximum value at decision (choice) nodes**, solved by **backward induction** from the end of the horizon — and the **option's value = value-with-the-option − value-without-it** (the lecture's abandon example: 100 − 50 = 50). For an exam calculation, draw the tree, probability-weight the chance branches, subtract costs, and **recommend the higher-value branch** (e.g. PublicCo's SmartMesh: develop, 620k > 500k). The second tool, the **PRINCE2 business case**, balances **Benefits against Cost and Risk** and enforces **continued business justification** across the project's life.

These tools serve **IT governance** — the high-level systems ensuring IT investments **contribute to the business and don't waste resources** **(Ward & Daniel 2012)**. Governance works across three levels — **project** (single deliverable, narrow time/cost/quality success), **programme** (interrelated projects implementing a strategic initiative, benefits-based success, multi-year, run via a PMO **— Lycett et al. 2004** for its efficiency-vs-business-focus goals), and **portfolio** (the entirety of investments, selected and prioritised for best organizational benefit). The portfolio is balanced with the **Strategic Grid (Ward & Peppard 2002 / McFarlan 1983)** — **strategic, high potential, key operational, support** — where **high-potential** investments are exactly where **real options thinking** belongs. Governance + portfolio management is how the organization links every investment back to its **drivers and strategy** (closing the loop from Day 1) and steers the whole set for strategic value.

---

# QUICK-FIRE SELF-TEST (cover the answers)

1. **What's wrong with traditional NPV/IRR for IT projects?** → Static, single-number view that ignores managerial flexibility and undervalues uncertain/risky projects. *(Mun 2002 / Harmelink L06)*
2. **Real options value formula?** → Value = static NPV + option premium, where option premium = the value of being flexible. *(Harmelink L06)*
3. **Define real options theory (narrow + broad).** → Narrow: extending financial option-pricing models to real (non-financial) assets. Broad: a way of thinking that helps managers formulate strategic options — future opportunities created by today's investments. For long-term strategic, not operational, decisions. *(Amram et al. 1999)*
4. **Call vs. put option; long vs. short?** → Call = right to buy; put = right to sell. Long = buy the option; short = sell it. You pay for the right, not the asset. *(Harmelink L06)*
5. **Name four real-option types.** → Defer/wait, expand, abandon, contract (also: growth, choose, switch, phased/sequential). *(Mun 2012 / Lee & Shin 2018)*
6. **Two decision-tree node types and how to value each?** → Probability/chance node → expected (probability-weighted) value of all branches (probabilities sum to 1). Decision node → maximum value of the available options. *(Harmelink L06)*
7. **What is backward induction?** → Start at the end of the time horizon and compute each preceding node's value (expected value at chance nodes, max at decision nodes), working back to the start to get the project's total expected value. *(Harmelink L06)*
8. **How do you find the value of an option (e.g. to abandon)?** → Value-with-the-option minus value-without-it (delete the decision moment to get the no-option value); e.g. 100 − 50 = 50. *(Harmelink L06)*
9. **Worked: develop SmartMesh? (cost 750k; 65%→1650k, 35%→850k; not-develop 500k).** → E[develop] = 0.65×1650 + 0.35×850 = 1370k; minus 750k = 620k > 500k → develop. *(Example exam)*
10. **What does the PRINCE2 business case balance, and its key principle?** → Balances Benefits against Cost and Risk; key principle = continued business justification across the project's life (stop if justification is lost). *(Harmelink L01)*
11. **Define IT governance.** → The high-level management and systems ensuring IT investments contribute to the business and don't waste funds/resources. *(Ward & Daniel 2012)*
12. **Project vs. programme vs. portfolio?** → Project = single deliverable, narrow time/cost/quality success, finite. Programme = interrelated projects implementing a strategic initiative, benefits-based success, multi-year, run via PMO. Portfolio = entirety of IT investments, selected/prioritised for best benefit, enduring, run by a CFO-type controller. *(Harmelink L07)*
13. **Name two key issues in IT programme delivery (+ how to resolve).** → e.g. keeping motivation alive; staying on track; reallocating/prioritising resources; inter-project communication — resolved via PMO coordination, dependency management, senior-management visibility, clear expectation-setting. *(Harmelink L07 / Lycett et al. 2004)*
14. **Define "IT portfolio" and the Strategic Grid's four quadrants.** → Portfolio = entirety of an org's IT investments, selected/prioritised for best benefit. Grid (Ward & Peppard 2002 / McFarlan 1983): Strategic (critical to future strategy), High Potential (may be important to future success), Key Operational (currently depended on), Support (valuable but not critical). *(Harmelink L07)*
15. **Which grid quadrant fits real-options thinking, and why?** → High Potential — uncertain, innovation-based investments where wait-and-see/expand/abandon flexibility is most valuable. *(synthesis: Harmelink L06 + L07)*

---

## Sources used in this summary

- **Harmelink (2026), Lecture 06 — "Real Options Theory: BCD for IT"** — the static-NPV problem and "NPV + option premium"; the Amram et al. (1999) definition; financial options (call/put, long/short, hedging); Mun (2012) option types; decision-tree node rules and backward induction; the worked OS/abandon example; the four business-case questions; the "long-term strategic, not operational" caveat. *(Source for Part 1.)*
- **Amram, M., Kulatilaka, N. & Henderson, J. C. (1999), "Managing business risk by IT investment: The real options view," *CIO Magazine*** — the narrow-and-broad definition of real options and the flexibility/dynamic-view framing. *(Source for §1.2.)*
- **Mun, J. (2002 / 2012), *Real Options Analysis*** — the critique of single-time-value methods (2002) and the list of real-option types (2012). *(Source for §1.1 and §1.4.)*
- **Lee, I. & Shin, Y. J. (2018), "Fintech: Ecosystem, business models, investment decisions, and challenges," *Business Horizons*** — NPV's neglect of flexibility; real options as rights-not-obligations (defer/expand/abandon/contract); decision trees recommended over closed-form pricing for one-of-a-kind tech projects; buyer-equals-seller for internal projects. *(Source for §1.1, §1.3–§1.5.)*
- **Harmelink (2026), Lecture 01 — "Introduction to IT Business Cases"** (citing Prince2primer.com) — the PRINCE2 business case balancing Benefits against Cost and Risk. *(Source for Part 2.)*
- **Harmelink (2026), Lecture 07 — "From Business Case to IT Governance"** — governance and IT-governance definitions (Cambridge Dictionary 2022; Ward & Daniel 2012; Weill & Aral 2006); project/programme/portfolio definitions and comparison; programme-management definition; Lycett et al. (2004) programme goals; key programme-execution issues; the IT portfolio and the Strategic Grid. *(Source for Part 3.)*
- **Ward, J. & Peppard, J. (2002), originally McFarlan (1983)** — the Strategic Grid (strategic / high potential / key operational / support). *(Source for §3.4.)*
- **Ward, J. & Daniel, E. (2012), *Benefits Management*** — the IT-governance rationale ("does not waste funds … on investments that do not adequately contribute"); the projects→programmes→portfolios progression; governance and portfolio management. *(Source for Part 3.)*
- **Lycett, M. et al. (2004)** — the efficiency/effectiveness vs. business-focus split of programme-management goals. *(Source for §3.3.)*
- **Example Questions (BCDIT) — the "PublicCo / SmartCity 5.0" exam** — the IT-portfolio + Strategic Grid question, the programme-delivery-issues question, and the decision-tree/expected-value calculation (SmartMesh). *(Source for §1.5, §3.2–§3.4.)*

---

*End of Day 5 summary. This completes the topic-by-topic coverage. For Day 6, run the full set of example questions under timed, closed-book conditions and grade against the norm answers — and make sure you can DRAW and COMPUTE a decision tree from scratch (the one skill on this exam that requires doing, not just describing).*
