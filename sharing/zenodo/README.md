# Zenodo DOI Integration (auto-connected to GitHub)

[Zenodo](https://zenodo.org) is an open-access repository hosted by CERN that assigns permanent Digital Object Identifiers (DOIs) to research outputs — including software and templates.

## The key point: Zenodo connects directly to GitHub

You do **not** manually upload anything to Zenodo. Instead:

1. You connect your GitHub account to Zenodo (one-time, 2 minutes)
2. Every time you publish a **GitHub Release**, Zenodo automatically:
   - Archives the release
   - Mints a permanent DOI
   - Creates a citable record with BibTeX/APA/EndNote export
3. You get **two DOIs** per release:
   - **Concept DOI** — always points to the latest version (use this in citations)
   - **Version DOI** — points to this specific release

No manual uploads. No maintenance. It just works.

## Why use Zenodo?

- **Permanent DOI** — even if GitHub disappears, the DOI resolves
- **Citable** — users can cite your templates in papers with a proper BibTeX entry
- **ORCID-linked** — your author profile gets credited
- **Free** — hosted by CERN
- **Automatic** — zero ongoing effort after the one-time setup

## Setup (one-time, ~5 minutes)

### Step 1: Create a Zenodo account
1. Go to https://zenodo.org
2. Sign in with ORCID (recommended) or GitHub

### Step 2: Connect GitHub to Zenodo
1. Go to https://zenodo.org/account/settings/github/
2. Click **"Connect"** and authorize Zenodo to access your GitHub
3. You'll see a list of your repos — toggle **ON** the `arabic-latex-templates` repo

### Step 3: Publish your first GitHub Release
```bash
git tag v1.0.0
git push origin v1.0.0
```
Or use the GitHub web UI: **Releases** → **Draft a new release** → tag `v1.0.0` → publish.

### Step 4: Get your DOI
1. After publishing the release, Zenodo automatically creates a record (within minutes)
2. Go to https://zenodo.org/account/settings/github/ to see your DOI
3. The DOI looks like `10.5281/zenodo.12345678`

### Step 5: Add DOI badge to README
Add this to the main `README.md` (replace the placeholder):
```markdown
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.YOUR_ZENODO_ID.svg)](https://doi.org/10.5281/zenodo.YOUR_ZENODO_ID)
```

### Step 6: Update CITATION.cff
Add the DOI to `CITATION.cff`:
```yaml
identifiers:
  - type: doi
    value: 10.5281/zenodo.YOUR_ZENODO_ID
    description: "Zenodo concept DOI for all versions"
```

## For subsequent releases

1. Update version in `CITATION.cff` and `README.md`
2. Create a new GitHub Release (e.g., `v1.1.0`)
3. Zenodo auto-archives it and assigns a new version-specific DOI
4. The concept DOI automatically points to the latest version
5. **No manual work on Zenodo's side**

## Citation format (example)

Once set up, users cite your templates like:

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

## Files

- [`CITATION.cff`](../github/CITATION.cff) — citation metadata (in the github/ folder, used by GitHub + Zenodo)
- [`.zenodo.json`](.zenodo.json) — optional Zenodo-specific metadata override

## Reference

- [Linking GitHub to Zenodo (official guide)](https://help.zenodo.org/docs/deposit/describe-software/)
- [Zenodo GitHub settings](https://zenodo.org/account/settings/github/)
- [Making code citable (GitHub guide)](https://guides.github.com/activities/citable-code/)
