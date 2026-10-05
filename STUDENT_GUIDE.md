# Washington College Mathematics Seminar: Student Slide Guide

Welcome to the **Washington College Mathematics Seminar** Quarto presentation template! 

This guide is designed for undergraduate students preparing their **Senior Capstone Experience (SCE)** or **Math Seminar** talk. Whether you are presenting pure algebra, real analysis, graph theory, applied statistics, or computational modeling, this template equips you with modern web-based slides that look stunning on any screen.

---

## 🌟 Quick Start Options

You can build, edit, and preview your presentation using any of the following methods:

### Option 1: GitHub Codespaces (Zero Setup — Recommended!)
You don't need to install Python, LaTeX, or Quarto on your personal laptop. You can edit everything inside your web browser:
1. Click the green **Code** button at the top of this repository on GitHub.
2. Select the **Codespaces** tab and click **Create codespace on main**.
3. Once the Codespace finishes loading (takes about 60–90 seconds the first time), open the terminal and run:
   ```bash
   quarto preview index.qmd
   ```
4. A live browser preview of your slides will open automatically side-by-side with your code! Every time you save `index.qmd`, the preview refreshes instantly.

---

### Option 2: Local VS Code or Positron
If you prefer working on your local machine:
1. Install [Quarto CLI](https://quarto.org/docs/get-started/) (version 1.4+).
2. Install the **Quarto extension** in VS Code or Positron.
3. Open `index.qmd` and click the **Render** / **Preview** button at the top of the editor.

---

### Option 3: Command Line / Terminal
In your terminal, navigate to this project folder:
```bash
# Live preview in your default web browser
quarto preview index.qmd

# Compile slides to the docs/ directory for publishing
quarto render index.qmd
```

---

## 📐 Structuring a 20–25 Minute Math Seminar Talk

A great math talk is not an exhaustive reading of your paper; it is an invitation to understand a beautiful mathematical idea. Aim for **12 to 18 slides total** (roughly 1.5 minutes per slide):

1. **Title & Affiliation** (1 slide): Your name, Washington College, SCE title, capstone advisor.
2. **Roadmap / Agenda** (1 slide): High-level overview so the audience never feels lost.
3. **Motivation & Intuition** (2–3 slides): Why does this question matter? Use a real example, puzzle, or geometric picture before writing formal definitions.
4. **Definitions & Notation** (2–3 slides): Keep notation lean. Define only what is strictly necessary for your main result.
5. **Main Results / Key Theorems** (2–3 slides): State your central theorem clearly using a `.thm-box`. Explain what the theorem says in plain English.
6. **Proof Sketch / Key Ideas** (2–4 slides): Don't show every line of algebraic manipulation. Highlight the *spark of genius* or key lemma that makes the proof work.
7. **Computational Visualizations or Examples** (2–3 slides): Show simulations, graphs, or concrete numerical calculations.
8. **Open Problems & Capstone Reflections** (1–2 slides): Where does the theory go next? What challenges did you tackle during your SCE?
9. **References** (1 slide): Acknowledge primary sources from `references.bib`.
10. **Q&A / Thank You** (1 slide): Contact info, link to your GitHub repo, and welcoming questions.

---

## 📝 Writing LaTeX Mathematics in Quarto

Quarto supports full LaTeX mathematics through **MathJax**.

### 1. Inline vs. Display Math
* **Inline Math:** Wrap equations in single dollar signs: `$e^{i\pi} + 1 = 0$` $\to$ $e^{i\pi} + 1 = 0$.
* **Display Math:** Wrap stand-alone equations in double dollar signs:
  ```markdown
  $$\int_{-\infty}^\infty e^{-x^2} \, dx = \sqrt{\pi}$$
  ```

### 2. Numbered Equations & Cross-References
Add `{#eq-name}` right after your display equation to automatically number it and reference it:
```markdown
$$\sum_{n=1}^\infty \frac{1}{n^s} = \prod_{p \in \mathbb{P}} \frac{1}{1 - p^{-s}} {#eq-euler}$$

As seen in @eq-euler, Euler established the prime connection...
```

### 3. Essential Math Cheat-Sheet

| Concept | LaTeX Code | Output Example |
|:---|:---|:---|
| **Number Sets** | `\mathbb{R}, \mathbb{C}, \mathbb{Z}, \mathbb{Q}, \mathbb{N}` | $\mathbb{R}, \mathbb{C}, \mathbb{Z}, \mathbb{Q}, \mathbb{N}$ |
| **Summations** | `\sum_{k=1}^n k = \frac{n(n+1)}{2}` | $\sum_{k=1}^n k = \frac{n(n+1)}{2}$ |
| **Integrals** | `\int_a^b f(x) \, dx` | $\int_a^b f(x) \, dx$ |
| **Limits** | `\lim_{x \to \infty} \frac{\sin x}{x} = 0` | $\lim_{x \to \infty} \frac{\sin x}{x} = 0$ |
| **Fractions** | `\frac{a + b}{c + d}` | $\frac{a+b}{c+d}$ |
| **Greek Letters** | `\alpha, \beta, \gamma, \delta, \lambda, \sigma, \omega` | $\alpha, \beta, \gamma, \delta, \lambda, \sigma, \omega$ |
| **Implication** | `A \implies B \iff \neg B \implies \neg A` | $A \implies B \iff \neg B \implies \neg A$ |

### 4. Multi-Line Aligned Equations
Use the `aligned` environment inside display math:
```latex
$$\begin{aligned}
(x + y)^3 &= (x + y)(x^2 + 2xy + y^2) \\
          &= x^3 + 2x^2y + xy^2 + x^2y + 2xy^2 + y^3 \\
          &= x^3 + 3x^2y + 3xy^2 + y^3
\end{aligned}$$
```

### 5. Matrices & Systems
```latex
$$A = \begin{pmatrix} 
a & b \\ 
c & d 
\end{pmatrix}, \quad 
f(x) = \begin{cases} 
x^2 & \text{if } x \ge 0, \\ 
-x & \text{if } x < 0. 
\end{cases}$$
```

---

## 🎨 Washington College Math Styling Blocks

This template includes custom styles pre-configured in `custom.scss` using Washington College colors (Maroon `#862633`, Gold `#C5A059`, and Dark Charcoal `#1E293B`).

### Theorem Box (`.thm-box`)
```markdown
::: {.thm-box}
<div class="box-title"><span class="badge badge-wc">Theorem 1</span> Bolzano-Weierstrass</div>
Every bounded sequence in $\mathbb{R}^n$ has a convergent subsequence.
:::
```

### Definition Box (`.def-box`)
```markdown
::: {.def-box}
<div class="box-title"><span class="badge badge-blue">Definition 2</span> Metric Space</div>
A metric space is an ordered pair $(M, d)$ where $M$ is a set and $d$ is a metric on $M$.
:::
```

### Lemma Box (`.lem-box`)
```markdown
::: {.lem-box}
<div class="box-title"><span class="badge badge-gold">Lemma 1.1</span> Cauchy-Schwarz Inequality</div>
For all vectors $u, v$ in an inner product space, $|\langle u, v \rangle|^2 \le \langle u, u \rangle \cdot \langle v, v \rangle$.
:::
```

### Proof Box (`.proof-box`)
```markdown
::: {.proof-box}
<div class="box-title">Proof Outline</div>
Let $\epsilon > 0$ be given. Choose $N = \lceil 1/\epsilon \rceil$...
<span class="qed">∎</span>
:::
```

### Key Takeaway Card (`.takeaway-card`)
```markdown
::: {.takeaway-card}
<div class="takeaway-title">✨ Key Intuition</div>
The zeros of the Riemann zeta function dictate the oscillatory waves in prime distribution.
:::
```

---

## 🎤 Presenter Superpowers (During Your Talk)

Quarto Reveal.js gives you powerful live tools during your seminar:

### 1. Presenter Console (<kbd>S</kbd>)
Press the <kbd>S</kbd> key on your keyboard at any point during your talk. A dual-screen presenter window opens showing:
* **Elapsed Time & Live Clock** (keeps you on time!).
* **Preview of the Next Slide** (so your transitions are seamless).
* **Speaker Notes** (private bullet points only you can see).

To add speaker notes to any slide, write:
```markdown
::: {.notes}
* Emphasize that this inequality only holds when $p > 2$.
* Pause for 5 seconds to let the audience digest the definition.
:::
```

### 2. Live Chalkboard & Pen Tool (<kbd>C</kbd>)
During questions, a professor might say: *"Can you explain the third step of that derivation?"*
* Press <kbd>C</kbd> or click the pencil icon in the bottom-left corner to toggle the **Live Chalkboard**.
* Use your mouse or trackpad to draw, circle formulas, or write equations directly on the slide.
* Press <kbd>B</kbd> to toggle a blank whiteboard.
* Press <kbd>DEL</kbd> to clear your drawings.

### 3. Slide Overview Grid (<kbd>O</kbd> or <kbd>ESC</kbd>)
Press <kbd>O</kbd> to zoom out into an interactive grid of all your slides. Click any slide to jump directly to it during Q&A!

---

## 📚 Citations & Bibliographies

1. Put your BibTeX entries into `references.bib`:
   ```bibtex
   @article{nash1950,
     author  = {Nash, John},
     title   = {Equilibrium Points in n-Person Games},
     journal = {PNAS},
     year    = {1950}
   }
   ```
2. Cite them in your slide markdown:
   * `[@nash1950]` renders as **(Nash, 1950)** or **[1]**.
   * `@nash1950 demonstrated that...` renders as **Nash (1950) demonstrated that...**
3. At the end of `index.qmd`, include the `#refs` placeholder:
   ```markdown
   ## References
   ::: {#refs}
   :::
   ```
4. **Switching Citation Styles**:
   In the YAML header of `index.qmd`:
   * Uncomment `csl: ieee.csl` for numeric brackets: `[1]`.
   * Uncomment `csl: apa.csl` for author-date: `(Nash, 1950)`.

---

## 🚀 Publishing to GitHub Pages (Automated!)

This repository includes a GitHub Actions workflow (`.github/workflows/publish.yml`) that builds and deploys your slides to the web whenever you push to GitHub!

### Step 1: Render and Push Your Changes
```bash
quarto render
git add .
git commit -m "Update math seminar slides"
git push origin main
```

### Step 2: GitHub Pages is Live!
Your personal repository set up by your instructor is already pre-configured to publish directly from the `/docs` folder on your `main` branch. 
* Whenever you run `quarto render` and push to `main`, your updated slides go live at:
  `https://washington-college.github.io/quarto-math-seminar-slides-<your-username>/`

---

## 🤝 Need Advice or Support?

* **Washington College Department of Mathematics & Computer Science**
* **Dr. Dylan Poulsen**: [Book Office Hours](https://outlook.office.com/bookwithme/user/f78874d353574c549378ea832faf2ae7@washcoll.edu?anonymous&ep=plink)
* Quarto Documentation: [quarto.org/docs/presentations/revealjs/](https://quarto.org/docs/presentations/revealjs/)
