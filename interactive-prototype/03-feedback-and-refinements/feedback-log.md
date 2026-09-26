# Feedback Log & Refinements — FitTrack Prototype

Findings below are illustrative, written the way real notes from running [`testing-plan-and-script.md`](../02-user-testing/testing-plan-and-script.md) would look, to demonstrate how a finding turns into a specific design change. If you run the actual session, replace these with real observations.

## Findings

| # | Observation | Participants affected | Task | Severity |
|---|---|---|---|---|
| F1 | Two participants tapped directly on the streak number expecting it to open a detail/history view; nothing happened. | 2 of 5 | Task 4 | Minor |
| F2 | One participant paused on the "Add detail" toggle for several seconds, unsure if leaving it collapsed meant the workout would be "incomplete." | 1 of 5 (but failed to proceed confidently — treated as a finding per the severity rule) | Task 2 | Major |
| F3 | All 5 participants located and correctly read the weekly trend chart on the Progress tab without prompting, and used the words "up" / "down" / "better than last week" unprompted. | 5 of 5 | Task 4 | — (confirms design intent; not a problem) |
| F4 | Three participants expected the back arrow (‹) on the Log Workout screen to also appear on Progress/Profile, and looked for it briefly before finding the bottom tab bar. | 3 of 5 | Task 5 | Minor |
| F5 | The toast confirmation ("Logged! 🔥 Streak +1") was well received — 4 of 5 participants smiled or reacted positively and described it as "satisfying." | 4 of 5 | Task 2/3 | — (positive signal) |
| F6 | One structured-exerciser participant (Daniel profile) wanted the Duration field, once expanded, to remember the last value entered rather than starting empty each time. | 1 of 5 | Task 3 | Minor (noted, not actioned this round — see below) |

## Refinements Made

**From F1 →** Made the streak card visually indicate it's a static summary rather than a tappable element, by removing any hover/press affordance from it in the next prototype iteration, and confirmed with two follow-up participants that this resolved the confusion. *(Design principle: if something looks tappable, it should be — otherwise strip the affordance rather than leave it ambiguous.)*

**From F2 →** This was the most important finding, since it undermines the core "quick log is genuinely optional" premise the whole flow was built around (see the FitTrack design-thinking doc's Ideate section). Fix applied: relabeled the toggle from "+ Add detail (optional)" to "+ Add detail — skip if you're in a rush," making the optionality explicit in-line rather than relying on the word "(optional)" being noticed. Also kept the Confirm button equally prominent whether or not the toggle was opened, so nothing about the button's state implies a missing step.

**From F4 →** Not changed. Per the testing plan's finding threshold, this is a minor, quickly self-corrected issue (all 3 participants found the tab bar within a couple seconds), and the current separation — back arrow only for "drilled into" screens vs. tab bar for peer-level screens — is a standard, learnable mobile pattern. Flagged to revisit only if it recurs in a larger follow-up test.

**From F6 →** Logged as a backlog item for a future iteration rather than actioned now: remembering previous input is a data/state feature, not a layout or flow issue, and is out of scope for a prototype focused on testing navigation and information hierarchy.

## What This Round Validated

- The core need this project was designed around — N1 (fast logging) and N4 (optional depth) — holds up under testing, once the wording fix from F2 is applied.
- N2 (glanceable trend over raw data) is strongly validated by F3 and F5: people read the trend correctly and responded emotionally to the confirmation moment, without being shown any raw numbers first.

## Next Testing Round

Re-test the updated toggle copy from the F2 fix with 2–3 new participants, specifically re-running Task 2, to confirm the optionality is now unambiguous before considering this interaction finalized.
