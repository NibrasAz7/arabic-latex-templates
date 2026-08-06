# Overleaf Distribution

[Overleaf](https://www.overleaf.com) is the most popular online LaTeX editor. These templates can be shared via Overleaf in three ways.

## Method 1: Import from GitHub (easiest, no ZIPs needed)

Overleaf has built-in GitHub integration. This is the cleanest approach â€” no ZIPs stored anywhere.

### Setup (one-time)
1. Push this repository to GitHub
2. Go to [overleaf.com](https://www.overleaf.com) â†’ **New Project** â†’ **Import from GitHub**
3. Authorize Overleaf to access your GitHub (one-time)
4. Select `arabic-latex-templates` from the repo list
5. Overleaf imports the entire repo as a project

### For end users
Users can either:
- **Fork the repo** to their own GitHub, then import from Overleaf
- **Copy a single template folder** to a new repo, then import
- Use the **one-click API links** below (Method 2)

## Method 2: One-Click API Links (via GitHub Release assets)

Overleaf's API can start a new project from a ZIP at a public URL. Instead of storing ZIPs in the repo (bad practice â€” bloats git history), ZIPs are built by GitHub Actions and attached to **GitHub Releases** as assets.

### Link format
```
https://www.overleaf.com/docs?zip=https://github.com/NibrasAz7/arabic-latex-templates/releases/download/v1.0.0/thesis_template.zip
```

### Full link table

See [`links.md`](links.md) for all 91 one-click links. These URLs point to GitHub Release assets, which are:
- Permanent (Release assets don't change)
- Fast (GitHub CDN)
- Versioned (each release has its own set)

### How the ZIPs get built

The CI workflow (`.github/workflows/compile-and-verify.yml`) automatically:
1. Compiles all 91 templates (verifies they build)
2. Builds a ZIP per template
3. Builds an all-templates bundle ZIP
4. Attaches all ZIPs to the GitHub Release as downloadable assets

This runs automatically when you publish a release. **No ZIPs are stored in the git repo itself.**

## Method 3: Overleaf Gallery Submission (for standout templates)

The [Overleaf Gallery](https://www.overleaf.com/gallery) is a curated, searchable collection. Overleaf staff review submissions.

### When to submit to the Gallery
- Official/standard templates (thesis, journal article, conference paper)
- Templates with broad appeal and polished design
- **Not** suitable for: homework, letters, personal templates, or large batches

### How to submit
1. Go to https://www.overleaf.com/latex/templates
2. Click "Submit a template to the gallery"
3. Upload your template as an Overleaf project
4. Add title, description, tags, and a preview image
5. Overleaf staff review and publish (may take days/weeks)

### Recommendation for this collection
Submit 3-5 standout templates to the Gallery (e.g., `thesis_template`, `scientific_article_template`, `cv_template`, `conference_talk_template`). Use Methods 1 & 2 for the rest.

## Method 4: Link Sharing (for small groups)

For sharing with specific people (students, colleagues):

1. Create a new Overleaf project from a template
2. Click **Share** â†’ **Turn on link sharing**
3. Copy the "Edit link" or "View link"
4. Send to your collaborators

Best for classroom use (e.g., distributing a homework template to students).

## Reference

- [Overleaf API documentation](https://www.overleaf.com/devs)
- [Import from GitHub on Overleaf](https://www.overleaf.com/learn/how-to/Importing_from_GitHub)
- [Publishing to the Overleaf Gallery](https://www.overleaf.com/learn/how-to/Publishing_templates_and_examples_in_the_Overleaf_Gallery)
- [Sharing a project](https://www.overleaf.com/learn/how-to/Sharing_a_project)
