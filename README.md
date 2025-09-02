# 🎵 Italian Rhythm & Word Stress — Interactive Lesson + Quiz

An all-in-one **HTML page** for English speakers learning Italian prosody.  
Based on a lesson about why Italian sounds “musical,” this mini-app teaches and drills:

- **Golden rule:** stress the **penultimate** syllable
- **Predictable exceptions:** antepenultimate stress (e.g., _tèlefono_, _góndola_, _párlano_)
- **Accent marks & meaning:** final stress (_caffè, perché, università, ventitré_) and pairs like **è/e**, **sì/si**
- **Clitics → long words:** commands with attached pronouns (e.g., _manda_ → _mandamelo_) where **stress stays on the verb**

> No frameworks, no build step — just open the file.

---

## 🚀 Quick Start

1. **Clone / Download** this repo.
2. Open **`italian_stress_rhythm_quiz.html`** in your browser.

That’s it. The page is self-contained (HTML + CSS + JS).

---

## 🧠 What’s Inside

- **Tabbed lesson flow**: Golden Rule → Exceptions → Accent Marks → Clitics → Mixed Quiz  
- **Interactive tasks**:
  - Click the **stressed syllable** (syllable tiles)
  - **Drag & drop** words into stress categories
  - **Accent keypad** for typing _à è é ì ò ù_
  - Mini-quizzes on **accent = meaning** (è/e, sì/si)
  - Build clitic “super-words” (e.g., _mandamelo_) and mark stress
  - Mixed MCQs + short answers
- **Instant scoring** with a global progress bar
- **Export results** as `italian_stress_results.json` (for learners/teachers)

---

## 🛠 Customize

Open `italian_stress_rhythm_quiz.html` and edit the data arrays in the `<script>`:
- Add words to **P1_WORDS** (syllables + stressed index)
- Add exceptions in **P2_BANK** (assign to `penult`, `antepenult`, or `final`)
- Add accent items in **P3_FILL** and **P3_MC**
- Extend clitic examples in `chunkSyllables(...)` map
- Expand mixed quiz via **P5_MC**

Everything is in plain JavaScript; no tooling required.

---

## 🌐 Publish on GitHub Pages

### Option A — Rename file (recommended)
1. Rename **`italian_stress_rhythm_quiz.html`** to **`index.html`**.
2. Push to the **`main`** branch.
3. In your repo: **Settings → Pages → Build and deployment**
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` / `/root`
4. Your quiz will be live at:
