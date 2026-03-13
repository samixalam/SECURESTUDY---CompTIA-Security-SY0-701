# 🔐 SecureStudy — CompTIA Security+ SY0-701 Practice Suite

A fully self-contained, browser-based revision tool for the **CompTIA Security+ SY0-701** exam. No installs, no accounts, no server — just open the HTML file and start studying.

---

## Why I Built This

I'm currently studying for my Security+ whilst simultaneously job-hunting in cybersecurity. I looked at my exam date, looked at the state of my revision, and decided I needed **one place** that did everything I actually wanted — not a paid subscription service, not a flashcard app, not a PDF. A proper interactive practice exam with real feedback.

So I built it. It's the tool I needed, and I'm publishing it here because if you've landed on this repo, you're probably in the same boat.

---

## What It Does

### 🎯 Practice Exam Mode
A full **90-question timed exam** designed to mirror the real SY0-701 format as closely as possible.

- Questions are drawn randomly from a pool of 150+ across all five official domains — you won't get the same paper twice
- **90-minute countdown timer** with colour warnings as time runs low
- Flag questions for review and jump between them freely using the sidebar navigator
- At the end, your raw score is converted to a **scaled score (100–900)** with a clear **PASS / FAIL verdict** — the passing threshold is 750, same as the real exam

### ⚙️ Custom Paper Mode
Build your own practice paper around your weak spots.

- Select **one or more domains** to pull questions from
- Choose how many questions you want: preset options (10, 25, 50, 75) or any custom number
- Toggle between **timed** (1 minute per question) or **untimed** mode
- The app calculates available questions from your selection in real time so you always know what you're working with

### 📊 Results & Review
After any exam you get a full breakdown:

- Percentage score and scaled score with pass/fail verdict
- Correct, incorrect, and skipped counts
- **Time taken**
- A **domain performance pie chart** — the outer ring shows domain weighting, the inner fill shows how well you scored in each one
- A full **collapsible question review** — every question, your answer, the correct answer, and a written explanation of *why*

---

## The Five SY0-701 Domains Covered

| # | Domain | Exam Weighting |
|---|--------|----------------|
| 1 | General Security Concepts | 12% |
| 2 | Threats, Vulnerabilities & Mitigations | 22% |
| 3 | Security Architecture | 18% |
| 4 | Security Operations | 28% |
| 5 | Security Program Management & Oversight | 20% |

---

## How to Use It

1. Open the following link: https://samixalam.github.io/SECURESTUDY---CompTIA-Security-SY0-701/
2. Consider bookmarking the link. Spaced repetition is great for exam prep!
3. Take the tests! 

---

## Tech Stack

| | |
|--|--|
| **Language** | Vanilla HTML, CSS, JavaScript |
| **Dependencies** | None — zero external libraries or frameworks |
| **Fonts** | Google Fonts (Space Mono + DM Sans) — loaded remotely |
| **Storage** | None — everything runs in memory, nothing is tracked or sent anywhere |

The whole thing is a single `.html` file by design. It's portable, auditable, and easy to fork or extend.

---

## Extending It

Want to add more questions? Each question in the `QUESTIONS` array follows this simple structure:

```js
{
  d: 2,                          // Domain number (1–5)
  q: "What is a zero-day?",      // Question text
  a: ["Option A", "Option B", "Option C", "Option D"],  // Answer options
  c: 1,                          // Index of correct answer (0-based)
  e: "Explanation text here."    // Shown in the review screen
}
```

Contributions of additional questions are very welcome — open a PR.

---

## Disclaimer

This project was built with the assistance of **Claude Sonnet 4.6** by Anthropic.

Not out of laziness — I'm actively studying for this exam and understand the material. I used it because I saw my exam date, needed a centralised revision tool fast, and wanted something polished enough to be genuinely useful rather than cobbled together. Claude helped me build it quickly so I could spend the rest of my time actually revising.

I'm publishing it openly because the Security+ community is full of people self-studying on tight timelines, often without the budget for paid platforms. If this saves someone a few hours or helps them pass, that's the whole point.

**Important caveats:**
- This is a study aid, not an official CompTIA resource
- Questions are written to reflect SY0-701 objectives and are not sourced from real exam dumps — using brain dumps is a violation of CompTIA's candidate agreement and defeats the purpose of the certification
- Always cross-reference with official CompTIA study materials, the [Professor Messer SY0-701 course](https://www.professormesser.com/security-plus/sy0-701/sy0-701-video/sy0-701-comptia-security-plus-course/), and the official exam objectives document

---

## Licence

MIT — do whatever you want with it. If you improve it, consider sharing it back.

---

*Good luck with the exam. You've got this.*
