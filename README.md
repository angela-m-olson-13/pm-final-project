# RouteLogic Velocity, A Stream-lined Workflow for Our Experienced Drivers

> When drivers stop trusting their tools, they start looking for new ones — RouteLogic fixes the workflow before it becomes a churn problem.

**Angela Olson · Product Management Cohort · Sept 15-26 weekdays 2026** · https://github.com/angela-m-olson-13/pm-final-project

Prototype: https://apricot-rhodia-14.tiiny.site/

Presentation:  https://final-presentation.tiiny.site/

---

## Final Project Deliverables

### Slide 5 · Strategy
- **Problem:** Strategic crisis
If Route Logic does nothing for 12 months there is a real threat that the company will lose its standing in the market to leaner, more agile competitors for their logistics platform.

Moment of misery
The user of Route Logic today is compelled to use workarounds like spreadsheets, emails/texts, or even exploring their own with AI versus utilizing the platform. Users also have suggested willingness to look at competitors in the market to meet their needs.

Problem hook
Route Logic's complexity is doing our competitors' sales pitch for them - unless we act, users already solving their problems with workarounds will take their business somewhere that does not make them work this hard.
- **Value proposition:** For experienced drivers at regional delivery fleet companies, we will value simplicity in core features to avoid user workarounds and desire to look at competitor products.
- **Hypothesis:** Based on avg. daily time lost to manual workarounds increasing 3.4× (from ~9 min to 31 min over two years), I believe that solving compliance check friction for drivers will reduce daily workaround time per stop, as measured by a reduction in compliance check time back toward the ~9-min industry benchmark and improved workflow drop-off rates. I will protect Live Dispatch Board and Route Optimizer daily usage rates (must not decline). I will make a go/no-go decision after two weeks of post-launch data across all drivers to ensure adoption trends are stable before scaling, pivoting, or sunsetting.

### Slide 6 · Research
- **Competitive analysis:** The product demonstrates strong strategic value at the reporting and operational management layer, but is experiencing a critical erosion of trust at the frontline driver level due to compounding stability, latency, and usability failures. Core workflows — delivering a stop, receiving a route update, and operating without connectivity — are sufficiently broken that users have built parallel systems (WhatsApp groups, paper manifests, dispatcher phone calls) to compensate. Without urgent intervention on technical reliability and workflow simplicity, the platform risks losing renewals despite its differentiated administrative capabilities.

Drivers want to complete a full route shift efficiently, not losing time in the tool and with the tool having correct information.  A compounding issue of overall tool performance and complexity stops this from happening today.  The tool does not provide timely, correct information to provide real-time information to drivers and it is overly complicated to complete routine tasks, that are performed up to 30x/day that drivers want to spend little time on.  Drivers resort to Screenshots, paper, phone call, and tribal knowledge to complete their work.
- **Journey map:** Today's Process: 
Screenshot of the full stop list for the day
Navigation to stops referencing user tribal knowledge or paper notes
Mark a stop delivered and take multiple pictures in case of failure
If application fails, call the dispatcher to receive remaining stop list manually

Future Journey:
Shift starts → Route load instantly, off-line ready 
Route in Motion -> Overrides saved for next time
At Every Stop -> Routine data saved and one tap confirms
End of Shift -> Dispatch Dashboard matches reality, no calls needed

### Slide 7 · Blueprint
- **Roadmap:** # Feature Roadmap, Module 4 · RouteLogic Velocity

**Team:** 2 engineers + 1 designer + 1 CS lead

## Strategic anchors
- **Persona:** The Experienced Driver Who Has Given Up Trusting It
- **Primary metric:** In the workflow, expect to see time spend on compliance checks to decrease. This is the start of closing the gap. Ideally this should reduce to close to industry benchmarks of ~9min.
- **Moment of misery:** A compounding issue of overall tool performance and complexity. The tool does not provide timely, correct information to provide real-time information to drivers and it is overly complicated to complete routine tasks that drivers want to spend little time on.
- **Guardrail:** The Live Dispatch Board and Route Optimizer have daily usage metrics that are fairly high. This cannot drop - the users are trying each day because they must to do their job, but then the workarounds start as they go about their workflow.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| B1 One-Click Compliance Checklist | 5 | 2 | Quick Win | Now | Directly attacks the 14.6-min compliance moment of misery; pre-fill reuses existing data — low build cost for maximum primary metric impact. |
| B2 Smart Daily Report Auto-Fill | 4 | 4 | Major Project | Later | High value for the persona but AI-generated field population requires data-pipeline work that will strain a 2-engineer pilot team. |
| B3 Shift Handoff Wizard | 4 | 3 | Major Project | Next | The 6.8-min saving is real, but building a reliable multi-step wizard with state persistence risks the dispatch-board guardrail if it shares the same UI surface. |
| B4 Mobile-First Coordinator Dashboard | 4 | 5 | Major Project | Later | Addresses the complexity axis of the moment of misery, but a full responsive redesign is a multi-sprint rebuild — too risky for a 4-week pilot with a guardrail on daily dispatch usage. |
| B5 Step Progress Indicator | 3 | 1 | Fill-In | Now | Minimal dev cost; restores the experienced driver's sense of control within the existing workflow and preserves dispatch-board behaviour — no regression risk. |
| B6 Driver Alert Notifications | 4 | 2 | Quick Win | Next | Directly counters "tool does not provide timely, correct information"; push infra is usually low effort if data triggers already exist in the route optimizer. |
| B7 Contextual AI ETA Display | 3 | 5 | Time Sinker | Later | 11% adoption signals the persona has already stopped trusting it; rebuilding ML confidence takes far more than 4 weeks and risks eroding the primary metric benchmark. |
| B8 Fleet Analytics Manager View | 2 | 4 | Time Sinker | Cut | Serves an exec persona, not the experienced driver; does nothing for compliance time and pulls designer + engineer capacity away from the primary metric. |
| B9 Compliance Audit Trail Export | 2 | 1 | Fill-In | Cut | PDF export is a low-effort admin convenience; useful for the CS lead  but doesn't move the primary metric. |
| B10 In-App Coordinator Training | 2 | 2 | Fill-In | Cut | Targets new coordinators, not the experienced driver persona; could help CS lead during onboarding of the 3 accounts but is the wrong lever for the moment of misery. |

## Roadmap
### NOW, Pilot (4 weeks, 3 accounts)
- **B1 One-Click Compliance Checklist**, Directly attacks the 14.6-min compliance moment of misery; pre-fill reuses existing data — low build cost for maximum primary metric impact.
- **B5 Step Progress Indicator**, Minimal dev cost; restores the experienced driver's sense of control within the existing workflow and preserves dispatch-board behaviour — no regression risk.

### NEXT, GA Release (weeks 5-8)
- **B3 Shift Handoff Wizard**, The 6.8-min saving is real, but building a reliable multi-step wizard with state persistence risks the dispatch-board guardrail if it shares the same UI surface.
- **B6 Driver Alert Notifications**, Directly counters "tool does not provide timely, correct information"; push infra is usually low effort if data triggers already exist in the route optimizer.

### LATER, backlog
- **B2 Smart Daily Report Auto-Fill**, High value for the persona but AI-generated field population requires data-pipeline work that will strain a 2-engineer pilot team.
- **B4 Mobile-First Coordinator Dashboard**, Addresses the complexity axis of the moment of misery, but a full responsive redesign is a multi-sprint rebuild — too risky for a 4-week pilot with a guardrail on daily dispatch usage.
- **B7 Contextual AI ETA Display**, 11% adoption signals the persona has already stopped trusting it; rebuilding ML confidence takes far more than 4 weeks and risks eroding the primary metric benchmark.

### ✂ Cut List
- **B8 Fleet Analytics Manager View**, Serves an exec persona, not the experienced driver; does nothing for compliance time and pulls designer + engineer capacity away from the primary metric.
- **B9 Compliance Audit Trail Export**, PDF export is a low-effort admin convenience; useful for the CS lead  but doesn't move the primary metric.
- **B10 In-App Coordinator Training**, Targets new coordinators, not the experienced driver persona; could help CS lead during onboarding of the 3 accounts but is the wrong lever for the moment of misery.
- **PRD highlights:** # PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** One-Click Compliance Checklist
- **My finalized Must-Haves (after overriding the AI):** 1) Pre-filled checklist from existing dispatch data. The form auto-populates known fields (vehicle ID, route, shift start, driver ID) from the active session. Zero manual re-entry of data the system already holds.
2) Single submission action. One tap/click submits the completed checklist. No multi-step confirmation screens, no secondary "are you sure" dialogs.
3) Completion timestamp written to the compliance record. The system records when the checklist was submitted. This is the data source for measuring the primary metric (time-on-task reduction).
- **What I demoted from Must → Should/Won’t, and why:** 1) Inline validation with plain-language errors. If a required field is empty or out of range, the field highlights and shows a one-line fix instruction — not an error code. The driver does not need to hunt for what's wrong. ->  While this is really important this may impact feasible of timeline and should be a fast-follow feature.
2) Visible checklist status on the dispatch board. After submission, the driver's compliance status flips to "complete" on the Live Dispatch Board without a page reload. The guardrail metric depends on the dispatch board remaining the source of truth — this closes that loop.  -> While this helps with guardrail metric, this deviates slightly from the persona targeted and should be a fast-follow.

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** Situation → Outcome logic for the prototype to demonstrate.  Essentially the PRD outlines the situation by the user and the expected system behavior.  This is what makes the user stories come to life in terms of relating to the actual solution.

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** The PRD did not cover the situation where the user had a partial checklist completed and the dispatch board reflected the status "Pending - start checklist".  
Also what constituted the checklist was not clear, including what are typically good to auto-default vs having driver check every time.
- **My prototype, as a link or a screenshot (publish or share from your tool; in Lovable that is Share → Share Preview, in Bolt Publish → Web. No share URL? Screenshot the working flow):** routelogic-compliance-prototype.html
- **Prototype:** https://apricot-rhodia-14.tiiny.site/

### Slide 8 · Validation
# A/B Experiment Brief, RouteLogic (B2B)

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | One-Click Compliance Checklist |
| Persona | The Experienced Driver Who Has Given Up Trusting It |
| Expected outcome | Manual workarounds are reduced, the workflow steps - especially compliance checks - reduce in time and drop off rates to improve. |
| Primary success metric | Compliance check time-on-task (target ≤ 9 min).  Time-on-task starts when the driver opens the compliance checklist screen and ends when the confirmation screen is displayed following successful submission. Incomplete sessions (abandoned before submission) are excluded from the primary metric and tracked separately as a drop-off rate secondary metric. |
| Baseline rate | 14.6 min |
| Guardrail metric | Daily active sessions on the Live Dispatch Board and Route Optimizer are monitored per arm throughout the experiment. If the variant arm shows a statistically significant decrease vs. the control arm at any weekly check-in, the experiment is paused and the variant is rolled back regardless of primary metric performance. |
| Guardrail boundary | Daily usage of the Live Dispatch Board and Route Optimizer must not fall by more than 5% |
| Second guardrail | Workflow completion compliance must not drop before today's level of 48% |
| Minimum Detectable Effect | Compliance check time-on-task reduces at least 5.6min |
| Sample size per arm | 24 |
| Traffic split | 50/50 |
| Test duration | 3 weeks |
| Significance threshold | p<0.05 (95%) |

## Control vs. Variant
- **Control (A):** A compounding issue of overall tool performance and complexity where it is overly complicated for drivers to complete routine tasks.   The big pain point identified in the workflow was the time spent by drivers in marking a stop delivered.
- **Variant (B):** A redesigned compliance checklist screen combining two UX changes tested as a bundle:  1) auto-population of known session fields and 2) single-action submission. These are intentionally bundled because separating them would require a third arm the pilot team cannot support. The auto-population is expected to contribute the larger share of time reduction by eliminating re-entry of known fields; single-action submission is expected to reduce hesitation and confirmation-loop behavior. The follow-on isolation test will verify this if the bundle wins.
- **Held constant (isolation check):** Dispatch board, app version, route engine logic, core driver information (name, vehicle, route), overall workflow from coordinator view.

## Hypothesis
> I believe that One-Click Compliance Checklist for The Experienced Driver Who Has Given Up Trusting It will result in Manual workarounds are reduced, the workflow steps - especially compliance checks - reduce in time and drop off rates to improve., as measured by a Compliance check time-on-task reduces at least 5.6min change in Compliance check time-on-task (target ≤ 9 min).  Time-on-task starts when the driver opens the compliance checklist screen and ends when the confirmation screen is displayed following successful submission. Incomplete sessions (abandoned before submission) are excluded from the primary metric and tracked separately as a drop-off rate secondary metric. within 3 weeks. We will protect Daily active sessions on the Live Dispatch Board and Route Optimizer are monitored per arm throughout the experiment. If the variant arm shows a statistically significant decrease vs. the control arm at any weekly check-in, the experiment is paused and the variant is rolled back regardless of primary metric performance. throughout the test.

## Shipping criteria
> We will **ship** if Compliance check time-on-task (target ≤ 9 min).  Time-on-task starts when the driver opens the compliance checklist screen and ends when the confirmation screen is displayed following successful submission. Incomplete sessions (abandoned before submission) are excluded from the primary metric and tracked separately as a drop-off rate secondary metric. improves by ≥ Compliance check time-on-task reduces at least 5.6min at p<0.05 (95%) and Daily active sessions on the Live Dispatch Board and Route Optimizer are monitored per arm throughout the experiment. If the variant arm shows a statistically significant decrease vs. the control arm at any weekly check-in, the experiment is paused and the variant is rolled back regardless of primary metric performance. does not reach Daily usage of the Live Dispatch Board and Route Optimizer must not fall by more than 5% after 3 weeks.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 3 weeks, no results reviewed before this date.

### Slide 9 · Launch
- **GTM:** # GTM Launch Plan, RouteLogic (B2B)

| Field | Value |
|---|---|
| Feature | One-Click Compliance Checklist |
| Goal | Engagement |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Engagement, The solution already has an existing user base but adoption is low.  The intent would be to improve adoption and get that loyalty to improve to avoid look at alternative solutions on the market.
- **Target audience:** Primary audience: Experienced drivers (existing user base) with low feature adoption and documented workaround behavior.
Secondary audience (amplifier, not recipient): Dispatch coordinators — incentivized by reduced driver escalations and workaround requests.

## Launch Tier
- **M, Targeted**, This is an existing product with an existing user base, so this is a targeted re-engagement .  The reach is the existing user base and the supporting dispatch coordinator group whom support them.  The launch needs to be beyond anything in the solution itself.  It should include emails, perhaps quick videos to capture attention, even posters in the distribution hubs to advertise the new feature and encourage feedback.
Revenue impact is retention — reducing churn risk from drivers and accounts actively evaluating alternatives. Budget for paid items (print, video production) must be confirmed and approved before week 1 begins. If budget is not confirmed by end of week 1, the paid channel plan is paused and the launch timeline is reassessed.

## Channels
1. **Owned: Email, notification in the solution for the new feature, company website updated highlighting new feature**
2. **Earned: Social mentions by seeded / identified drivers (super users), Endorsements by dispatch coordinators to mention as they work with drivers**
3. **Paid: Posters/print media in main distribution hubs with QR codes to short video**

## Enablement & Assets
Launch email, notification in the app as drivers load their routes for the day, one-pager for customers of Route Logic, posters in main distribution hubs with a short demo / highlight video highlighting the new feature.

## Ownership, Budget & Timeline
- **Ownership & budget:** PM owns the GTM plan, the success metrics and the identification and communication to super users prior to launch; Marketing team owns the email written based on PM draft input and the paid items, with paid items requiring budget;  Engineering team owns the in-solution notification and production of one-page brief draft for marketing.  Budget approvals must be obtained before feature launch and GTM timeline execution.
- **Timeline:** Week 1 and 2 - Driver and Dispatch coordinator super users communicated and with early access to feature.  Week 3 - Launch of new feature to the identified user base along with email / video demo to that targeted user base.  Communication provided on working with super users for questions.  Week 3+ - Collect feedback, capture and track metrics and decide on any iteration.
- **Metrics:** Metrics: Metric 1: Feature activation rate (week 1): % of targeted drivers who complete at least one compliance checklist submission via the new feature within 7 days of launch. Target: ≥ 40% of the identified driver cohort. If activation is below 20% at day 7, trigger a review of the in-solution notification copy and the super-user outreach response rate before proceeding. Metric 2: Compliance check time-on-task (week 3+): Average time from checklist open to confirmation screen, measured across all variant-arm drivers. Target: ≤ 9 min. Baseline: 14.6 min. Metric 3: Dispatch board weekly active sessions (retention measurement): Monitored per cohort (super-users, launched cohort, control group if available). Target: no decrease in weekly active sessions in the launched cohort vs. the 4-week pre-launch baseline. This is the leading indicator that re-engagement is holding.
Bad signal to watch for: Successful submissions of the compliance checklist - If compliance checklist submission volume is high but average time-on-task has not decreased vs. baseline by week 3, the feature is being used but not solving the moment of misery. Likely causes: drivers are completing the form but not benefiting from pre-fill (data pipeline issue) or are still navigating confirmation loops (engineering regression). Investigate before claiming adoption success.

### Slide 10 · Story
- **Friction + aha:** Friction points:  The biggest strategic challenge I faced was really sifting through all the data and deciding what was the right aspect to go after solving. Even when that was chosen, really being narrow in scope to solve just that problem and not get pulled into bleeding into solving others was critical. Keeping the persona everything was anchored to had to be in the forefront of all decisions.
The  'aha' moment: The power of defining success metrics and guardrails ahead of testing / launch. While of course testing always happens, there is so much more than just it worked or didn't work. Making adoption and value creation at the heart of the assessment of the outcome for any feature launch is critical.
- **Takeaways / next:** There were definitely insights I gained with each class! Overall how AI can assist and really help be a "neutral" assessment of each of my deliverables / plan. It really opened my eyes where I thought I was clear but actually had holes in logic or aspects that could be clarified and sharpened more. The MOSCOW approach to requirements was simple and for sure useful to apply as well as the Journey map and way of visualizing the roadmap. Really so much of the deliverables from each class's assignment taught me something.

Being new to the PM role, this course really brought me a great end-to-end viewpoint of all the components it really takes to be a PM. My eyes were definitely open to the ways to really get specific about how a product should evolve, ensuring evidence supports the changes intended, clarity and specificity of requirements, considering ahead of time how to evaluate success of the change, and most important the GTM plan - which I think is often undervalued.  I will definitely take all the elements of this course back to my existing team and PMs to begin to incorporate.

---

Submitted to the Product Management Certification learning platform · Product School.

```
