# Washington College Math Seminar — Quarto Slides Template

A modern, web-based presentation template designed for undergraduate students at **Washington College** preparing their **Senior Capstone Experience (SCE)** or **Mathematics Seminar** talks.

[![Washington College](https://img.shields.io/badge/Washington_College-Math_Seminar-862633?style=for-the-badge)](https://www.washcoll.edu)
[![Open in GitHub Codespaces](https://img.shields.io/badge/Codespaces-Open_in_Cloud-blue?style=for-the-badge&logo=github)](https://codespaces.new/Washington-College/quarto-math-seminar-slides)
[![Quarto](https://img.shields.io/badge/Built_With-Quarto_Reveal.js-007acc?style=for-the-badge&logo=quarto)](https://quarto.org)

---

## 🎯 Features

* 🏛️ **Washington College Aesthetic**: Custom styling matching official Washington College maroon (`#862633`) and gold accents.
* 📐 **Math First**: Built-in styling for **Theorems**, **Definitions**, **Lemmas**, **Proofs** (with QED $\blacksquare$), and **Key Takeaways**.
* ⚡ **Fast Zero-Install Cloud Editing**: Lightweight GitHub Codespaces setup with Quarto pre-installed in seconds.
* 🎙️ **Presenter Console**: Press <kbd>S</kbd> to unlock a synchronized dual-screen presenter view with live timer, preview, and private speaker notes.
* ✏️ **Interactive Chalkboard**: Press <kbd>C</kbd> or click the pen icon to write or draw derivations live during your talk.
* 🌐 **Automated GitHub Pages Publishing**: Push your changes to `main` and your slides update online automatically.
* 📚 **Citation Ready**: Integrated BibTeX bibliography (`references.bib`) with 1-click toggling between APA and IEEE styles.

---

## 🚀 60-Second Quick Start

### 1. Open Your Personal Repository
Your instructor will create your personal seminar repository for you under the Washington College organization (`Washington-College/quarto-math-seminar-slides-<your-username>`). Open that repository on GitHub to get started.

### 2. Launch GitHub Codespaces (Zero Setup)
Click the green **Code** button $\to$ **Codespaces** $\to$ **Create codespace on main**. No local installation required!

### 3. Edit & Preview Live
In the terminal, run:
```bash
quarto preview index.qmd
```
Your presentation will open in the preview pane. Any edits you make in `index.qmd` reload automatically on save!

### 4. Publish to the Web
Render your slides and push your changes:
```bash
quarto render
git add .
git commit -m "Update my math seminar slides"
git push origin main
```
GitHub Pages is pre-configured to serve directly from the `/docs` folder on `main`. Your updated slides go live automatically within seconds at:
`https://washington-college.github.io/<your-repo-name>/`

---

## 📁 Repository Overview

| File / Folder | Purpose |
|:---|:---|
| [`index.qmd`](index.qmd) | **Your main slide deck**. Contains a complete sample talk (Prime Number Theorem & Riemann Zeta Function) illustrating every formatting feature. |
| [`STUDENT_GUIDE.md`](STUDENT_GUIDE.md) | **Comprehensive Student Guide**. Detailed instructions on slide structure, LaTeX formulas, presenter shortcuts, and talk delivery advice. |
| [`_quarto.yml`](_quarto.yml) | Reveal.js configuration (aspect ratio, transitions, chalkboard, and output directory). |
| [`custom.scss`](custom.scss) | Washington College theme, custom theorem/definition callout boxes, typography, and badges. |
| [`references.bib`](references.bib) | BibTeX bibliography containing classic math literature and sample annotations. |
| [`apa.csl`](apa.csl) / [`ieee.csl`](ieee.csl) | Citation style files for switching between author-date and numeric references. |
| [`.devcontainer/`](.devcontainer/) | Lean Codespace definition pre-configured with Quarto and auto-preview. |
| [`.github/workflows/`](.github/workflows/) | GitHub Actions workflow for automatic deployment to GitHub Pages. |

---

## ⌨️ Presentation Day Hotkeys

| Key | Function |
|:---:|:---|
| <kbd>S</kbd> | Open **Presenter Console** (timer, upcoming slide, and notes) |
| <kbd>F</kbd> | Toggle **Fullscreen** mode |
| <kbd>C</kbd> | Toggle **Live Chalkboard** pen tool |
| <kbd>B</kbd> or <kbd>.</kbd> | **Blank screen** (whiteboard / blackout) |
| <kbd>O</kbd> / <kbd>ESC</kbd> | Slide **Overview Grid** |
| <kbd>?</kbd> | Reveal.js keyboard shortcuts cheat sheet |

---

## 📖 In-Depth Student Guide

For detailed explanations of:
* How to structure a 20–25 minute capstone talk
* LaTeX equation writing (matrices, piece-wise, summations, integrals)
* How to structure theorems, lemmas, definitions, and proof sketches
* How to present effectively on seminar day

👉 **Read the full [STUDENT_GUIDE.md](STUDENT_GUIDE.md)**

---

## 🆘 Questions & Faculty Support

* **Washington College Department of Mathematics & Computer Science**
* **Dr. Dylan Poulsen**: [Schedule Office Hours](https://outlook.office.com/bookwithme/user/f78874d353574c549378ea832faf2ae7@washcoll.edu?anonymous&ep=plink)
