# Day 2 Study Summary — Business Case Development for IT Projects
## Topic block: Costs + Risk Management

*University of Twente — covers Lecture 03 (Costs in BCD for IT, Harmelink), the Costs/Benefits workshop (Harmelink), the Risk Management lecture (Effing), Peixoto et al. (2014), and the relevant parts of Nelson (2008) and Ward & Daniel (2012). This is everything you need to fully understand the costs side and the risk side of a business case.*

---

## How to use this summary

Same approach as Day 1: read it through once, then test yourself by covering the explanations and reproducing each definition, classification, and formula from memory. The exam is **closed-book**, so recall is what counts. **"Exam angle"** flags points the exam is especially likely to test — and on Day 2 there are two near-certain ones: the **risk-management formulas** (mitigation/contingency/reduction/exposure) and the **risk vs. ethical issue** distinction, which appears verbatim in the example-answer file.

A note on sources: because you asked for them, I've attributed the key claims to the specific lecture or paper they come from, using short tags like *(Harmelink, Lecture 03)* or *(Peixoto et al., 2014)*. A full source list sits at the end. Costs and Risks are each weighted ~5% on the individual exam, but they're also two of Nelson's top-three failure causes, so they punch above their point weight.

A reminder of where this connects to Day 1: costs attach to exactly the same chain as benefits in the **Benefits Dependency Network** — IS/IT enablers, enabling changes, and business changes all *cost money*, just as they *deliver benefits*. So Day 2 is the mirror image of Day 2's benefits material. Keep the BDN in mind throughout.

---

# PART 1 — COSTS IN BUSINESS CASE DEVELOPMENT

The Costs lecture (Harmelink, Lecture 03) is organized into four blocks, and this summary follows the same logic: (1) cost definitions and types, (2) the link between benefits and costs, (3) costs and ways of working, and (4) cost estimation methods.

## 1.1 Costs: definitions and types

### Tangible vs. intangible costs

The starting distinction *(Harmelink, Lecture 03)*:

- **Tangible costs** are **measurable** — you can put a clear number on them. *Example:* the purchase price of server hardware, or the licence fee for software.
- **Intangible costs** are real costs that are hard to measure directly. The lecture explicitly confirms that **intangible costs are possible in IT projects**, giving two examples: **loss of employer goodwill** and **loss of customer satisfaction**. These are genuine costs to the organization even though you can't read them off an invoice.

The conceptual framing the lecture opens with — *"Time = Money = Costs = Investment?"* — is a prompt to think about how the resources you spend (especially people's time) translate into money, and whether that money is a cost (consumed) or an investment (expected to generate return). For the exam, the takeaway is that costs are broader than the obvious cash outlays; a complete business case must surface intangible and time-based costs too.

### Costs according to Ward & Daniel (2012)

This is the **named classification** you should know cold *(Harmelink, Lecture 03, citing Ward & Daniel 2012)*. Ward & Daniel split IT-project costs into five categories:

1. **Purchase costs** — hardware, software, and services bought in. *Example:* buying servers, software licences, or a consultant's implementation services.
2. **Internal system development costs** — the cost of your own people building the system, measured in **internal FTEs** (full-time-equivalent staff effort). *Example:* the salary-time of your in-house developers writing custom modules.
3. **Infrastructure costs** — the underlying technical environment the system needs (networks, data centres, platforms).
4. **Costs of carrying out the business changes** — the **"soft" costs** of making the organizational changes happen, such as **training**, change management, and redesigning processes. This category is the cost-side twin of the *business changes* and *enabling changes* from the Benefits Dependency Network (Day 1). *Example:* the cost of training all staff on the new system, or of paying people while they adapt to new ways of working.
5. **Ongoing costs** — the recurring costs of running and maintaining the system after go-live. *Example:* annual maintenance contracts, support staff, licence renewals.

**Exam angle:** A likely question is "name and explain the cost categories according to Ward & Daniel." Learn all five, and be ready to give an example of each. The category most students forget is #4 (cost of business changes / soft costs like training) — and it's the most conceptually important because it embodies the Day 1 lesson that **the technology is only part of the cost; making people work differently costs money too.**

### Total Cost of Ownership (TCO)

**TCO** is the second cost-classification framework you must know *(Harmelink, Lecture 03 and the Costs/Benefits workshop)*. TCO captures the *full* cost of an IT asset across its entire life — not just the sticker price at purchase, but everything needed to own and run it over time. The lecture presents TCO as a wheel with eight components around a central "TCO" hub:

- **Hardware cost**
- **Software cost**
- **Software functionality**
- **Software architecture and scalability**
- **Time to implementation**
- **User training**
- **Support and maintenance**
- **Data architecture**

The point of TCO is that organizations routinely underestimate cost by looking only at the purchase price. A cheap system that needs heavy training, constant maintenance, and a costly data-architecture overhaul may have a *higher* TCO than a more expensive system that's easy to run. *Example:* "free" open-source software can have a high TCO once you add the support, integration, and training it demands.

**Exam angle:** Be able to (a) define TCO as the complete cost of owning an asset across its whole life-cycle, not just acquisition, and (b) explain *why* it matters — it prevents the classic mistake of judging an investment on purchase price alone. You don't need to recite all eight wheel segments perfectly, but know the spirit (hardware + software + implementation + training + support/maintenance + architecture/scalability + data). The course manual's suggested outline explicitly asks for a **TCO analysis** in the costs section, so it's expected knowledge.

**TCO vs. Ward & Daniel — how they relate:** Both are ways of making sure you capture *all* the costs. Ward & Daniel's classification is organized by *type of resource* (purchase, internal development, infrastructure, change, ongoing); TCO is organized by *life-cycle completeness* (everything from acquisition through to support and data architecture). They overlap heavily — e.g., "ongoing costs" in Ward & Daniel ≈ "support and maintenance" in TCO. In your business case you can use either or both as a checklist so nothing is missed.

## 1.2 The link between benefits and costs

This is the conceptual bridge back to Day 1 *(Harmelink, Lecture 03 and Costs/Benefits workshop, drawing on Miguens, da Silva & Guerreiro 2018)*. The chain of reasoning is:

> **Benefits are realized through activities → activities require resources → different resources are different types of costs.**

In other words, every benefit you claimed in the benefits dependency network has a *cost footprint*: to get the benefit you must perform certain activities (the enabling and business changes), and those activities consume resources (people, technology, infrastructure), each of which is a cost. This is why the workshop asks you to **identify all costs that drive the Changes, the Enabling Changes, and the IT/IS Enablers** — the same three left-hand columns of the BDN from Day 1, now viewed through a cost lens.

**Exam angle:** Be ready to explain the benefits–costs link in one clean sentence: *benefits are delivered by activities, activities need resources, and resources are costs — so every benefit traces to a cost, along the same dependency chain as the BDN.* This is the single most important conceptual point in the costs block because it ties costs to the whole benefits-management philosophy rather than treating them as a separate spreadsheet.

## 1.3 Costs and ways of working

This block reinforces that **how you organize the work changes the cost profile** *(Harmelink, Lecture 03)*. The major shift the lecture highlights is from traditional, deterministic, plan-everything-upfront approaches toward **Agile and DevOps** ways of working (see also 1.4 below). The cost implication:

- In a **traditional/deterministic** approach, you try to predict the full scope and the resources needed in advance, then cost that plan.
- In an **Agile/DevOps** approach, you instead **plan the resources (a team for a period) and see what you can deliver in that time.** The cost question flips from "how much will this fixed scope cost?" to "given this budget/team, what's the most valuable thing we can build?"

This matters because, as the lecture notes, **scopes often change in IT projects, so the projections change too** — which is exactly why fixed up-front cost predictions so often fail (echoing Nelson's #1 mistake, poor estimation/scheduling).

**Exam angle:** Understand that the *way of working* (deterministic vs. agile) shapes how you estimate and control costs, and that agile reframes costing around fixed time/resources and variable scope rather than fixed scope and variable cost.

## 1.4 Cost estimation methods

This is the most detailed cost sub-topic and a strong exam candidate. The big question the lecture poses: **do you trust experts or models to estimate costs?** *(Harmelink, Lecture 03)*

### The headline research finding

**Jørgensen (2004)** — the key cited source here — found that studies show **no clear favouring of expert estimation over model-based estimation** *(Harmelink, Lecture 03, citing Jørgensen 2004, "Top-down and bottom-up expert estimation of software development effort")*. Neither approach is reliably better; each has strengths and weaknesses. This is an important, citable, exam-ready conclusion: **there is no single best estimation method.**

### Expert judgement

**Expert judgement** uses experienced people who have developed **heuristics** (rules of thumb) for estimating costs *(Harmelink, Lecture 03)*.

- **Strength:** it works *better than models* on projects where **estimation models do not cover the specific domain knowledge** — i.e., novel or unusual projects where no good model exists.
- **Weaknesses:** experts can be **strongly biased**, and they can be **misled by irrelevant information** (e.g., anchoring on a number someone mentioned that has nothing to do with the real effort).

### Model-based / parametric estimation: COCOMO

**COCOMO (Constructive Cost Model)**, developed by **Barry Boehm**, is the lecture's example of a **parametric model** *(Harmelink, Lecture 03)*. A parametric model estimates cost/effort by feeding measurable parameters (like software size and a set of cost-driver ratings) into a formula. COCOMO II, for instance, takes inputs such as **source lines of code (SLOC)**, scale drivers (e.g., process maturity, team cohesion), and cost drivers (e.g., required reliability, product complexity, personnel capability) and computes an effort/cost estimate.

The lecture frames this as moving **"from predicting code complexity to funding capacity"**: COCOMO and other **deterministic methods treat software as predictable**, but because scopes change, the predictions drift — which is why agile/DevOps approaches (plan resources, see what fits the time) have risen as an alternative.

### Measuring the "size" of IT (inputs to estimation)

To estimate, you often need a measure of software size/complexity *(Harmelink, Lecture 03)*. Two methods given:

- **Lines of code (LOC/SLOC)** — simply count the lines. *Benefit:* simple and objective. *Downside (be ready to discuss):* it rewards verbose code, is language-dependent, can't be known accurately upfront, and counts quantity not value.
- **Function Point Analysis (FPA)** — instead of counting lines, you (1) identify the *functions* the software provides, (2) categorize each as one of five types — **outputs, inquiries, inputs, internal files, external interfaces** — and (3) assign function points based on each function's complexity. FPA is more about *what the software does* than how many lines implement it, making it more language-independent.

### Best practices in cost estimation

The lecture's practical advice *(Harmelink, Lecture 03)*:

- **Use real-life/historical data where possible** (it cites ISBSG, a benchmarking dataset, as an example source).
- **Clarify your assumptions** — make explicit what you're assuming so the estimate can be judged and revised.
- **Use averages** rather than betting on a single optimistic point.

This dovetails with Nelson's (2008) best practices for the #1 failure cause (poor estimation/scheduling): use developer-based estimates, historical data, algorithms like COCOMO II, and treat estimation as **iterative refinement** — estimates presented as **ranges that narrow over time** (the "cone of uncertainty" / estimate-convergence graph) *(Nelson, 2008)*.

**Exam angle:** The most likely cost-estimation question asks you to **compare expert judgement vs. model-based (parametric) estimation**, including when each is preferable and their weaknesses, and to cite that **Jørgensen (2004) found no clear winner**. Also know COCOMO = Boehm's parametric model, and be able to name LOC and Function Point Analysis as size measures with one pro/con each. *(Note: the lecture explicitly marks the "Too many software estimation methods?" overview slide and the COCOMO calculator detail page as "NOT exam material," so don't memorize the long taxonomy of data-driven/expert/hybrid methods — focus on the expert-vs-model comparison, COCOMO as the parametric example, and the two sizing methods.)*

---

# PART 2 — RISK MANAGEMENT

The Risk Management lecture (Effing) builds on the strong reason from Day 1 that **insufficient risk management is the #3 cause of IT project failure** in Nelson's (2008) study (occurring in ~47% of projects) — and that the top three causes, including risk management, occurred in roughly half of all projects studied. So this isn't a peripheral topic; it's one of the proven make-or-break areas.

## 2.1 What is a risk? (definitions)

The lecture deliberately offers **several definitions** of risk to show it's a contested concept *(Effing, Risk Management lecture)*. Know at least the PMBOK one verbatim-ish, and recognize the others:

- **PMBOK (Project Management Institute):** a risk is *"an uncertain event or condition that, if it occurs, has a positive or negative effect on a project's objectives."* This is **the** definition to anchor on. Note the crucial nuance: a risk can be **positive or negative** — an "upside risk" is an *opportunity*, not just a threat.
- **Society for Risk Analysis (in Aven, 2016):** risk is *"the relation of a future activity to its consequences with respect to something that humans value."* (Emphasizes that risk is about what we *value*.)
- **Chowdhury & Arefeen (2011):** risk is *"the precursor to a problem; the probability that, at any given point in the software life cycle, the predicted goals cannot be achieved within available resources."*
- **Stoneburner et al. (2002):** risk is *"a function of the likelihood of a given threat source's exercising a particular potential vulnerability, and the resulting impact of that adverse event on the organization."* (A security-flavoured definition: likelihood × impact.)

**Exam angle:** If asked "what is a risk?", lead with the **PMBOK** definition and stress that risks can be **positive (opportunities) or negative (threats)** and are defined relative to **project objectives**. Mentioning that multiple definitions exist (security-flavoured, value-flavoured) shows depth.

### Risk vs. uncertainty (Peixoto et al., 2014)

A precise, examinable distinction *(Effing lecture, citing Peixoto et al. 2014)*:

- A **risk** is an event whose **probability of occurrence is known** — the **"known unknowns"** — and is therefore **susceptible to analysis**. You can estimate how likely it is and how bad it would be.
- An **uncertainty** is an event whose **probability is not known** — the **"unknown unknowns"** — and is therefore **not susceptible to (this kind of) analysis**. You know it *could* happen but can't put a number on it.

Project managers face both, and Peixoto et al. argue for broadening risk-management practice to pay more attention to the lack of knowledge that creates uncertainty.

**Exam angle:** "What is the difference between risk and uncertainty?" → Risk = known probability, known unknowns, analyzable; uncertainty = unknown probability, unknown unknowns, not analyzable. Use the "known unknowns vs. unknown unknowns" phrasing — it's memorable and exactly what the source says.

## 2.2 The risk management formulas (Effing) — HIGH PRIORITY

This is the single most likely thing to be tested from the risk block, because it's concrete and the lecture lays it out as a clean set *(Effing, Risk Management lecture)*. Learn every line:

- **Event** — *What could happen?* (the risk itself)
- **Probability** — *How likely is it to happen?*
- **Impact** — *How bad will it be if it happens?*
- **Mitigation** — *How can you reduce the **probability** (and by how much)?* → Mitigation attacks the **likelihood**.
- **Contingency** — *How can you reduce the **impact** (and by how much)?* → Contingency attacks the **consequences**.
- **Reduction = Mitigation × Contingency** — your total risk-reducing effect combines lowering probability *and* lowering impact.
- **Exposure = Risk − Reduction** — your remaining (residual) risk is the original risk minus what your reduction measures take off.

The clean mental model: a raw ("inherent") risk has some size driven by probability × impact. You apply **mitigation** (push probability down) and **contingency** (push impact down); together these give your **reduction**. What's left after reduction is your **exposure** (the residual risk you still carry).

*Worked example:* Suppose the risk is "the data migration corrupts customer records." **Mitigation** might be running automated validation scripts before go-live (lowers the *probability* of corruption). **Contingency** might be keeping a full backup so you can roll back (lowers the *impact* if corruption happens anyway). The combined effect is your **reduction**; whatever chance-and-damage remains is your **exposure**.

**Exam angle:** Be able to (a) define each of the six terms, (b) state the two formulas exactly — *Reduction = Mitigation × Contingency* and *Exposure = Risk − Reduction* — and crucially (c) explain the **mitigation vs. contingency** distinction: **mitigation reduces probability, contingency reduces impact.** That mitigation/contingency split is a classic "what is the difference between X and Y" item for this exam.

## 2.3 The risk management process

The lecture frames risk management as two big phases, each with three activities *(Effing, Risk Management lecture)*:

**Risk assessment**
1. **Risk identification** — find and document the risks.
2. **Risk analysis** — work out the relationships between risk factors and project outcomes.
3. **Risk prioritization** — rank the risks so you focus on what matters most.

**Risk control**
4. **Risk-management planning** — decide what to do about each risk.
5. **Risk resolution** — actually carry out the responses.
6. **Risk monitoring** — keep watching, because new risks appear and known risks change.

The overarching purpose, per the lecture (echoing the literature), is that **risk management ensures almost all problems are discovered early enough that there's time to recover without missing schedules or overspending the budget** *(Effing lecture; the phrasing comes from the risk-management literature cited in Peixoto et al. 2014)*. Note the explicit link to the three core project-control measures — **Time, Money, and Scope/Quality** (the "iron triangle") — that risk management exists to protect.

### The PMBOK six processes (Peixoto et al., 2014)

Peixoto et al. (2014) — the dedicated risk paper — present PMBOK's **six risk-management processes**, which are a more granular version of the same idea *(Peixoto et al., 2014)*:

1. **Plan risk management** — set up how you'll handle risk on this project.
2. **Identify risks** — document risks that may affect objectives.
3. **Perform qualitative risk analysis** — judge likelihood and consequences *subjectively* to prioritize.
4. **Perform quantitative risk analysis** — for the most important risks, assess probability and impact *numerically* and rigorously.
5. **Plan risk responses** — develop actions to enhance opportunities and reduce threats.
6. **Control risks** — track defined risks, spot new ones, and run the response plans.

A key empirical point from the paper: project managers tend to invest effort in the **early** phases (planning, identification, analysis) but **neglect the risk-control phase** later, under time and resource pressure — and the paper warns this is a tendency to avoid. Related finding it cites: **the most successful projects undertook more risk-management practices, and the earlier risk management started, the more successful the project** (Elkington & Smallman).

**Exam angle:** Know the **two-phase structure (assessment / control)** with its activities from the Effing lecture, and recognize PMBOK's **six processes** from Peixoto. The distinction between **qualitative** (subjective, prioritizing) and **quantitative** (numeric, for the high-priority risks) analysis is examinable.

## 2.4 Qualitative analysis: the Probability–Impact (PxI) matrix

The core qualitative tool *(Peixoto et al., 2014)*. Each risk is scored on a **probability scale** and an **impact scale**, and the two are combined in a **PxI matrix** (probability × impact). Risks are then rated and colour-coded:

- **Green = low impact** → just **monitor and control**.
- **Yellow = moderate impact** → **periodic revision** + mitigation response plans.
- **Red = high impact** → **urgent attention** + avoidance/preventive response plans.

The matrix tells the team *which response type fits which risk* — high-impact red risks get preventive avoidance, moderate yellow risks get mitigation/contingency, low green risks just get monitored *(Peixoto et al., 2014, Table 7)*.

## 2.5 Quantitative analysis: Expected Monetary Value (EMV)

For the highest-priority risks, you go numeric *(Peixoto et al., 2014)*. The key tool is **Expected Monetary Value (EMV)**, often computed with a **decision-tree** technique: you weigh each possible outcome of a risk by its probability and its monetary consequence to get an expected value, which lets you compare response alternatives and decide how much it's worth spending to respond. *Example from the paper:* a risk was analyzed with a decision tree, an EMV was computed, and "make minor technical changes" came out as the best response given the objectives. (Decision trees reappear later in the course under Real Options — same underlying technique.)

## 2.6 Risk responses (the four strategies)

When planning responses, each risk gets a response strategy *(Peixoto et al., 2014; also reflected in the Effing lecture's risk-register columns)*. The four classic strategies — note each has a *threat* version and an *opportunity* version, consistent with risk being positive or negative:

- **Avoid / Explore** — *Avoid:* eliminate the threat entirely (e.g., drop the risky feature). *Explore (the opportunity twin):* make sure you capture an upside.
- **Mitigate / Enhance** — *Mitigate:* reduce a threat's probability or impact. *Enhance:* increase an opportunity's probability or impact.
- **Transfer / Share** — *Transfer:* shift a threat to a third party (e.g., insurance, or outsourcing the risky work). *Share:* share an opportunity with a partner.
- **Accept** — take no action and live with it. Crucially, the paper stresses **a response plan should be identified for *all* risks, even if the response is "accept"** — accepting must be a conscious documented decision, not an oversight.

The paper also maps responses to the matrix zones with the labels **Preventive (avoid)** for high/red, **Contingency (reduce/mitigate)** for moderate/yellow, and **Corrective (mitigate/accept)** for low/green *(Peixoto et al., 2014, Table 7)*.

**Exam angle:** Memorize the **four response strategies — Avoid, Mitigate, Transfer, Accept** (with their opportunity twins Explore, Enhance, Share). A frequent question is to name them and give an example of each. Don't forget that **"accept" still requires a documented response plan.**

## 2.7 The risk register and risk breakdown structure

Two documents to know *(Peixoto et al., 2014)*:

- **Risk register** — the **main output** of risk management: a living document with one record per risk, capturing its ID/description, qualitative and quantitative evaluation, the response plan, the **risk owner**, and its status during monitoring and control. Because risk management is **iterative and continuous**, the register must be **regularly updated** as new risks appear and old ones change.
- **Risk breakdown structure (RBS)** — organizes identified risks by **type of source**. Peixoto et al. classify sources as **external, commercial, project management, and technical**. (Elkington & Smallman, cited in the paper, use a similar typing: business risks, procurement risks, management risks, technical risks.)

Tools used to *identify* risks include **brainstorming meetings, documentary review (of contracts, the work breakdown structure, meeting records, etc.), and decision-tree analysis** *(Peixoto et al., 2014, Table 3)*.

**Exam angle:** Know that the **risk register is the central output** and that it's continuously updated, and be able to name a few **risk source categories** (external, commercial, project-management, technical).

## 2.8 Risk vs. ethical issue — HIGH PRIORITY (cross-links to Day 3 ethics)

This exact distinction appears in the example-questions/norm-answers file, so treat it as near-guaranteed. Although ethics is a Day 3 topic, the *contrast* is best learned here alongside the risk definitions.

- A **risk** is an **uncertain event** that positively or negatively impacts the **process or outcomes of the project** (PMBOK). It primarily affects the **business outcome**.
- An **ethical issue** is more of a **potential impact with moral effects on stakeholders** in or outside the project. It can have **societal** impact, not just business impact. Whether it's perceived as good or bad **depends on the viewpoint and (moral) belief system of the stakeholder** — it's something viewed through a **philosophical angle**, differing in the extent of perceived good or bad (morality), and it concerns **norms and values**.

**A risk that is NOT an ethical issue** (the second part of the example question): a purely project-related matter such as a **limited budget overrun, unforeseen operational costs, or a temporary dip in performance** where no system depends on it for vital functionality. These affect the project but carry no moral/societal dimension.

**Exam angle:** Be ready to (a) state the difference — *risk = uncertain event affecting project outcomes; ethical issue = potential moral impact on stakeholders/society, viewpoint-dependent, about norms and values* — and (b) give an example of a risk that is not an ethical issue (budget overrun, operational cost surprise, minor non-critical performance dip). This is almost certainly worth points; lock it in.

---

# PART 3 — TYING IT TOGETHER (THE DAY 2 STORY IN ONE PASS)

Here's the connected narrative to hold for the exam:

Day 1 showed that benefits are realized only through change. Day 2's **costs** are the mirror image: **benefits come from activities, activities consume resources, and resources are costs** *(Harmelink, Lecture 03; Miguens et al. 2018)* — so every benefit in the **Benefits Dependency Network** has a cost footprint on the same enablers, enabling changes, and business changes. To capture costs fully you avoid the trap of pricing only the purchase, using two checklists: **Ward & Daniel's five categories** (purchase, internal development, infrastructure, business-change/soft costs, ongoing) and **Total Cost of Ownership** (the whole-life cost including training, support, maintenance, and architecture). Estimating those costs is genuinely hard — **Jørgensen (2004) found no clear winner between expert judgement and model-based estimation** *(Harmelink, Lecture 03)*; experts handle novel domains but are biased, while parametric models like **COCOMO (Boehm)** treat software as predictable but break when scope shifts — which is why **agile/DevOps** reframes costing around fixed time and variable scope, and why best practice is historical data, explicit assumptions, averages, and iterative range-based estimates (the cone of uncertainty, per Nelson 2008).

**Risk** is the other half of a credible business case and, per **Nelson (2008)**, the #3 failure cause. A **risk** is an uncertain event with a positive or negative effect on project objectives (PMBOK), distinct from **uncertainty** (unknown probability; "unknown unknowns") *(Peixoto et al., 2014)*. You manage it through **assessment** (identify → analyze → prioritize) and **control** (plan → resolve → monitor) — PMBOK's six processes — using a **qualitative PxI matrix** to triage (red/yellow/green) and **quantitative EMV/decision trees** for the big ones *(Peixoto et al., 2014)*. The Effing formulas are the operational core: **mitigation cuts probability, contingency cuts impact, Reduction = Mitigation × Contingency, and Exposure = Risk − Reduction.** Responses are **Avoid, Mitigate, Transfer, Accept** (with opportunity twins), all logged in the continuously-updated **risk register**. Finally, a **risk is not the same as an ethical issue**: a risk hits project outcomes, while an ethical issue is a viewpoint-dependent moral impact on stakeholders and society — the bridge into Day 3.

---

# QUICK-FIRE SELF-TEST (cover the answers)

1. **Tangible vs. intangible cost — define + IT example of intangible.** → Tangible = measurable (hardware price); intangible = real but hard to measure (loss of employer goodwill, loss of customer satisfaction). *(Harmelink, L03)*
2. **Ward & Daniel's five cost categories?** → Purchase costs; internal system development (FTEs); infrastructure; cost of carrying out business changes (soft costs, e.g. training); ongoing costs. *(Harmelink, L03 / Ward & Daniel 2012)*
3. **What is TCO and why use it?** → The full cost of owning an asset across its whole life (hardware, software, implementation, training, support/maintenance, architecture, data) — not just purchase price; prevents judging investments on sticker price alone. *(Harmelink, L03)*
4. **The benefits–costs link in one line?** → Benefits are realized through activities; activities need resources; resources are costs. *(Harmelink, L03 / Miguens et al. 2018)*
5. **Expert judgement vs. model-based estimation — which wins?** → Neither; Jørgensen (2004) found no clear favouring. Experts: good for novel domains, but biased/misled. Models (COCOMO, Boehm): treat software as predictable, break on scope change. *(Harmelink, L03 / Jørgensen 2004)*
6. **Two ways to measure IT size?** → Lines of code (simple but language-dependent, rewards verbosity) and Function Point Analysis (counts functions by type: outputs, inquiries, inputs, internal files, external interfaces). *(Harmelink, L03)*
7. **Define risk (PMBOK) and note the key nuance.** → An uncertain event/condition that, if it occurs, has a positive or negative effect on project objectives — risks can be opportunities, not only threats. *(PMBOK, via Effing / Peixoto et al. 2014)*
8. **Risk vs. uncertainty?** → Risk = known probability, "known unknowns", analyzable; uncertainty = unknown probability, "unknown unknowns", not analyzable. *(Peixoto et al., 2014)*
9. **State the four risk formulas/terms relationships.** → Mitigation reduces probability; contingency reduces impact; Reduction = Mitigation × Contingency; Exposure = Risk − Reduction. *(Effing)*
10. **The two phases of risk management and their activities?** → Assessment (identify, analyze, prioritize) and Control (plan, resolve, monitor). *(Effing)*
11. **PMBOK's six risk processes?** → Plan risk mgmt; identify; qualitative analysis; quantitative analysis; plan responses; control. *(Peixoto et al., 2014)*
12. **Qualitative vs. quantitative risk analysis?** → Qualitative = subjective likelihood/impact via PxI matrix to prioritize; quantitative = numeric (e.g., EMV/decision trees) for the highest-priority risks. *(Peixoto et al., 2014)*
13. **The four risk response strategies (+ the catch on "accept")?** → Avoid, Mitigate, Transfer, Accept (opportunity twins: Explore, Enhance, Share). Even "accept" needs a documented response plan. *(Peixoto et al., 2014)*
14. **What is the risk register?** → The main, continuously-updated output: one record per risk with evaluation, response, owner, and status. *(Peixoto et al., 2014)*
15. **Difference between a risk and an ethical issue, + a risk that is NOT an ethical issue?** → Risk = uncertain event affecting project outcomes; ethical issue = viewpoint-dependent moral impact on stakeholders/society, about norms and values. Risk-not-ethical example: budget overrun, unforeseen operational costs, or a temporary non-critical performance dip. *(Example-answer file / PMBOK)*

---

## Sources used in this summary

- **Harmelink (2026), Lecture 03 — "Costs in Business Case Development for IT"** — cost definitions (tangible/intangible), Ward & Daniel cost categories, TCO, benefits–costs link, costs and ways of working, estimation methods (expert judgement, COCOMO, LOC, FPA), best practices. *(Source for §1.1–§1.4.)*
- **Harmelink (2026), Workshop 02 — "Benefits and Costs in BCD for IT"** — TCO and Ward & Daniel as cost checklists; costs driving Changes / Enabling Changes / IT-IS Enablers; benefits-realized-through-activities chain. *(Source for §1.1–§1.2; cites Miguens, da Silva & Guerreiro 2018.)*
- **Ward, J. & Daniel, E. (2012), *Benefits Management*** — the five cost categories; underpins the benefits–cost dependency logic. *(Source for §1.1.)*
- **Jørgensen, M. (2004), "Top-down and bottom-up expert estimation of software development effort"** — the finding that there's no clear winner between expert and model-based estimation; expert-judgement strengths/weaknesses. *(Source for §1.4.)*
- **Boehm — COCOMO (Constructive Cost Model)** — the parametric estimation example. *(Source for §1.4.)*
- **Effing (2026), Risk Management lecture** — the multiple risk definitions (PMBOK, Aven 2016, Chowdhury & Arefeen 2011, Stoneburner et al. 2002); the Event/Probability/Impact/Mitigation/Contingency framework and the Reduction and Exposure formulas; the assessment/control two-phase process. *(Source for §2.1–§2.3.)*
- **Peixoto, Tereso, Fernandes & Almeida (2014), "Project Risk Management Methodology: A Case Study of an Electric Energy Organization," *Procedia Technology*** — PMBOK's six processes; risk vs. uncertainty (known vs. unknown unknowns); PxI matrix and colour coding; EMV/decision trees; the four response strategies; risk register and risk breakdown structure; the empirical findings on risk-management practice and success. *(Source for §2.1, §2.3–§2.7.)*
- **Nelson, R. R. (2008), "IT Project Management: Infamous Failures, Classic Mistakes, and Best Practices," *MIS Quarterly Executive*** — risk management as the #3 failure cause and poor estimation/scheduling as #1; the cone of uncertainty and estimation best practices. *(Cross-referenced in §1.4 and §2 intro.)*
- **Example Questions & Norm Answers (BCDIT)** — the risk vs. ethical issue distinction and the "risk that is not an ethical issue" example. *(Source for §2.8.)*

---

*End of Day 2 summary. Next up (Day 3): Ethics — the heaviest single exam topic (10% of the individual exam), where the risk-vs-ethical-issue distinction from §2.8 becomes the doorway into the philosophical angles (Aristotle, Kant, Habermas, Levinas, Machiavelli) and the smart-cities ethics paper.*
