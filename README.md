<div align="center">

# arabic-latex-templates

**English** | A collection of **91 Arabic/RTL LaTeX templates** across 10 categories -- academic, business, legal, project management, finance, presentations, letters, marketing, personal, and technical engineering.

**العربية** | مجموعة من **91 قالب لاتيك عربي (RTL)** ضمن 10 فئات -- أكاديمي، أعمال، قانوني، إدارة مشاريع، مالية، عروض تقديمية، رسائل، تسويق، شخصي، وهندسي.

[![License: LPPL-1.3c](https://img.shields.io/badge/license-LPPL--1.3c-blue.svg)](https://www.latex-project.org/lppl/)
[![Templates](https://img.shields.io/badge/templates-91-brightgreen.svg)](#categories--الفئات)
[![Compiler](https://img.shields.io/badge/compiler-XeLaTeX-orange.svg)](https://www.latex-project.org/)
[![Font](https://img.shields.io/badge/font-Amiri-red.svg)](https://www.amirifont.org/)
[![RTL](https://img.shields.io/badge/RTL-Arabic-success.svg)](#)
[![DOI](https://img.shields.io/badge/DOI-Zenodo-blueviolet.svg)](https://doi.org/10.5281/zenodo.YOUR_ZENODO_ID)
[![Open in Overleaf](https://img.shields.io/badge/Open%20in-Overleaf-47A141.svg)](https://www.overleaf.com)

![LaTeX](https://img.shields.io/badge/LaTeX-008080?logo=latex&logoColor=white)
![GitHub stars](https://img.shields.io/github/stars/NibrasAz7/arabic-latex-templates?style=social)
![GitHub forks](https://img.shields.io/github/forks/NibrasAz7/arabic-latex-templates?style=social)

</div>

---

## Categories | الفئات

| # | Category | Count | Highlights |
|---|---|---|---|
| 1 | `Academic_and_Research` | 19 | Article, book, thesis, conference paper, posters, lab report/notebook, grant/research proposal, preprint, manuscript submission, response to reviewers, book chapter, dissertation defense (Beamer), Quran/Hadith |
| 2 | `Business_and_Legal` | 18 | Incorporation, business plan, cap table, agreements (partnership/shareholder/founders/operating/contractor/employment/service/non-compete), NDA, IP assignment, pitch deck, stock options, TOS, privacy policy, financial model |
| 3 | `Project_Management` | 20 | Charter, WBS, Gantt, CPM, RACI, Kanban, risk register, issue log, status report, change request, lessons learned, communication plan, meeting minutes/agenda, decision log, milestone tracker, budget tracker, stakeholder register, procurement plan, kickoff document |
| 4 | `Education_and_Personal` | 10 | CV, resume, exam, syllabus, cheatsheet, technical report, homework assignment, lecture notes, flashcards, certificate |
| 5 | `Presentations` | 4 | Conference talk, lecture slides, sales pitch, webinar (all Beamer 16:9) |
| 6 | `Letters_and_Correspondence` | 4 | Cover letter, recommendation letter, business letter, thank-you letter |
| 7 | `Finance_and_Accounting` | 4 | Invoice, quotation/offer, receipt, financial statement |
| 8 | `Marketing_and_Communications` | 4 | Press release, brochure, newsletter, one-pager |
| 9 | `Personal_and_Life` | 4 | Wedding invitation, recipe book, calendar, weekly planner |
| 10 | `Technical_and_Engineering` | 4 | Technical spec, API reference, datasheet, schematic sheet |
| | **Total | المجموع** | **91** | |

> **العربية:** الفئات هي: أكاديمي وبحثي (19)، أعمال وقانوني (18)، إدارة مشاريع (20)، تعليمي وشخصي (10)، عروض تقديمية (4)، رسائل ومراسلات (4)، مالية ومحاسبة (4)، تسويق واتصالات (4)، شخصي وحياتي (4)، هندسي وتقني (4).

---

## Quick Start | البدء السريع

### Option 1: Open in Overleaf (no install needed) | الخيار 1: الفتح في Overleaf (بدون تثبيت)

Click any link below to open a ready-to-edit copy of the template in [Overleaf](https://www.overleaf.com). No LaTeX install required.

انقر على أي رابط أدناه لفتح نسخة جاهزة للتحرير من القالب في [Overleaf](https://www.overleaf.com). لا يحتاج إلى تثبيت LaTeX.

### Option 2: Clone and compile locally | الخيار 2: الاستنساخ والترجمة محلياً

```bash
git clone https://github.com/NibrasAz7/arabic-latex-templates.git
cd arabic-latex-templates/Academic_and_Research/thesis_template
xelatex main.tex
xelatex main.tex   # run twice for TOC/refs | شغّل مرتين لفهرس المحتويات والمراجع
```

**Requirements | المتطلبات:** XeLaTeX (TeX Live or MiKTeX) with `amiri`, `polyglossia`, `bidi`, `fontspec` packages. The Amiri font must be installed or available to fontspec.

**المتطلبات:** XeLaTeX (TeX Live أو MiKTeX) مع الحزم `amiri` و`polyglossia` و`bidi` و`fontspec`. يجب تثبيت خط Amiri أو توفره لـ fontspec.

### Option 3: Download a single template | الخيار 3: تنزيل قالب واحد

Download any template ZIP from the [`zips/`](zips/) folder, or use GitHub's "Download ZIP" button on any folder.

نزّل أي قالب بصيغة ZIP من مجلد [`zips/`](zips/)، أو استخدم زر "Download ZIP" في GitHub على أي مجلد.

---

## Template Structure | بنية القالب

Each template folder contains | كل مجلد قالب يحتوي على:

```
<template_name>_template/
  main.tex          # XeLaTeX source (start here) | مصدر XeLaTeX (ابدأ هنا)
  main.pdf          # Compiled preview | معاينة مترجمة
  bibliography.bib  # (only for templates with citations) | (فقط للقوالب مع استشهادات)
```

Every `main.tex` starts with `% !TEX program = xelatex` and includes a header comment block with compile instructions and feature list. Placeholder text is marked with `% TODO:` comments.

كل ملف `main.tex` يبدأ بـ `% !TEX program = xelatex` ويتضمن كتلة تعليقات في الرأس مع تعليمات الترجمة وقائمة الميزات. النص Placeholder محدد بتعليقات `% TODO:`.

---

## Compile Commands | أوامر الترجمة

| Template type | Command |
|---|---|
| Most templates | `xelatex main.tex` (run twice) |
| Templates with bibliography | `xelatex main.tex` -> `bibtex main` -> `xelatex main.tex` -> `xelatex main.tex` |
| Beamer presentations | `xelatex main.tex` (run twice) |

> **العربية:** معظم القوالب: `xelatex main.tex` (مرتين). القوالب مع ببليوغرافيا: `xelatex` ثم `bibtex` ثم `xelatex` مرتين. عروض Beamer: `xelatex main.tex` (مرتين).

---

## Tech Stack | التقنيات المستخدمة

| Component | Value |
|---|---|
| Compiler | XeLaTeX |
| Font | Amiri (`Amiri-Regular.ttf`) |
| Arabic/RTL | `polyglossia` + `bidi` |
| English font | TeX Gyre Termes |
| Document class | `article` (most), `beamer` (presentations) |
| Key packages | `graphicx`, `booktabs`, `tabularx`, `tcolorbox`, `tikz`, `fancyhdr`, `titlesec`, `enumitem`, `hyperref` |

> **العربية:** المترجم: XeLaTeX. الخط: Amiri. العربية/RTL: `polyglossia` + `bidi`. الخط الإنجليزي: TeX Gyre Termes. صنف المستند: `article` (معظم القوالب)، `beamer` (العروض). الحزم الرئيسية: `graphicx`، `booktabs`، `tabularx`، `tcolorbox`، `tikz`، `fancyhdr`، `titlesec`، `enumitem`، `hyperref`.

---

## Open in Overleaf -- All 91 Templates | الفتح في Overleaf -- جميع القوالب الـ 91

> ### ⚠️ IMPORTANT: Change the compiler after opening | مهم: غيّر المترجم بعد الفتح ⚠️
>
> **English:** After opening any template in Overleaf, go to **Menu** (top-left) -> **Compiler** -> select **XeLaTeX** or **LuaLaTeX**. The default compiler (pdfLaTeX) will NOT work with Arabic/RTL templates.
>
> **العربية:** بعد فتح أي قالب في Overleaf، اذهب إلى **Menu** (أعلى اليسار) -> **Compiler** -> اختر **XeLaTeX** أو **LuaLaTeX**. المترجم الافتراضي (pdfLaTeX) لن يعمل مع قوالب العربية/RTL.

### Academic and Research | أكاديمي وبحثي

| Template | Open in Overleaf |
|---|---|
| `academic_article` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/academic_article_template.zip) |
| `academic_book` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/academic_book_template.zip) |
| `article` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/article_template.zip) |
| `book_chapter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/book_chapter_template.zip) |
| `book` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/book_template.zip) |
| `conference_paper` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/conference_paper_template.zip) |
| `dissertation_defense` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/dissertation_defense_template.zip) |
| `grant_proposal` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/grant_proposal_template.zip) |
| `lab_notebook` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lab_notebook_template.zip) |
| `lab_report` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lab_report_template.zip) |
| `manuscript_submission` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/manuscript_submission_template.zip) |
| `poster_landscape` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/poster_landscape_template.zip) |
| `poster` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/poster_template.zip) |
| `preprint` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/preprint_template.zip) |
| `quran_hadith` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/quran_hadith_template.zip) |
| `research_proposal` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/research_proposal_template.zip) |
| `response_to_reviewers` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/response_to_reviewers_template.zip) |
| `scientific_article` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/scientific_article_template.zip) |
| `thesis` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thesis_template.zip) |

### Business and Legal | أعمال وقانوني

| Template | Open in Overleaf |
|---|---|
| `articles_of_incorporation` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/articles_of_incorporation_template.zip) |
| `business_plan` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/business_plan_template.zip) |
| `cap_table` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cap_table_template.zip) |
| `contractor_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/contractor_agreement_template.zip) |
| `employment_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/employment_agreement_template.zip) |
| `financial_model` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/financial_model_template.zip) |
| `founders_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/founders_agreement_template.zip) |
| `ip_assignment` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/ip_assignment_template.zip) |
| `nda` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/nda_template.zip) |
| `non_compete` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/non_compete_template.zip) |
| `operating_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/operating_agreement_template.zip) |
| `partnership_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/partnership_agreement_template.zip) |
| `pitch_deck` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/pitch_deck_template.zip) |
| `privacy_policy` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/privacy_policy_template.zip) |
| `service_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/service_agreement_template.zip) |
| `shareholder_agreement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/shareholder_agreement_template.zip) |
| `stock_option_plan` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/stock_option_plan_template.zip) |
| `terms_of_service` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/terms_of_service_template.zip) |

### Education and Personal | تعليمي وشخصي

| Template | Open in Overleaf |
|---|---|
| `certificate` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/certificate_template.zip) |
| `cheatsheet` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cheatsheet_template.zip) |
| `cv` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cv_template.zip) |
| `exam` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/exam_template.zip) |
| `flashcard` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/flashcard_template.zip) |
| `homework_assignment` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/homework_assignment_template.zip) |
| `lecture_notes` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lecture_notes_template.zip) |
| `resume` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/resume_template.zip) |
| `syllabus` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/syllabus_template.zip) |
| `technical_report` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/technical_report_template.zip) |

### Finance and Accounting | مالية ومحاسبة

| Template | Open in Overleaf |
|---|---|
| `financial_statement` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/financial_statement_template.zip) |
| `invoice` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/invoice_template.zip) |
| `quotation_offer` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/quotation_offer_template.zip) |
| `receipt` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/receipt_template.zip) |

### Letters and Correspondence | رسائل ومراسلات

| Template | Open in Overleaf |
|---|---|
| `business_letter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/business_letter_template.zip) |
| `cover_letter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cover_letter_template.zip) |
| `recommendation_letter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/recommendation_letter_template.zip) |
| `thank_you_letter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thank_you_letter_template.zip) |

### Marketing and Communications | تسويق واتصالات

| Template | Open in Overleaf |
|---|---|
| `brochure` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/brochure_template.zip) |
| `newsletter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/newsletter_template.zip) |
| `one_pager` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/one_pager_template.zip) |
| `press_release` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/press_release_template.zip) |

### Personal and Life | شخصي وحياتي

| Template | Open in Overleaf |
|---|---|
| `calendar` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/calendar_template.zip) |
| `planner` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/planner_template.zip) |
| `recipe_book` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/recipe_book_template.zip) |
| `wedding_invitation` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/wedding_invitation_template.zip) |

### Presentations | عروض تقديمية

| Template | Open in Overleaf |
|---|---|
| `conference_talk` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/conference_talk_template.zip) |
| `lecture_slides` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lecture_slides_template.zip) |
| `sales_pitch` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/sales_pitch_template.zip) |
| `webinar` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/webinar_template.zip) |

### Project Management | إدارة المشاريع

| Template | Open in Overleaf |
|---|---|
| `budget_tracker` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/budget_tracker_template.zip) |
| `change_request` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/change_request_template.zip) |
| `communication_plan` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/communication_plan_template.zip) |
| `cpm_diagram` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cpm_diagram_template.zip) |
| `decision_log` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/decision_log_template.zip) |
| `gantt_chart` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/gantt_chart_template.zip) |
| `issue_log` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/issue_log_template.zip) |
| `kanban_board` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/kanban_board_template.zip) |
| `kickoff_document` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/kickoff_document_template.zip) |
| `lessons_learned` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lessons_learned_template.zip) |
| `meeting_agenda` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/meeting_agenda_template.zip) |
| `meeting_minutes` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/meeting_minutes_template.zip) |
| `milestone_tracker` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/milestone_tracker_template.zip) |
| `procurement_plan` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/procurement_plan_template.zip) |
| `project_charter` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/project_charter_template.zip) |
| `raci_matrix` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/raci_matrix_template.zip) |
| `risk_register` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/risk_register_template.zip) |
| `stakeholder_register` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/stakeholder_register_template.zip) |
| `status_report` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/status_report_template.zip) |
| `wbs` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/wbs_template.zip) |

### Technical and Engineering | هندسي وتقني

| Template | Open in Overleaf |
|---|---|
| `api_reference` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/api_reference_template.zip) |
| `datasheet` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/datasheet_template.zip) |
| `schematic` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/schematic_template.zip) |
| `technical_spec` | [Open in Overleaf](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/technical_spec_template.zip) |

---

## Citing | الاقتباس

If you use these templates in academic work, please cite:

إذا استخدمت هذه القوالب في عمل أكاديمي، يرجى الاقتباس:

```bibtex
@software{arabic_latex_templates,
  author       = {Nibras ABO ALZAHAB},
  title        = {arabic-latex-templates: 91 Arabic/RTL LaTeX templates},
  year         = 2026,
  publisher    = {Zenodo},
  version      = {v1.0.0},
  doi          = {10.5281/zenodo.YOUR_ZENODO_ID},
  url          = {https://doi.org/10.5281/zenodo.YOUR_ZENODO_ID}
}
```

Or click the **"Cite this repository"** button on GitHub (powered by `CITATION.cff`).

أو انقر زر **"Cite this repository"** في GitHub (مدعوم بـ `CITATION.cff`).

---

## License | الرخصة

LaTeX Project Public License v1.3c (LPPL-1.3c) -- see [LICENSE](LICENSE).

رخصة LaTeX Project Public License v1.3c (LPPL-1.3c) -- انظر [LICENSE](LICENSE).
