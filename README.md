# Master's Thesis: Study Of The Quantum Phase In The Framework Of The Fractional Fourier Transform

**Author:** Miguel Jafert Serrano Mantilla
**Degree:** Master studen of Applied Mathematics
**Institution:** Universidad Industrial De Santander
**Supervisor:** PhD. Rafael Ángel Torres Amaris
**Co-Supervisor:** Papá Dios  
**Academic Year:** 2025-2027

[![LaTeX](https://img.shields.io/badge/Made%20with-LaTeX-1f425f.svg)](https://www.latex-project.org/)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-b31b1b.svg)](https://arxiv.org/abs/XXXX.XXXXX) *<!-- Optional -->*

## 📘 Overview

This repository contains the complete digital source materials for my Master's thesis in Theoretical Quantum Optics and Quantum Field Theory. The work explores [brief mention of core theme, e.g., "entanglement generation in coupled cavity arrays," "the Unruh effect in analog systems," "open quantum systems approaches to decoherence"].

The repository is structured to ensure transparency, reproducibility of figures, and archival permanence for the theoretical derivations and results presented.

## 📁 Repository Structure

```
.
├── 📄 Project_Proposal.pdf                 # The formal research proposal
├── 📚 Thesis/                              # Full LaTeX source for the thesis
│   ├── main.tex                           # Main document
│   ├── preamble.tex                       # LaTeX packages & custom commands
│   ├── chapters/                          # Individual chapters
│   │   ├── 01_introduction.tex
│   │   ├── 02_background.tex
│   │   └── ...
│   ├── references.bib                     # BibTeX database
│   └── figures/                           # Compiled PDF/PNG figures (for inclusion)
│
├── 🎨 Figures_Source/                      # All editable source figures
│   ├── chapter_01/
│   │   ├── cavity_array.svg
│   │   └── level_diagram.svg
│   ├── chapter_02/
│   │   ├── penrose_diagram.svg
│   │   └── circuit_diagram.svg
│   └── ... (All .svg files created with Inkscape)
│
├── 📝 README.md                            # This file
└── .gitignore                             # Standard LaTeX and OS ignore patterns
```

## 🔬 Thesis Abstract

*A placeholder for your abstract. Typically 200-300 words summarizing the problem, theoretical framework, key findings, and implications.*

> **Example:** This thesis investigates the non-equilibrium dynamics of an impurity coupled to a structured bosonic reservoir, modeled within the framework of the spin-boson model with spectral density \( J(\omega) \sim \omega^s \). Employing a combination of analytical path-integral techniques (Leggett et al.) and numerical tensor network simulations (Time-Evolving Block Decentralization), we characterize the localization-delocalization transition for sub-Ohmic (\(s < 1\)) baths. A key result is the identification of a novel multi-time correlation structure in the localized phase, with direct implications for quantum memory applications. Furthermore, we propose an analog quantum simulation protocol for this model using trapped ions in a tailored spectral environment.

## 🛠️ Compiling the Thesis

The document is written in LaTeX and uses standard packages for physics (`physics`, `amssymb`) and mathematics (`amsmath`). For typesetting quantum mechanics, it may use `braket`.

### Prerequisites
- A full LaTeX distribution (e.g., [TeX Live](https://www.tug.org/texlive/), [MiKTeX](https://miktex.org/), or [MacTeX](https://www.tug.org/mactex/)).
- The following LaTeX packages (usually included in full distributions):
  - `amsmath`, `amssymb`, `amsthm`
  - `geometry`, `hyperref`, `graphicx`
  - `physics`, `braket`
  - `booktabs`, `siunitx`
- For bibliography management: `biblatex` (with backend `biber`) or `natbib`.

### Compilation Instructions

Using the command line in the `Thesis/` directory:

```bash
# 1. Compile LaTeX, generate bibliography, recompile (standard biblatex/biber workflow)
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex  # For resolved references

# Or use the latexmk tool (recommended for automation)
latexmk -pdf -pdflatex="pdflatex -interaction=nonstopmode" -bibtex main.tex
```

The final PDF will be generated as `Thesis/main.pdf`.

## 🎨 Figures Source

All schematic diagrams, theoretical plots (concept diagrams, not data plots), and custom illustrations are created as vector graphics using **[Inkscape](https://inkscape.org/)** and stored as `.svg` files in the `Figures_Source/` directory.

- **Why SVG?** Vector graphics are infinitely scalable, editable, and produce crisp results in the final PDF at any resolution.
- **Organization:** Figures are grouped by chapter for easy navigation.
- **Naming Convention:** Descriptive names (e.g., `keldysh_contour.svg`, `hbn_layer_structure.svg`).
- **Inclusion in LaTeX:** The compiled figures in `Thesis/figures/` are in PDF or PNG format. To re-export from source:
  1. Open `.svg` file in Inkscape.
  2. *File → Save As...* and choose "PDF" (for LaTeX with `\includegraphics`) or "PNG" (set high DPI, e.g., 300).
  3. Save to the appropriate `Thesis/figures/` subdirectory.

## 📚 Theoretical Context & Key Tools

- **Primary Theoretical Framework:** Quantum Optics, Quantum Field Theory (QFT)
- **Mathematical Tools:** Second Quantization, Green's Functions, Master Equations (Lindblad, GKSL), Path Integrals (Schwinger-Keldysh contour)
- **Concepts Explored:** [e.g., Coherence, Entanglement, Quantum Vacuum, Open Quantum Systems, Analog Models]
- **Notation:** Follows standard conventions (e.g., \(\hat{a}^\dagger\) for creation operator, \(c=\hbar=1\) natural units where applicable).

## 📄 Project Proposal

The `Project_Proposal.pdf` document contains the original research plan, including initial research questions, proposed methodology, and timeline, submitted for thesis approval.

## 🤝 How to Cite

If you wish to reference this thesis or its contents in academic work, please use the following BibTeX entry (update with your final details):

```bibtex
@mastersthesis{SerranoMantilla2024,
  author  = {Jafert Serrano, Rafael Torres },
  title   = {Study of the quantum phase in the framework of the Fractional Fourier Transform},
  school  = {Universidad Industrial De Santander},
  year    = {2026},
  month   = {December},
  type    = {Master's Thesis},
  url     = {https://github.com/GoofyCorleone/Tesis},
  note    = {Available at: \url{https://github.com/GoofyCorleone/Tesis}}
}
```

## 📜 License

- **Thesis Text & Original Figures (`Thesis/`, `Figures_Source/`):** Licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).
- **Project Proposal (`Project_Proposal.pdf`):** All rights reserved. Provided for reference only.

This license allows for sharing and adaptation of the theoretical work for non-commercial purposes, provided appropriate credit is given and any derivative works are shared under the same license.

## 🙏 Acknowledgments

I extend my sincere gratitude to my supervisor, [Supervisor's Name], for their profound guidance through the conceptual depths of quantum theory. I also thank [Other Professors, Collaborators] for insightful discussions. This work was supported by [Funding Body, if applicable, e.g., the University's Graduate Scholarship].

---

*This repository represents the culmination of my Master's research. For any questions regarding the theoretical content, please contact me at [your.email@domain.com].*
