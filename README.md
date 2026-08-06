<div align="center">

# arabic-latex-templates

A collection of **91 Arabic/RTL LaTeX templates** across 10 categories â€” academic, business, legal, project management, finance, presentations, letters, marketing, personal, and technical engineering.

[![License: LPPL-1.3c](https://img.shields.io/badge/license-LPPL--1.3c-blue.svg)](https://www.latex-project.org/lppl/)
[![Templates](https://img.shields.io/badge/templates-91-brightgreen.svg)](#categories)
[![Compiler](https://img.shields.io/badge/compiler-XeLaTeX-orange.svg)](https://www.latex-project.org/)
[![Font](https://img.shields.io/badge/font-Amiri-red.svg)](https://www.amirifont.org/)
[![RTL](https://img.shields.io/badge/RTL-Arabic-success.svg)](#)
[![DOI](https://img.shields.io/badge/DOI-Zenodo-blueviolet.svg)](https://doi.org/10.5281/zenodo.YOUR_ZENODO_ID)
[![Open in Overleaf](https://img.shields.io/badge/Open%20in-Overleaf-47A141.svg)](https://www.overleaf.com)

![LaTeX](https://img.shields.io/badge/LaTeX-008080?logo=latex&logoColor=white)
![GitHub stars](https://img.shields.io/github/stars/NibrasAz7/arabic-latex-templates?style=social)
![GitHub forks](https://img.shields.io/github/forks/NibrasAz7/arabic-latex-templates?style=social)
![GitHub issues](https://img.shields.io/github/issues/NibrasAz7/arabic-latex-templates)

</div>

---

## Preview

A compiled PDF preview of each template is included in its folder (`main.pdf`). You can also browse all previews by cloning the repo and opening any `main.pdf`.

> **Tip:** Click any template folder above to view its `main.pdf` directly on GitHub.

---

## Categories

| # | Category | Count | Highlights |
|---|---|---|---|
| 1 | [`Academic_and_Research`](../../tree/main/Academic_and_Research) | 19 | Article, book, thesis, conference paper, posters, lab report/notebook, grant/research proposal, preprint, manuscript submission, response to reviewers, book chapter, dissertation defense (Beamer), Quran/Hadith |
| 2 | [`Business_and_Legal`](../../tree/main/Business_and_Legal) | 18 | Incorporation, business plan, cap table, agreements (partnership/shareholder/founders/operating/contractor/employment/service/non-compete), NDA, IP assignment, pitch deck, stock options, TOS, privacy policy, financial model |
| 3 | [`Project_Management`](../../tree/main/Project_Management) | 20 | Charter, WBS, Gantt, CPM, RACI, Kanban, risk register, issue log, status report, change request, lessons learned, communication plan, meeting minutes/agenda, decision log, milestone tracker, budget tracker, stakeholder register, procurement plan, kickoff document |
| 4 | [`Education_and_Personal`](../../tree/main/Education_and_Personal) | 10 | CV, resume, exam, syllabus, cheatsheet, technical report, homework assignment, lecture notes, flashcards, certificate |
| 5 | [`Presentations`](../../tree/main/Presentations) | 4 | Conference talk, lecture slides, sales pitch, webinar (all Beamer 16:9) |
| 6 | [`Letters_and_Correspondence`](../../tree/main/Letters_and_Correspondence) | 4 | Cover letter, recommendation letter, business letter, thank-you letter |
| 7 | [`Finance_and_Accounting`](../../tree/main/Finance_and_Accounting) | 4 | Invoice, quotation/offer, receipt, financial statement |
| 8 | [`Marketing_and_Communications`](../../tree/main/Marketing_and_Communications) | 4 | Press release, brochure, newsletter, one-pager |
| 9 | [`Personal_and_Life`](../../tree/main/Personal_and_Life) | 4 | Wedding invitation, recipe book, calendar, weekly planner |
| 10 | [`Technical_and_Engineering`](../../tree/main/Technical_and_Engineering) | 4 | Technical spec, API reference, datasheet, schematic sheet |
| | **Total** | **91** | |

---

## Quick Start

### Option 1: Open in Overleaf (no install needed)

Overleaf lets you import a template directly from this GitHub repo:

1. Go to [overleaf.com](https://www.overleaf.com) â†’ **New Project** â†’ **Import from GitHub**
2. Connect your GitHub account and select `arabic-latex-templates`
3. Choose any template folder â€” it opens as an editable project

Or use the **one-click API links** in [`sharing/overleaf/links.md`](sharing/overleaf/links.md) (available after the first GitHub Release with ZIP assets).

### Option 2: Clone and compile locally

```bash
git clone https://github.com/NibrasAz7/arabic-latex-templates.git
cd arabic-latex-templates/Academic_and_Research/thesis_template
xelatex main.tex
xelatex main.tex   # run twice for TOC/refs
```

**Requirements:** XeLaTeX (TeX Live or MiKTeX) with `amiri`, `polyglossia`, `bidi`, `fontspec` packages. The Amiri font must be installed or available to fontspec.

### Option 3: Download a single template

GitHub lets you download any folder:
1. Navigate to the template folder on GitHub
2. Click **Download ZIP** (or use `git sparse-checkout` for specific folders)

Or download a **Release bundle** â€” each GitHub Release includes per-template ZIPs as assets. See the [Releases page](../../releases).

---

## Template Structure

Each template folder contains:
```
<template_name>_template/
â”œâ”€â”€ main.tex          # XeLaTeX source (start here)
â”œâ”€â”€ main.pdf          # Compiled preview
â””â”€â”€ bibliography.bib  # (only for templates with citations)
```

Every `main.tex` starts with `% !TEX program = xelatex` and includes a header comment block with compile instructions and feature list. Placeholder text is marked with `% TODO:` comments.

---

## Compile Commands

| Template type | Command |
|---|---|
| Most templates | `xelatex main.tex` (run twice) |
| Templates with bibliography | `xelatex main.tex` â†’ `bibtex main` â†’ `xelatex main.tex` â†’ `xelatex main.tex` |
| Beamer presentations | `xelatex main.tex` (run twice) |

---

## Tech Stack

| Component | Value |
|---|---|
| Compiler | XeLaTeX |
| Font | Amiri (`Amiri-Regular.ttf`) |
| Arabic/RTL | `polyglossia` + `bidi` |
| English font | TeX Gyre Termes |
| Document class | `article` (most), `beamer` (presentations) |
| Key packages | `graphicx`, `booktabs`, `tabularx`, `tcolorbox`, `tikz`, `fancyhdr`, `titlesec`, `enumitem`, `hyperref` |

---

## Distribution Channels

| Channel | Status | How to use |
|---|---|---|
| **GitHub** | This repo | Clone, download, or fork |
| **Overleaf** | [`sharing/overleaf/`](sharing/overleaf/) | Import from GitHub or one-click API links |
| **Zenodo (DOI)** | [`sharing/zenodo/`](sharing/zenodo/) | Auto-connected to GitHub Releases â€” each release gets a permanent DOI |
| **CTAN** | [`sharing/ctan/`](sharing/ctan/) | Submit `arabic-templates.zip` to ctan.org for `tlmgr install` distribution |

---

## Citing

If you use these templates in academic work, please cite:

```bibtex
@software{arabic_latex_templates,
  author       = {{arabic-latex-templates contributors}},
  title        = {arabic-latex-templates: 91 Arabic/RTL LaTeX templates},
  year         = 2026,
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.YOUR_ZENODO_ID},
  url          = {https://doi.org/10.5281/zenodo.YOUR_ZENODO_ID}
}
```

Or click the **"Cite this repository"** button on GitHub (powered by `CITATION.cff`).

---

## Contributing

Contributions are welcome â€” new templates, fixes, or improvements. Please ensure any new template:

1. Compiles cleanly with `xelatex main.tex` (run twice)
2. Follows the existing Arabic/RTL stack (XeLaTeX + Amiri + polyglossia + bidi)
3. Includes a compiled `main.pdf`
4. Uses generic placeholder branding (no specific organization names)

---

## License

LaTeX Project Public License v1.3c (LPPL-1.3c) â€” see [LICENSE](LICENSE).

---

<div align="center">

**[Report Bug](../../issues)** Â· **[Request Template](../../issues/new?labels=template-request&template=template-request.md)** Â· **[Overleaf Links](sharing/overleaf/links.md)**

</div>
