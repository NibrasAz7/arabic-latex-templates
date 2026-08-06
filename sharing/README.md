# Sharing & Distribution

This directory contains everything needed to share the 91 Arabic/RTL LaTeX templates via four channels.

## Channels

| Channel | Folder | How it works | Effort |
|---|---|---|---|
| **GitHub** | [`github/`](github/) | Canonical home. Templates stored as source (no ZIPs in repo). CI compiles + verifies on every push. Releases auto-build ZIPs as assets. | Low |
| **Overleaf** | [`overleaf/`](overleaf/) | Users import from GitHub directly, or use one-click API links pointing to GitHub Release assets. Zero install. | Low |
| **Zenodo** | [`zenodo/`](zenodo/) | Auto-connected to GitHub. Each Release → permanent DOI. No manual uploads. | Low |
| **CTAN** | [`ctan/`](ctan/) | Submit `arabic-templates.zip` to ctan.org. Ships via `tlmgr install`. | Medium |

## Recommended workflow

1. **GitHub** — push the repo. No ZIPs in the repo itself; CI builds them on release.
2. **Overleaf** — users import from GitHub, or use the one-click links (pointing to Release assets).
3. **Zenodo** — connect GitHub → Zenodo (one toggle). First release auto-mints a DOI. Add badge to README.
4. **CTAN** — submit when ready for maximum LaTeX-community reach.

## What's in each folder

### `github/`
- `README.md` — repo README with shields.io badges, category table, quick start
- `LICENSE` — LPPL-1.3c
- `CITATION.cff` — citation metadata (GitHub "Cite this repository" button)
- `.gitignore` — ignores LaTeX build artifacts
- `.github/workflows/compile-and-verify.yml` — CI: compiles all templates, builds ZIPs on release
- `TOPICS.md` — suggested GitHub repository topics/tags for discoverability

### `overleaf/`
- `README.md` — four sharing methods (GitHub import, API links, Gallery, link sharing)
- `links.md` — 91 one-click Overleaf API links (pointing to GitHub Release assets)

### `zenodo/`
- `README.md` — Zenodo-GitHub auto-connection setup guide
- `.zenodo.json` — Zenodo metadata override

### `ctan/`
- `README.md` — CTAN submission guide
- `arabic-templates.zip` — ready-to-submit archive
- `arabic-templates/` — unpacked package (docs + all 91 templates)

## Key design decisions

- **No ZIPs in the git repo** — bloats history. ZIPs are built by CI and attached to GitHub Releases as assets.
- **Zenodo is auto-connected to GitHub** — no manual Zenodo uploads. Releases trigger DOI minting.
- **Overleaf links point to Release assets** — permanent, CDN-backed URLs.
- **Each template has a compiled `main.pdf`** — users can preview on GitHub without downloading.
