# arabic-templates

A collection of 91 Arabic/RTL LaTeX templates organized into 10 categories.

## Description

This package provides 91 ready-to-use LaTeX templates for Arabic right-to-left typesetting. Templates cover academic, business, legal, project management, education, presentations, letters, finance, marketing, personal, and technical engineering use cases.

All templates use **XeLaTeX** with the **Amiri** font and `polyglossia`/`bidi` for full RTL support with mixed English.

## Requirements

- **Compiler:** XeLaTeX (not pdfLaTeX — required for `fontspec` and `bidi`)
- **Font:** Amiri (`Amiri-Regular.ttf`) — included in TeX Live and MiKTeX
- **Packages:** `polyglossia`, `bidi`, `fontspec`, plus standard packages (`graphicx`, `booktabs`, `tabularx`, `tcolorbox`, `tikz`, etc.)

## Usage

Each template is in its own directory under `templates/`. Compile with:

```bash
cd templates/Academic_and_Research/thesis_template
xelatex main.tex
xelatex main.tex
```

For templates with a bibliography, also run `bibtex main` between XeLaTeX runs.

## Categories

| Category | Count |
|---|---|
| Academic_and_Research | 19 |
| Business_and_Legal | 18 |
| Project_Management | 20 |
| Education_and_Personal | 10 |
| Presentations | 4 |
| Letters_and_Correspondence | 4 |
| Finance_and_Accounting | 4 |
| Marketing_and_Communications | 4 |
| Personal_and_Life | 4 |
| Technical_and_Engineering | 4 |
| **Total** | **91** |

## License

LaTeX Project Public License v1.3c (LPPL-1.3c).

## Maintainer

arabic-latex-templates contributors
