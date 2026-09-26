# 🔗 Interactive Prototype Creation — FitTrack

**Turning the FitTrack low-fidelity wireframes into a clickable, navigable prototype — then testing it on real users and documenting what changed as a result.**

> Task type: UX Prototyping exercise
> Builds on: the wireframes and user flows from the *Mobile App Wireframing* project (same FitTrack case study)

---

## 🎯 The Brief

Build a clickable prototype that simulates real app interactions:

1. Convert wireframes into an interactive prototype
2. Add animations, transitions, and navigation flows
3. Conduct quick user testing on the prototype
4. Gather feedback and refine the design

## 📂 Repository Structure

```
interactive-prototype/
├── README.md
├── 01-prototype/
│   └── fittrack-prototype.html        ← the clickable prototype (open in any browser)
├── 02-user-testing/
│   └── testing-plan-and-script.md     ← moderated test plan, tasks, and script
└── 03-feedback-and-refinements/
    └── feedback-log.md                ← findings from testing + the resulting design changes
```

## 🖱️ Using the Prototype

`fittrack-prototype.html` is a single self-contained file simulating a phone screen in the browser. It is genuinely clickable, not a static image:

- **Get Started** → skip sign-in → lands on the Home dashboard
- **+ Log Workout** → pick an activity → optionally expand **Add detail** → **Confirm** → slides back to Home with the streak counter incremented (this loop is the app's core interaction, and the one tested in the user-testing session)
- Bottom tab bar switches between **Home / Progress / Profile** with a fade transition
- A **‹ Back** control appears wherever a screen was reached by drilling in, not by tab

This mirrors what you'd build by wiring up frames in Figma/InVision — the same screens from the wireframes, now connected by real navigation, transitions, and one piece of simulated state (the streak count).

## 🧭 How to Read This Repo

| Stage | File | What it answers |
|---|---|---|
| 1. Build | [`01-prototype/fittrack-prototype.html`](01-prototype/fittrack-prototype.html) | Do the wireframes actually connect into a usable flow? |
| 2. Test | [`02-user-testing/testing-plan-and-script.md`](02-user-testing/testing-plan-and-script.md) | What should we watch for, and how do we run the session? |
| 3. Refine | [`03-feedback-and-refinements/feedback-log.md`](03-feedback-and-refinements/feedback-log.md) | What did testing surface, and what did we change because of it? |

## ✅ Expected Outcome

By the end of this repo you should be able to see, end to end:
- How static wireframes become a testable, tap-through prototype
- Why animations/transitions matter even at low fidelity (they signal hierarchy: a slide = "going deeper," a fade = "moving sideways" between peer tabs)
- How to structure a short usability test so it produces specific, actionable findings rather than vague impressions
- How a design changes in response to real feedback, with each change traceable to an observation

## 📄 License

Provided as an educational template — free to reuse and adapt for coursework, portfolios, or your own case studies.
