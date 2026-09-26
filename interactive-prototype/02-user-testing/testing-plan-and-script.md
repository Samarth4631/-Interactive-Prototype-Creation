# User Testing Plan & Script — FitTrack Prototype

Goal: run a short, moderated usability test on the clickable prototype to check whether the two-tier "quick log" interaction actually behaves the way the design intended (see the FitTrack design-thinking doc's proposed test plan — this is that plan, executed).

## 1. Objectives

- Confirm a first-time user can get from launch to a logged workout without hesitation.
- Confirm the "Add detail" step reads as optional, not a required field they're missing.
- Confirm the Progress tab's weekly trend is understood without explanation.
- Surface anything about the transitions/navigation that confuses rather than orients.

## 2. Participants

5 participants, mixed:
- 3 "casual exerciser" profile (matches persona Maya)
- 2 "structured/consistent exerciser" profile (matches persona Daniel)

5 is enough to surface the most common usability problems at this stage (per standard usability-testing sample-size guidance); this is a formative test, not a statistical study.

## 3. Setup

- Moderated, remote or in-person, screen-shared.
- Participant is given the prototype link and told: *"This simulates a real app. Tap anything you'd normally tap. I can't tell you where to click — just talk out loud as you go."*
- Session length: ~15 minutes per participant.
- Reset the prototype (the "Reset prototype" link) before each session so the streak count starts consistent.

## 4. Tasks & Script

**Task 1 — First impression / onboarding**
> "Open the prototype. Without me explaining anything, get to the point where you've logged your first workout."

Watch for: hesitation on the welcome screen, whether they look for a way to skip sign-up (there isn't a sign-up screen in this prototype build — note if anyone expects one).

**Task 2 — Quick log**
> "Log a second workout — try to do it as fast as you can."

Watch for: do they open "Add detail" without needing to? Do they treat it as required? Time how long it takes.

**Task 3 — Add detail**
> "Now log a third workout, but this time add some detail to it."

Watch for: is the toggle discoverable? Does the expand/collapse animation clearly show what happened?

**Task 4 — Check progress**
> "Without me telling you, find out whether you did more or less this week compared to last week."

Watch for: do they go to Progress unprompted? Do they correctly read the trend, or do they look for a number/table instead?

**Task 5 — Free exploration**
> "Take a minute and tap around anywhere else you're curious about."

Watch for: unprompted reactions to the bottom nav, the back button, profile screen, anything that breaks expectations.

## 5. Post-Task Questions

- "On a scale of 1–5, how confident are you that you actually logged something each time?"
- "Was there any point where you weren't sure what would happen if you tapped something?"
- "What would you call the button that expands the extra fields, in your own words?"

## 6. What Counts as a Finding

Only note something as a finding if it happened with **2 or more of the 5 participants**, or if a single occurrence involved the participant failing a task outright (can't recover on their own within ~20 seconds). Isolated personal preferences (e.g. "I'd want it in blue") are logged but not treated as usability issues.

Findings from running this script are recorded in [`../03-feedback-and-refinements/feedback-log.md`](../03-feedback-and-refinements/feedback-log.md).
