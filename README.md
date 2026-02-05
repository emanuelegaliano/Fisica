![Course Logo](logo.png)

# Fisica (Physics) — Course Notes

This repository contains **personal university notes in Physics**, written in **LaTeX** and organized as a structured set of course chapters.
The notes were created for study and revision purposes during a university-level Physics course and are **not official lecture notes**, but a personal re-elaboration of the material.

All of the content (text, figures, comments) is written in **Italian**.

---

## Repository overview

The repository is centered around a single LaTeX project that compiles into a complete set of Physics notes, including figures, boxed formulas, and an indexed list of equations.

```
.
├── fisica.tex           # Main LaTeX entrypoint
├── references.bib       # Bibliography (biblatex + biber)
├── chapters/            # One LaTeX file per chapter
├── frontmatter/         # Preface, license page, metadata
├── images/              # Figures used throughout the notes
└── README.md
```

---

## `chapters/` — Course notes

Each chapter is written as a standalone LaTeX file and included in `fisica.tex`.

Current topics include:

* **Kinematics**
* **Dynamics**
* **Thermodynamics**
* **Waves**
* **Quantum Mechanics**

The structure is designed to be modular and easily extendable with additional chapters or appendices.

---

## Compiled PDF

After compilation, the full document is available as:

* `out/fisica.pdf`

The PDF includes:

* A custom-designed cover page
* Table of contents
* Numbered and boxed equations
* An index of equations
* Figures and explanatory text

---

## Build instructions

### Requirements

* A LaTeX distribution (TeX Live or MiKTeX)
* `latexmk`
* `biber` (used by `biblatex`)

### Compile the notes

From the repository root:

```bash
latexmk -pdf -shell-escape -interaction=nonstopmode -synctex=1 -output-directory=out fisica.tex
```

### Clean build files

```bash
latexmk -c -output-directory=out
```

---

## Notes on usage

* All figures are stored in `images/` and referenced throughout the chapters.
* On the first compilation, some cross-references may appear as undefined; a second LaTeX/Biber run resolves them automatically.
* The notes reflect the author’s understanding and organization of the material and may differ in style or emphasis from official lecture notes.

## Contribute

Contributions are welcome and appreciated 🙂

Since these notes are a personal re-elaboration of the course material, **issues and pull requests are encouraged**, especially for:

* Typographical errors or LaTeX issues  
* Incorrect or unclear explanations  
* Improvements to figures or diagrams  
* Minor clarifications or additional comments  
* Consistency fixes (notation, formatting, references)

### Issues

If you find an error, ambiguity, or have a suggestion:

1. Open a **GitHub Issue**
2. Clearly describe:
   * the chapter and section involved,
   * the problem or suggestion,
   * (optionally) a proposed fix.

This helps keep track of improvements and discussions in a structured way.

### Pull Requests

Pull requests are welcome for small, well-scoped changes.

Guidelines:
* Keep changes focused and relevant to the notes.
* Follow the existing LaTeX structure and style.
* Make sure the document still compiles correctly.
* If possible, reference the related issue in the PR description.

By contributing, you agree that your changes will be released under the same license as the rest of the project.

---

## License & disclaimer

These notes are **personal study notes** created for educational purposes.
They are **not endorsed by any university or instructor**.
