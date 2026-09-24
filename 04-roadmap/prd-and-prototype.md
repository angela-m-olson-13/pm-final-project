# PRD & Prototype Sprint (Module 4)

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
- **My prototype, as a link or a screenshot (publish or share from your tool; in Lovable that is Share → Share Preview, in Bolt Publish → Web. No share URL? Screenshot the working flow):**
-      Prototype created using Claude.   Link (also found in repo):  routelogic-compliance-prototype.html

