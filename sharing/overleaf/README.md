# Overleaf Distribution

[Overleaf](https://www.overleaf.com) is the most popular online LaTeX editor. These templates can be shared via Overleaf in several ways.

## Method 1: One-Click API Links (recommended)

Overleaf's API can start a new project from a ZIP at a public URL. The ZIPs are stored in the `zips/` folder of this repo and served via GitHub's `raw.githubusercontent.com` CDN.

### Link format

The key parameter is **`snip_uri`** (not `zip`). It points to a publicly accessible ZIP file:

```
https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thesis_template.zip
```

### Full link table

See [`links.md`](links.md) for all 91 one-click links. Click any link and Overleaf opens a ready-to-edit copy of the template -- no LaTeX install required.

### How the ZIPs are maintained

The per-template ZIPs live in `zips/` at the repo root. Each ZIP contains `main.tex`, `main.pdf`, and any supporting files (bibliography, chapters, etc.) for that template.

To regenerate all ZIPs after updating templates:

```powershell
$base = "path/to/arabic-latex-templates"
$zipDir = Join-Path $base "zips"
Get-ChildItem -Path $base -Directory | Where-Object { $_.Name -ne "sharing" -and $_.Name -ne "zips" -and $_.Name -ne ".github" } | ForEach-Object {
  Get-ChildItem -Path $_.FullName -Directory | ForEach-Object {
    Compress-Archive -Path (Join-Path $_.FullName "*") -DestinationPath (Join-Path $zipDir "$($_.Name).zip") -Force
  }
}
```

## Method 2: Import from GitHub

Overleaf has built-in GitHub integration. This imports the entire repo as a single project.

### Setup (one-time)
1. Go to [overleaf.com](https://www.overleaf.com) -> **New Project** -> **Import from GitHub**
2. Authorize Overleaf to access your GitHub (one-time)
3. Select `arabic-latex-templates` from the repo list
4. Overleaf imports the entire repo as a project

### For end users
Users can either:
- **Fork the repo** to their own GitHub, then import from Overleaf
- **Copy a single template folder** to a new repo, then import
- Use the **one-click API links** above (Method 1)

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
Submit 3-5 standout templates to the Gallery (e.g., `thesis_template`, `scientific_article_template`, `cv_template`, `conference_talk_template`). Use Method 1 for the rest.

## Method 4: Link Sharing (for small groups)

For sharing with specific people (students, colleagues):

1. Create a new Overleaf project from a template
2. Click **Share** -> **Turn on link sharing**
3. Copy the "Edit link" or "View link"
4. Send to your collaborators

Best for classroom use (e.g., distributing a homework template to students).

## Reference

- [Overleaf API documentation](https://www.overleaf.com/devs)
- [Import from GitHub on Overleaf](https://www.overleaf.com/learn/how-to/Importing_from_GitHub)
- [Publishing to the Overleaf Gallery](https://www.overleaf.com/learn/how-to/Publishing_templates_and_examples_in_the_Overleaf_Gallery)
- [Sharing a project](https://www.overleaf.com/learn/how-to/Sharing_a_project)
