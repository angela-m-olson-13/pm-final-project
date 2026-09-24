# Feature Roadmap, Module 4 · RouteLogic Velocity

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


## Wireframes / prototype
[RouteLogic Velocity — Initiative Roadmap.pdf](https://github.com/user-attachments/files/32605642/RouteLogic.Velocity.Initiative.Roadmap.pdf)

- Link:  routelogic-velocity-roadmap.html
