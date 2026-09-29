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
> I believe that One-Click Compliance Checklist for The Experienced Driver Who Has Given Up Trusting It will result in Manual workarounds are reduced, the workflow steps - especially compliance checks - reduce in time and drop off rates to improve.  This will be measured by a Compliance check time-on-task reducing at least 5.6min change in Compliance check time-on-task (target ≤ 9 min). Time-on-task starts when the driver opens the compliance checklist screen and ends when the confirmation screen is displayed following successful submission. Incomplete sessions (abandoned before submission) are excluded from the primary metric and tracked separately as a drop-off rate secondary metric, within 3 weeks. We will protect Daily active sessions on the Live Dispatch Board and Route Optimizer are monitored per arm throughout the experiment. If the variant arm shows a statistically significant decrease vs. the control arm at any weekly check-in, the experiment is paused and the variant is rolled back regardless of primary metric performance throughout the test.

## Shipping criteria
> We will **ship** if Compliance check time-on-task by ≥ 5.6min at p<0.05 (95%) and Daily active sessions on the Live Dispatch Board and Route Optimizer are monitored per arm throughout the experiment. If the variant arm shows a statistically significant decrease vs. the control arm at any weekly check-in, the experiment is paused and the variant is rolled back regardless of primary metric performance. The Daily usage of the Live Dispatch Board and Route Optimizer must not fall by more than 5% after 3 weeks. 
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 3 weeks, no results reviewed before this date.

## Debrief
> Hardest parameter to define, and did it change your hypothesis? Primary success metric was initially thought to be clear, actually was not.  This had to be refined and also better clarified and separated from the guardrail metric.  Testing the experiment hypothesis a few times and making iterative improvements was eye-opening in being more crisp and clear on the goals of the change and what really defines success.
