# Washington College Math Seminar — Quarto Slides Template

A modern, web-based presentation template designed for undergraduate students at **Washington College** preparing their **Senior Capstone Experience (SCE)** or **Mathematics Seminar** talks.

[![Use This Template](https://img.shields.io/badge/Template-Use_This_Template-862633?style=for-the-badge&logo=github)](https://github.com/Washington-College/quarto-math-seminar-slides/generate)
[![Open in GitHub Codespaces](https://img.shields.io/badge/Codespaces-Open_in_Cloud-blue?style=for-the-badge&logo=github)](https://codespaces.new/Washington-College/quarto-math-seminar-slides)
[![Quarto](https://img.shields.io/badge/Built_With-Quarto_Reveal.js-007acc?style=for-the-badge&logo=quarto)](https://quarto.org)

---

## 🎯 Features

* 🏛️ **Washington College Aesthetic**: Custom styling matching official Washington College maroon (`#862633`) and gold accents.
* 📐 **Math First**: Built-in styling for **Theorems**, **Definitions**, **Lemmas**, **Proofs** (with QED $\blacksquare$), and **Key Takeaways**.
* ⚡ **Zero-Install Cloud Editing**: Full GitHub Codespaces support with Quarto, Python, and LaTeX pre-installed.
* 🎙️ **Presenter Console**: Press <kbd>S</kbd> to unlock a synchronized dual-screen presenter view with live timer, preview, and private speaker notes.
* ✏️ **Interactive Chalkboard**: Press <kbd>C</kbd> or click the pen icon to write or draw derivations live during your talk.
* 🌐 **Automated GitHub Pages Publishing**: Push your changes to `main` and GitHub Actions automatically renders and hosts your slide deck online.
* 📚 **Citation Ready**: Integrated BibTeX bibliography (`references.bib`) with 1-click toggling between APA and IEEE styles.

---

## 🚀 60-Second Quick Start

### 1. Create Your Presentation
Click the green **[Use this template](https://github.com/Washington-College/quarto-math-seminar-slides/generate)** button at the top of this repository (or click the badge above) to create your own copy.

### 2. Launch GitHub Codespaces
Click **Code** $\to$ **Codespaces** $\to$ **Create codespace on main**. No local installation required!

### 3. Preview Live
In the terminal, run:
```bash
quarto preview index.qmd
```
Your presentation will open in the preview pane. Edits in `index.qmd` reload automatically on save!

### 4. Publish to the Web
Commit and push your work:
```bash
git add .
git commit -m "Update my math seminar slides"
git push origin main
```
In your GitHub repository, go to **Settings** $\to$ **Pages** $\to$ choose **GitHub Actions** under *Source*. Your slides are now live on the internet!

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
| [`.devcontainer/`](.devcontainer/) | Codespace definition pre-configured with Quarto, Python, and extensions. |
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
* How to add computational plots with Python or R
* How to present effectively on seminar day

👉 **Read the full [STUDENT_GUIDE.md](STUDENT_GUIDE.md)**

---

## 🆘 Questions & Faculty Support

* **Washington College Department of Mathematics & Computer Science**
* **Dr. Shaun Poulsen**: [Schedule Office Hours](https://outlook.office.com/bookwithme/user/f78874d353574c549378ea832faf2ae7@washcoll.edu?anonymous&ep=plink)
