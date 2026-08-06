# CTAN Package Distribution

[CTAN](https://ctan.org) (Comprehensive TeX Archive Network) is the central repository for LaTeX packages. Submitting here makes your templates installable via `tlmgr install` (TeX Live) and the MiKTeX package manager — reaching every LaTeX user in the world.

## Important: CTAN expects a *package*, not a folder of templates

CTAN distributes LaTeX **packages** (`.sty`/`.cls` files + documentation). A folder of 91 standalone templates is not a standard CTAN submission. To publish on CTAN, you need to restructure into a coherent package.

## Two approaches

### Approach A: Single class file + sample documents (recommended)

Create one document class `arabic-templates.cls` that encapsulates the shared Arabic/RTL preamble (XeLaTeX + Amiri + polyglossia + bidi + common packages), then ship each template as a sample document that uses `\documentclass{arabic-templates}`.

**Package structure:**
```
arabic-templates/
├── arabic-templates.cls       # Shared class (the "package")
├── arabic-templates.tex       # Documentation (compiled to PDF)
├── arabic-templates.pdf       # Compiled documentation
├── README.md                  # Package description
├── LICENSE                    # LPPL-1.3c
├── samples/                   # Sample documents (one per template)
│   ├── thesis.tex
│   ├── invoice.tex
│   ├── cv.tex
│   └── ... (91 samples)
└── examples/                  # Compiled sample PDFs (optional)
    ├── thesis.pdf
    └── ...
```

**Pros:** Clean, standard CTAN layout, one install gives users everything
**Cons:** Requires writing a `.cls` file and refactoring all 91 templates to use it (significant work)

### Approach B: Template bundle (simpler, less standard)

Ship the templates as-is in a single archive with a README. CTAN does accept "template collections" though they're less common.

**Package structure:**
```
arabic-templates/
├── README.md                  # Description + usage
├── LICENSE                    # LPPL-1.3c
├── arabic-templates.tex       # Brief documentation
├── arabic-templates.pdf       # Compiled documentation
└── templates/                 # All 91 templates
    ├── Academic_and_Research/
    │   └── thesis_template/
    │       └── main.tex
    └── ... (all categories)
```

**Pros:** Minimal restructuring — your current layout works
**Cons:** Less idiomatic for CTAN; users can't `tlmgr install` individual templates

## Submission steps

### 1. Prepare the package

This folder (`sharing/ctan/arabic-templates/`) contains a starter structure for Approach B. Adjust as needed.

### 2. Write the documentation

The file `arabic-templates.tex` is a minimal documentation file. Compile it:
```bash
xelatex arabic-templates.tex
```
This produces `arabic-templates.pdf`, which CTAN requires.

### 3. Create the archive

CTAN requires a ZIP or `.tar.gz` with a top-level directory:
```bash
cd sharing/ctan
zip -r arabic-templates.zip arabic-templates/
```

The archive must have this structure:
```
arabic-templates.zip
└── arabic-templates/        # top-level dir = package name
    ├── README.md
    ├── LICENSE
    ├── arabic-templates.tex
    ├── arabic-templates.pdf
    └── templates/
```

### 4. Upload

1. Go to https://ctan.org/upload
2. Fill in:
   - **Package name:** `arabic-templates`
   - **Version:** 1.0.0
   - **Author:** Your name
   - **Email:** Your email (use the same email for all future updates)
   - **License:** LPPL-1.3c
   - **Summary:** "91 Arabic/RTL LaTeX templates across 10 categories"
   - **Notes:** Mention XeLaTeX requirement, Amiri font dependency
3. Upload the ZIP
4. CTAN team reviews (usually within a few days)

### 5. After acceptance

- Your package appears at `https://ctan.org/pkg/arabic-templates`
- TeX Live includes it in the next update cycle
- Users install with: `tlmgr install arabic-templates`
- MiKTeX users: install via MiKTeX Package Manager

## Requirements checklist

- [ ] Top-level directory in archive matches package name
- [ ] `README.md` with description, license, dependencies
- [ ] `LICENSE` file (LPPL-1.3c)
- [ ] Documentation `.tex` + compiled `.pdf`
- [ ] No derived files (no `.aux`, `.log`, etc. — only source + PDF)
- [ ] File names use only printable ASCII (no spaces)
- [ ] Archive is `.zip`, `.tgz`, or `.tar.gz`

## Reference

- [How to upload to CTAN](https://ctan.org/help/upload-pkg)
- [CTAN upload form](https://ctan.org/upload)
- [CTAN upload addendum](https://www.ctan.org/file/help/ctan/CTAN-upload-addendum)
- [ctanify tool](https://www.ctan.org/tex-archive/support/ctanify) — prepares packages for CTAN
