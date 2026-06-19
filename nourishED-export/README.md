# nourishED — Interactive Prototype

A clickable, single-file prototype for **nourishED**, an AI-powered K–12 digital
nutrition & wellness platform. Built as one self-contained HTML file — no build
step, no dependencies, no internet required (fonts load from Google Fonts when
online, and fall back gracefully offline).

---

## Quick start

Open `nourishED-prototype.html` in any modern web browser
(Chrome, Edge, Safari, or Firefox). Double-click the file, or drag it into a
browser tab. That's it.

To share it, send the single HTML file — everything is bundled inside.

---

## What's inside

### 1. Landing page
The entry screen: brand hero ("Empowering Students with Lifelong Wellness"),
call-to-action buttons, and three feature highlights (Adaptive Curriculum,
Real-Time Analytics, Role-Based Access).

- **Sign In** and **Get Started** → open the role-selection screen.
- **View Curriculum** → open the public curriculum overview.

### 2. Role selection
Choose one of five role experiences to explore:

| Role | What you see |
|------|--------------|
| **Student** | Dashboard, progress, and four playable learning games |
| **Teacher** | Class analytics, student progress table, lesson tracking, AI insights |
| **Parent** | Child's daily learning summary, topic mastery, weekly activity |
| **School Administrator** | School-wide stats and engagement by grade *(preview)* |
| **District Administrator** | District rollup and per-school performance *(preview)* |

### 3. Curriculum overview
A public, marketing-style page browsing lessons by grade band (K through 12).

---

## Interactive games (Student role)

All four are fully playable:

- **Food Sorting** — drag or tap foods into the correct food group.
- **Trivia Quiz** — multiple-choice nutrition questions with feedback.
- **MyPlate Builder** — assemble a balanced plate against MyPlate goals.
- **Speed Match** — 60-second timed match of foods to their benefits, with a
  motivational affirmation tailored to your score on the results screen.

---

## Navigating

- Use the in-app **Logout** button (top right) to return to the landing page.
- **Back to Home** links appear on the role-selection and curriculum screens.

---

## Notes for handoff

- **Single file.** All markup, styles, and logic live in
  `nourishED-prototype.html`. State is held in a plain JavaScript object and the
  UI re-renders on change — no framework required.
- **Brand tokens** (colors, radius, shadow, fonts) are defined as CSS custom
  properties in the `:root` block near the top of the file — a good place to
  start when adjusting the visual theme.
- **Demo data** (roles, lessons, students, quiz questions, etc.) is declared in
  the `DATA` section of the script, near the top — swap in real content there.
- Screens marked *(preview)* are inferred placeholders and are flagged in the UI;
  confirm against final designs before development.

---

*Prototype only — not production code. Intended for design review, stakeholder
walkthroughs, and developer handoff.*
