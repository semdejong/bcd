# Day 1 Study Summary — Business Case Development for IT Projects
## Topic block: Introduction to IT Business Cases + Benefits Management

*University of Twente — covers Lecture 01 (Introduction), the Benefit Management lecture (Effing), Ward & Daniel (2012), Nelson (2008), and the Benefits/Costs workshop. Everything you need to fully understand the foundations and the benefits side of a business case.*

---

## How to use this summary

This is your single source for Day 1. Read it top to bottom once, then come back and test yourself by covering the explanations and trying to reproduce each definition and example from memory. The exam is **closed-book**, so you need recall, not recognition. Wherever you see **"Exam angle"**, that flags a point the exam is especially likely to test (often as a "what is the difference between X and Y" question, which is this exam's favourite format).

A quick map of where this fits: Benefits is worth ~5% of the individual exam on its own, but the *foundations* covered here (what a business case is, why IT projects fail, business–IT alignment) underpin almost every other topic. So this is high-leverage even beyond its direct point weight.

---

# PART 1 — FOUNDATIONS: WHAT IS A BUSINESS CASE AND WHY DOES IT MATTER?

## 1.1 What this course is fundamentally about

The course's central question is: **How do you develop and use business cases to initiate, monitor, and evaluate IT projects?** Notice the three verbs — a business case is not a one-off document you write at the start and forget. It is used:

- **to initiate** — to decide whether a project should start at all and to get it funded/approved;
- **to monitor** — to track during execution whether the project is still on course to deliver what was promised;
- **to evaluate** — to check afterwards whether the promised value was actually realized.

A business case is described as **part of the "IT Governance toolbox."** IT governance is the set of structures and processes an organization uses to make sure its IT investments serve the business strategy and that decisions are made by the right people with the right information. The business case is one of the key instruments inside that toolbox — it is the document that justifies an investment decision.

**Why IT specifically is hard** (the course stresses these as the reasons IT business cases deserve their own course):

- **Complexity of ICT projects and their planning** — IT projects touch many systems, departments, and stakeholders at once, making outcomes hard to predict.
- **The innovative character of IT projects** — you are often doing something new, so you cannot simply copy past estimates; uncertainty is built in.
- **The rise of agile project management** — modern projects increasingly deliver in iterations rather than one big plan, which changes how you justify and monitor value.
- **Advanced complications** like business cases for the **public sector** (multiple, non-financial, politically constrained objectives) and the use of **real options theory** (valuing flexibility under uncertainty) — both are later topics, but they are flagged here as the "advanced" edge of the discipline.

## 1.2 What a business case actually is

A **business case** is a structured, evidence-based argument that a proposed investment (here, an IT project) is worth making. It lays out the problem, the proposed solution, and the expected benefits, costs, and risks, so that a decision-maker can judge whether to commit resources.

The course gives you a concrete picture of what a full business case document contains. The **suggested outline** (based on Schwalbe 2018, Pearlson et al. 2016, and Ward & Daniel 2012) is worth knowing because it shows the logical skeleton of the whole argument:

1. **Executive summary** — one page summarizing the key points for a busy decision-maker.
2. **Introduction and overview** — business background, the current situation, a clear statement of the problem or opportunity, and the recommended solution at a high level.
3. **Problem / opportunity statement and current situation** — the rationale driving the proposal (operational, HR, environmental, competitive, market, or financial), and a specific description of the **As-Is situation** that drives the proposal.
4. **Business objective** — a concise, evidenced statement of what the project should achieve.
5. **Analysis of options and recommendation** — the alternatives considered, their assumptions and constraints, and a reasoned recommendation.
6. **Benefits and business impacts** — financial and non-financial impacts (new business, transformation, innovation, competitive response, organizational, supply-chain, HR).
7. **Costs estimate and financial analysis** — projected costs/revenues/benefits, financial metrics, a financial model, a cash-flow statement, underlying assumptions, and **total cost of ownership (TCO)**.
8. **Risks and contingency analysis** — risks, how to manage them, sensitivity analysis of scenarios, and interdependencies.
9. **Ethical analysis and corporate social responsibility** — moral consequences via various philosophical angles, and mapping to UN sustainability and public-responsibility goals.
10. **Governance of project and requirements** — scope, objectives, key activities, stakeholders, resource plan, metrics, implementation plan, success factors, schedule with milestones, and a **GANTT chart**.
11. **Conclusion and recommendation.**
12. **Appendices** — backup material (detailed financials, marketing materials, etc.).

**Exam angle:** You don't need to memorize all twelve in order, but you should be able to explain that a business case is a *reasoned, evidenced argument* structured around problem → objective → options → benefits/costs/risks → ethics → governance → recommendation. The recurring logic is **why (problem/drivers) → what (objective and benefits) → how (the project and changes that deliver them)**. Keep that triad in your head; it reappears in benefits management below.

## 1.3 The four criteria for a good business case

The course states the **key criterion for assessment is the rigor of the business case.** A good business case is:

- **Plausible** — the story holds together and is believable.
- **Well-reasoned** — conclusions follow validly from premises.
- **Well-evidenced** — claims are grounded in data or literature where possible.
- **Well-analyzed** — established tools and methods are applied correctly.

Three further questions are used to judge it: Is it **convincing**? Are the **idiosyncrasies of the public sector** considered (where relevant)? Are **financial and quantifiable values estimated where possible**?

**Exam angle:** "Plausible, well-reasoned, well-evidenced, well-analyzed" is a clean, memorable four-point answer to "what makes a business case rigorous/good?" Learn it as a set.

## 1.4 Guiding questions for building a business case

These are the questions the business case must answer, and they reveal the internal logic the examiner wants you to reproduce:

- **Is the business problem relevant and persisting?** What is the problem, why does it matter to *this* organization, what is the **As-Is situation** that drives it, and what specific **business objective** arises from it?
- **Is the proposed solution appropriate to achieve the objective (internal consistency)?** How and why will the benefits be derived, is it feasible, are **As-Is and To-Be** properly considered, and are benefits/costs/risks estimated transparently and robustly?
- **Are the state of the art and scientific literature consulted?** Is the relevant body of knowledge identified and applied correctly?

**Key terms to lock in:**

- **As-Is situation** — how things currently work *before* the project. The starting baseline.
- **To-Be situation** — how things will work *after* the project delivers its changes. The target state.
- The gap between As-Is and To-Be is, in effect, what the project delivers. You measure benefits by comparing the two. *Example:* if invoice-processing currently takes 5 days (As-Is) and the new system should bring it to 1 day (To-Be), the benefit is the 4-day reduction and everything that flows from it (lower admin cost, fewer errors, faster cash collection).

## 1.5 Why IT projects fail — Nelson (2008)

This paper is foundational and very exam-friendly because it gives you concrete, citable findings.

**The headline statistic:** Nelson (citing the Standish Group) reports that **roughly two out of three IT projects are considered failures** — meaning total failure, cost overruns, time overruns, or a rollout with **fewer features/functions than promised**. Note the four failure modes; "failure" is broader than total collapse.

**The study itself:** Nelson aggregated **99 retrospectives** (project post-mortems / post-implementation reviews) across **74 organizations** over seven years, looking for recurring "**classic mistakes**." A retrospective is a structured review conducted after a project to capture what went right, what went wrong, and lessons for the future.

**The single most important finding for the exam:** The vast majority of classic mistakes were **process mistakes (45%)** or **people mistakes (43%)**. Only a small minority were product (8%) or technology (4%) mistakes. **None of the top 10 mistakes was a technology mistake.**

> The takeaway: technology is *seldom* the chief cause of IT project failure. Project managers need to be experts in managing **processes and people first**, not just technically skilled.

**The top mistakes** (you don't need all 36, but know the leaders and that they are people/process, not tech):

1. Poor estimation and/or scheduling (process) — 54% of projects
2. Ineffective stakeholder management (people) — 51%
3. Insufficient risk management (process) — 47%
4. Insufficient planning (process) — 39%
5. Shortchanged quality assurance (process) — 37%

The **top three** (estimation/scheduling, stakeholder management, risk management) occurred in roughly **half** of all projects studied. Nelson's practical conclusion: if managers focus their attention on these three areas, they could significantly improve success rates. These map directly onto core business-case topics — estimation feeds benefits and costs, and risk management is its own topic.

A couple of nuances worth a sentence in an exam answer: **scope creep** (uncontrolled expansion of project requirements) did *not* make the top ten, which surprised the author given how often it's blamed — though about 1 in 4 projects still experienced it. And of the 10 most infamous (>$100m loss) failures, **half came from the public sector**, underscoring why public-sector IT decision-making is treated as its own hard problem.

**Exam angle:** A very likely question is some version of "Why do IT projects fail according to Nelson?" Your answer: ~2 in 3 fail; failures are overwhelmingly **people and process** problems rather than technology; the top three recurring mistakes are poor estimation/scheduling, ineffective stakeholder management, and insufficient risk management. The best practices are the mirror image — good estimation, stakeholder/communication planning, and active risk management.

---

# PART 2 — BENEFITS MANAGEMENT (WARD & DANIEL)

## 2.1 The core idea and definition

This is the heart of Day 1 and the part most likely to appear as a direct exam question.

**Definition (Ward & Daniel):** Benefits management is *"the process of organizing and managing such that the potential benefits arising from the use of IS/IT are actually realized."*

Read that definition carefully. The crucial word is **realized**. The whole philosophy rests on a simple but powerful observation: **buying and installing technology does not, by itself, produce benefits.** Benefits only appear when people actually change how they work and the technology is used effectively. So benefits must be actively *managed* into existence, not assumed to follow automatically from the IT.

**IS vs. IT** (a distinction worth being precise about): **IT (Information Technology)** is the hardware, software, and infrastructure — the technical artifacts. An **IS (Information System)** is the broader combination of technology *plus* the people, processes, and information that use it to achieve a purpose. Benefits flow from the *system in use*, not the technology sitting on its own.

## 2.2 The "from → to" shift: traditional IT projects vs. benefits management

Ward & Daniel contrast the old way of running IT projects with the benefits-management way. This comparison is highly memorable and exam-ready. The shift is **from** a technology focus **to** a benefits focus:

| From (traditional) | To (benefits management) |
|---|---|
| Technology **delivery** | Benefits **delivery** |
| Value for **MONEY** (cost focus) | **VALUE** for money (value focus) |
| Expenditure proposal | Business case |
| IT implementation plan | Change management plan |
| Business manager as onlooker / victim | Business manager involved and in control |
| Large set of unfocused functionality | IT investment sufficient to do the job |
| Stakeholders "subjected to" | Stakeholders "involved in" |
| Trained in technology | Educated in exploitation of technology |
| Technology and project audits | Benefits review |

**How to read this table:** Every row moves accountability and attention away from "did we deliver the technology?" toward "did we deliver the value, and did the business change to capture it?" *Example:* the shift from "IT implementation plan" to "change management plan" captures the whole idea — installing the software is the easy part; getting people to work differently so the software pays off is the real project.

**Exam angle:** If asked "what is different about the benefits-management approach compared to traditional IT project management?", structure your answer around this from→to shift: focus on benefits not technology, on value not just cost, business managers in control, stakeholders involved, and a change-management/benefits-review orientation rather than a technology-delivery/audit orientation.

## 2.3 Business–IT alignment

A foundational principle: **a business case should be linked to the organizational strategy.** This is **business–IT alignment** — the degree to which IT investments and the business strategy point in the same direction.

Modern approaches to strategic IS/IT planning (Ward & Peppard, 2002) aim to:

- identify **IS/IT-enabled business opportunities**;
- **align** IS/IT projects with business strategies and priorities;
- source and implement IT architectures, infrastructure, applications, and services;
- develop the organizational resources, competences, and capabilities to deploy and use the technology effectively.

The practical point: a benefit that doesn't trace back to a business driver and ultimately to strategy is hard to justify. Alignment is what keeps the business case anchored to something the organization actually cares about.

## 2.4 The benefits management process — the five steps

Ward & Daniel describe benefits management as a **five-step process**. It is **iterative** — not a strict one-way pipeline — because objectives get modified and new benefits get identified as ideas and options are explored. Know the five steps and what each does:

**Step 1 — Identifying and structuring the benefits.**
You analyze the **drivers** to determine the **investment objectives**, then identify the benefits each stakeholder will get from achieving those objectives and how each benefit will be measured. You establish **ownership** of benefits, identify the changes required and their stakeholder implications, and produce the basic information for the business case. Purpose in one line: agree *why* you're investing and *what* benefits you expect, and make sure each is measurable and owned.

**Step 2 — Planning benefits realization.**
You finalize the measurement of benefits and changes, get all stakeholders to agree their responsibilities and accountabilities, and produce the **benefits plan** as part of the business case. This step requires a thorough **stakeholder analysis** *before* the dependency network and benefits plan can be finalized. The full analysis includes: a full description of benefits, measures for all benefits, **baseline analysis (As-Is vs. To-Be)**, ownership of changes and actions, success criteria, and the **benefits dependency network** (see 2.7).

**Step 3 — Executing the benefits plan.**
You carry out the plan — implement the technology *and* the organizational changes — while monitoring progress against the planned benefits.

**Step 4 — Reviewing and evaluating the results.**
After implementation, you check which benefits were actually realized versus planned. This is where the honesty of the approach shows: you explicitly compare promise against outcome (the "benefits review" from the from→to table).

**Step 5 — Establishing the potential for further benefits.**
Having reviewed, you ask what *additional* benefits could now be pursued — often things that only became visible once the system was in use. This feeds back into the cycle, which is why the process is iterative.

**Exam angle:** Be able to list and briefly explain all five steps. A common trap is stopping at "implement." Emphasize that the process *continues past go-live* into review (Step 4) and further benefits (Step 5), and that it loops. A one-line memory hook: **Identify → Plan → Execute → Review → Exploit further.**

## 2.5 Drivers and investment objectives — the "why"

**Business drivers** are the forces — internal or external — creating pressure for the organization to change. They are the *reason* the investment is even on the table.

Types of business drivers the course highlights:
- **Internal vs. external** — e.g., an internal driver might be rising operating costs; an external driver might be a new competitor or a regulation.
- The three **value disciplines**: **product/service leadership, customer intimacy, operational excellence** (the strategic stance the organization competes on).
- The portfolio categories **strategic, high potential, key operational, support** (how critical a given system is to the business — this comes from the application-portfolio thinking in Ward & Daniel).

**Investment objectives** are what the organization wants to achieve from the investment. They sit **at the level of the organization**, they must **address the drivers** (an objective that doesn't respond to a real driver is pointless), and they act as the **success criteria** for the project.

Crucially, investment objectives should be **S.M.A.R.T.**:
- **S**pecific — clearly defined, not vague;
- **M**easurable — you can tell whether you hit it;
- **A**chievable — realistic given resources;
- **R**elevant — connected to the drivers and strategy;
- **T**ime-bounded — has a deadline.

*Example of the chain:* a driver might be "competitors are processing orders faster and we're losing customers" (external driver) → investment objective "reduce average order-processing time from 5 days to 1 day within 12 months" (SMART, addresses the driver) → from which specific benefits will flow.

**Exam angle:** Know the difference between a **driver** (the pressure/reason) and an **objective** (the targeted outcome that responds to the driver). And be ready to state that objectives should be SMART and must link back to drivers.

## 2.6 Benefits and the four benefit types

**What is a benefit?** A benefit is an advantage realized by a specific stakeholder as a result of the change. Two properties are stressed:

- Benefits are **specific to an individual or group** — someone is "benefiting."
- Benefits are **owned** by a stakeholder — someone is "responsible" for realizing it. Each investment objective is likely to give rise to a number of benefits for different stakeholders.

A central Ward & Daniel claim: **all business performance improvements are measurable in some way, and so are all the benefits delivered by information systems.** Some can be measured directly (e.g., staff reductions from automation, fewer product rejects from better production control), and many of those can be converted into financial values. Even softer things (customer satisfaction, staff sentiment) can be measured with appropriate methods. The hard rule: **if there is no possible way of measuring a benefit, it should be discarded** — though the course notes that even opinions and views can often be measured in some way, so genuinely unmeasurable benefits are rare.

A subtle but examinable nuance: benefits are not *only* designed in advance. Drawing on **sociomaterialism (e.g., Orlikowski)**, the course notes that benefits can also **emerge from unexpected patterns of use** — people use a system in ways the designers didn't anticipate, and value appears that nobody planned. This is part of why Step 5 (further benefits) and the iterative nature of the process matter.

**The four types of benefit** — this is a classic exam item; learn the ladder of increasing "hardness":

1. **Observable benefit** — judged against **criteria using expert judgement**. You can tell it happened, but only through informed opinion, not a hard number. *Example:* "staff morale appears improved" as assessed by managers.
2. **Measurable benefit** — you **can measure** the current level, **but cannot estimate the improvement** in advance. You know the metric exists and can track it, but you can't forecast how much it will get better. *Example:* you can measure current customer-complaint volume, but you can't reliably predict how much the new system will reduce it.
3. **Quantifiable benefit** — the **improvement can be forecasted**. You can put a number on the expected change. *Example:* "we expect order-processing time to fall from 5 days to 1 day."
4. **Financial benefit** — a **financial formula can be applied to compute a monetary value.** This is the hardest/strongest type because it expresses the benefit in euros/dollars. *Example:* the 4-day reduction in processing translates to €X saved labour cost per year.

**Exam angle:** The ordering and the precise distinction between *measurable* and *quantifiable* is the trap here. The key line: a **measurable** benefit can be measured but the *improvement cannot be forecast*; a **quantifiable** benefit is one where the *improvement can be forecast*. Financial is quantifiable *plus* a money value. Be ready to classify a given example into the right type.

## 2.7 Business changes, enabling changes, and the Benefits Dependency Network (BDN)

This is the single most important framework on Day 1. **Benefits are the result of changes** — not of the technology alone. Two precisely-defined kinds of change:

- **Business changes** — *"the new ways of working that are required to ensure that the desired benefits are realized."* These are the **new ongoing ways of working** in the organization (they persist, at least until the next change initiative). Think **process changes** — permanent shifts in how people operate. *Example:* "all orders are now entered through the new system at point of sale."

- **Enabling changes** — *"changes that are prerequisites for achieving the business changes, or that are essential to bring the system into effective operation."* These are usually **one-off activities** rather than ongoing ways of working. Think **one-time changes** — things you do once to make the business changes possible. *Example:* training all staff on the new system, defining new data codes, redefining job responsibilities.

The mnemonic from the lecture: **Enabling changes = one-time changes; Business changes = (ongoing) process changes.**

### The Benefits Dependency Network (BDN)

The BDN is the diagram that ties everything together. Read it **right to left** for logic (what we want → what delivers it) but it's drawn **left to right** as a flow. Its five columns, in order:

**IS/IT Enablers → Enabling Changes → Business Changes → Business Benefits → Investment Objectives** (with **Drivers** sitting at the far right, behind the objectives).

What each column means and how they connect:

- **IS/IT Enablers** (far left) — the technology and systems being provided (e.g., a new scanning and stock-control system, an ERP finance module). These are the *tools*.
- **Enabling Changes** — the one-off things you must do to make the technology usable and to set up the business changes (e.g., "new codes for all stock items," "staff attended training course," "redefined job responsibilities").
- **Business Changes** — the new ongoing ways of working the enablers and enabling changes make possible (e.g., "dispatch scanning operational," "new scheduling process on all lines," "single business plan in use").
- **Business Benefits** — the advantages that result from those new ways of working (e.g., "reduced number of dispatch errors," "reduced agency labour costs," "reduction in debtor days").
- **Investment Objectives** — the organizational outcomes the benefits add up to (e.g., "simplify and automate all business transactions," "integrate key processes and systems," "improve financial control of business assets").
- **Drivers** — the external/internal pressures behind the objectives (the ultimate "why").

The arrows show **dependency**: each benefit *depends on* specific business changes, which *depend on* enabling changes, which *depend on* the IS/IT enablers. This makes explicit a truth that traditional IT projects ignore — **the technology on the left is worthless unless the chain of changes in the middle actually happens.** If you install the system but skip the training (enabling change) and never adopt the new scheduling process (business change), the benefit never materializes.

**Exam angle:** You should be able to (a) name the five columns in order, (b) define business change vs. enabling change with the one-off vs. ongoing distinction, and (c) explain *why* the network matters — it forces you to trace every claimed benefit back through the changes and enablers needed to achieve it, exposing benefits that have no realistic path to delivery. If given a mini-scenario, be ready to slot items into the right column.

## 2.8 Stakeholders, ownership, and measurement

Three threads run through benefits management that the exam may probe:

- **Stakeholder analysis is a prerequisite.** Before the BDN and benefits plan can be finalized (Step 2), you must complete a thorough stakeholder analysis — identifying who benefits, who must change, and who owns each benefit and each change. Recall Nelson: ineffective stakeholder management is the #2 cause of IT project failure, so this is not a formality.

- **Ownership.** Every benefit and every change needs an owner — a named stakeholder accountable for realizing it. Unowned benefits tend not to happen.

- **Measurement and baselines.** For every benefit you specify a **measure** and a **baseline** (the As-Is level), so that after the project you can judge the improvement against the To-Be target. This is what makes Step 4 (review) possible and honest.

## 2.9 Moving toward financial appraisal: ROI (a bridge to later topics)

Benefits management ends by pushing toward putting numbers on value. The course introduces **Return on Investment (ROI)** as a tool for measuring the efficiency of an investment.

- **ROI** measures the return generated relative to the cost of the investment. Conceptually: you take the gains/cost-savings produced by the investment, net them against the costs, and divide by the costs.
- The decision rule given: if the **ratio is greater than 0** (i.e., returns exceed costs), the investment may be considered beneficial (ISACA 2012; Schmidt 2011).
- ROI requires the **initial cost**, the **investment made**, and the **cost savings** achieved due to the new investment.

This is just the doorway — the Costs lecture and the Real Options topic go much deeper into financial appraisal (NPV, IRR, TCO, option premiums). For Day 1, understand ROI conceptually as "did the money we got back exceed the money we put in, and by enough to be worth it?"

**Exam angle:** You're unlikely to be asked to compute a complex ROI on Day-1 material, but be ready to explain what ROI is, what it needs as inputs, and the basic decision rule (positive return ⇒ potentially worthwhile). Note its limitation as a single-number, static view — a point that becomes central when real options are introduced later.

---

# PART 3 — TYING IT TOGETHER (THE DAY-1 STORY IN ONE PASS)

Here is the whole Day 1 narrative as a single connected argument, which is the best way to hold it for a closed-book exam:

IT projects fail roughly two-thirds of the time, and **Nelson (2008)** shows the causes are overwhelmingly **people and process**, not technology — with poor estimation/scheduling, weak stakeholder management, and insufficient risk management leading the list. A **business case** is the governance instrument that fights this: a **plausible, well-reasoned, well-evidenced, well-analyzed** argument that an IT investment is worth making, structured as **why → what → how** and used to **initiate, monitor, and evaluate** the project.

The deepest reason IT projects underdeliver is captured by **Ward & Daniel's benefits management**: technology alone yields nothing — **benefits are realized only through organizational change**. Hence the shift **from technology delivery to benefits delivery**, with business managers in control and stakeholders involved. Benefits management runs as a five-step iterative process — **identify, plan, execute, review, exploit further** — anchored in **drivers** (the why) that lead to **SMART investment objectives**, which give rise to **benefits** (observable → measurable → quantifiable → financial) owned by stakeholders and tied to **measures and baselines (As-Is vs. To-Be)**.

The tool that makes the logic explicit is the **Benefits Dependency Network**: **IS/IT enablers → enabling changes (one-off) → business changes (ongoing) → benefits → objectives**, behind which sit the **drivers**. It forces you to prove that every claimed benefit has a real path through the changes needed to deliver it. Finally, value gets pushed toward numbers — **ROI** being the first, simplest financial lens, with richer methods to come.

---

# QUICK-FIRE SELF-TEST (cover the answers)

1. **Define benefits management (Ward & Daniel).** → The process of organizing and managing such that the potential benefits arising from the use of IS/IT are actually realized.
2. **Why do IT projects fail (Nelson)?** → ~2 in 3 fail; causes are mostly people (43%) and process (45%), not technology; top three: poor estimation/scheduling, ineffective stakeholder management, insufficient risk management.
3. **Name the five benefits-management steps.** → Identify & structure benefits → plan benefits realization → execute the plan → review & evaluate results → establish potential for further benefits (iterative).
4. **Four benefit types, hardest distinction?** → Observable (expert judgement) → Measurable (can measure, can't forecast improvement) → Quantifiable (improvement can be forecast) → Financial (money value). Measurable vs. quantifiable = whether the *improvement* can be forecast.
5. **Business change vs. enabling change?** → Business change = new ongoing way of working (process change). Enabling change = one-off prerequisite to make business changes/system operation possible.
6. **Name the BDN columns in order.** → IS/IT enablers → enabling changes → business changes → business benefits → investment objectives (drivers behind objectives).
7. **What makes a business case rigorous?** → Plausible, well-reasoned, well-evidenced, well-analyzed.
8. **Driver vs. investment objective?** → Driver = the internal/external pressure (the why); objective = the SMART organizational outcome that addresses the driver and serves as success criterion.
9. **As-Is vs. To-Be?** → Current state before the project vs. target state after; the gap defines the benefit and the needed changes.
10. **What is the from→to shift?** → From technology delivery / value-for-money / IT implementation / stakeholders subjected-to / audits → to benefits delivery / value-for-money / change management / stakeholders involved / benefits review.

---

*End of Day 1 summary. Next up (Day 2): Costs and Risk Management — which build directly on the benefits and BDN foundations laid here (costs also attach to enablers, enabling changes, and business changes; and risk management is the #3 failure cause from Nelson).*
