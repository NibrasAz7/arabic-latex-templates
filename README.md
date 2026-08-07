<div align="center">

# Arabic LaTeX Templates

Nibras's collection of **91 Arabic/RTL LaTeX templates** across 10 categories.

مجموعة من **91 قالب لاتيك عربي (RTL)** ضمن 10 فئات.

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

| # | Category (EN) | الفئة (AR) | Count | Highlights (EN) | أبرز القوالب (AR) |
|---|---|---|---|---|---|
| 1 | Academic and Research | أكاديمي وبحثي | 19 | Article, book, thesis, conference paper, posters, lab report, grant proposal, preprint, Quran/Hadith | مقال، كتاب، أطروحة، ورقة مؤتمر، ملصقات، تقرير مختبر، مقترح منحة، قبل النشر، قرآن وحديث |
| 2 | Business and Legal | أعمال وقانوني | 18 | Incorporation, business plan, cap table, agreements, NDA, IP, pitch deck, TOS, privacy policy | تأسيس، خطة عمل، جدول رأس المال، اتفاقيات، عدم إفصاح، ملكية فكرية، عرض تقديمي، شروط خدمة، خصوصية |
| 3 | Project Management | إدارة مشاريع | 20 | Charter, WBS, Gantt, CPM, RACI, Kanban, risk register, issue log, status report, meeting minutes | ميثاق، هيكل تقسيم، جانت، CPM، RACI، كانبان، سجل مخاطر، سجل مشكلات، تقرير حالة، محضر اجتماع |
| 4 | Education and Personal | تعليمي وشخصي | 10 | CV, resume, exam, syllabus, cheatsheet, homework, lecture notes, flashcards, certificate | سيرة ذاتية، امتحان، خطة مقرر، ورقة مرجعية، واجب، ملاحظات محاضرة، بطاقات تعليمية، شهادة |
| 5 | Presentations | عروض تقديمية | 4 | Conference talk, lecture slides, sales pitch, webinar (Beamer 16:9) | محاضرة مؤتمر، شرائح محاضرة، عرض بيع، ندوة إلكترونية |
| 6 | Letters and Correspondence | رسائل ومراسلات | 4 | Cover letter, recommendation letter, business letter, thank-you letter | رسالة تغطية، رسالة توصية، رسالة عمل، رسالة شكر |
| 7 | Finance and Accounting | مالية ومحاسبة | 4 | Invoice, quotation/offer, receipt, financial statement | فاتورة، عرض سعر، إيصال، بيان مالي |
| 8 | Marketing and Communications | تسويق واتصالات | 4 | Press release, brochure, newsletter, one-pager | بيان صحفي، كتيب، نشرة إخبارية، صفحة واحدة |
| 9 | Personal and Life | شخصي وحياتي | 4 | Wedding invitation, recipe book, calendar, weekly planner | دعوة زفاف، كتاب وصفات، تقويم، مخطط أسبوعي |
| 10 | Technical and Engineering | هندسي وتقني | 4 | Technical spec, API reference, datasheet, schematic sheet | مواصفات تقنية، مرجع API، صحيفة بيانات، مخطط كهربائي |
| | | **المجموع** | **91** | | |

---

## Quick Start | البدء السريع

### Option 1: Open in Overleaf | الخيار 1: الفتح في Overleaf

Click any link in the tables below to open a ready-to-edit copy in [Overleaf](https://www.overleaf.com). No LaTeX install required.

انقر على أي رابط في الجداول أدناه لفتح نسخة جاهزة للتحرير في [Overleaf](https://www.overleaf.com). لا يحتاج إلى تثبيت LaTeX.

### Option 2: Clone and compile locally | الخيار 2: الاستنساخ والترجمة محلياً

```bash
git clone https://github.com/NibrasAz7/arabic-latex-templates.git
cd arabic-latex-templates/Academic_and_Research/thesis_template
xelatex main.tex
xelatex main.tex   # run twice for TOC/refs
```

**Requirements:** XeLaTeX (TeX Live or MiKTeX) with `amiri`, `polyglossia`, `bidi`, `fontspec` packages. The Amiri font must be installed.

**المتطلبات:** XeLaTeX (TeX Live أو MiKTeX) مع حزم `amiri` و`polyglossia` و`bidi` و`fontspec`. يجب تثبيت خط Amiri.

### Option 3: Download a single template | الخيار 3: تنزيل قالب واحد

Use the "Download ZIP" column in the tables below, or browse the [`zips/`](zips/) folder.

استخدم عمود "Download ZIP" في الجداول أدناه، أو تصفح مجلد [`zips/`](zips/).

---

## Template Structure | بنية القالب

```
<template_name>_template/
  main.tex          # XeLaTeX source
  main.pdf          # Compiled preview
  bibliography.bib  # (only for templates with citations)
```

---

## Compile Commands | أوامر الترجمة

| Template type | Command |
|---|---|
| Most templates | `xelatex main.tex` (run twice) |
| With bibliography | `xelatex main.tex` -> `bibtex main` -> `xelatex main.tex` -> `xelatex main.tex` |
| Beamer presentations | `xelatex main.tex` (run twice) |

---

## Tech Stack | التقنيات

| Component | Value |
|---|---|
| Compiler | XeLaTeX |
| Font | Amiri (`Amiri-Regular.ttf`) |
| Arabic/RTL | `polyglossia` + `bidi` |
| English font | TeX Gyre Termes |
| Document class | `article` (most), `beamer` (presentations) |
| Key packages | `graphicx`, `booktabs`, `tabularx`, `tcolorbox`, `tikz`, `fancyhdr`, `titlesec`, `enumitem`, `hyperref` |

---

## Open in Overleaf -- All 91 Templates

> ### ⚠️ IMPORTANT: Change the compiler after opening | مهم: غيّر المترجم بعد الفتح ⚠️
>
> **English:** After opening any template in Overleaf, go to **Menu** (top-left) -> **Compiler** -> select **XeLaTeX** or **LuaLaTeX**. The default compiler (pdfLaTeX) will NOT work with Arabic/RTL templates.
>
> **العربية:** بعد فتح أي قالب في Overleaf، اذهب إلى **Menu** (أعلى اليسار) -> **Compiler** -> اختر **XeLaTeX** أو **LuaLaTeX**. المترجم الافتراضي (pdfLaTeX) لن يعمل مع قوالب العربية/RTL.

---

### Academic and Research | أكاديمي وبحثي

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `academic_article` | Academic journal article | مقال أكاديمي في مجلة علمية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/academic_article_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/academic_article_template.zip) |
| `academic_book` | Full academic book | كتاب أكاديمي كامل | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/academic_book_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/academic_book_template.zip) |
| `article` | General article | مقال عام | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/article_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/article_template.zip) |
| `book_chapter` | Book chapter | فصل في كتاب | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/book_chapter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/book_chapter_template.zip) |
| `book` | General book | كتاب عام | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/book_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/book_template.zip) |
| `conference_paper` | Conference paper | ورقة مؤتمر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/conference_paper_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/conference_paper_template.zip) |
| `dissertation_defense` | Dissertation defense slides | شرائح مناقشة أطروحة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/dissertation_defense_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/dissertation_defense_template.zip) |
| `grant_proposal` | Research grant proposal | مقترح منحة بحثية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/grant_proposal_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/grant_proposal_template.zip) |
| `lab_notebook` | Lab notebook | دفتر مختبر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lab_notebook_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lab_notebook_template.zip) |
| `lab_report` | Lab report | تقرير مختبر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lab_report_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lab_report_template.zip) |
| `manuscript_submission` | Manuscript submission | تقديم مخطوطة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/manuscript_submission_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/manuscript_submission_template.zip) |
| `poster_landscape` | Landscape poster | ملصق أفقي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/poster_landscape_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/poster_landscape_template.zip) |
| `poster` | Portrait poster | ملصق عمودي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/poster_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/poster_template.zip) |
| `preprint` | Preprint paper | ورقة قبل النشر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/preprint_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/preprint_template.zip) |
| `quran_hadith` | Quran and Hadith document | وثيقة قرآن وحديث | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/quran_hadith_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/quran_hadith_template.zip) |
| `research_proposal` | Research proposal | مقترح بحثي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/research_proposal_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/research_proposal_template.zip) |
| `response_to_reviewers` | Response to reviewers | رد على المراجعين | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/response_to_reviewers_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/response_to_reviewers_template.zip) |
| `scientific_article` | Scientific article | مقال علمي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/scientific_article_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/scientific_article_template.zip) |
| `thesis` | Thesis / dissertation | أطروحة / رسالة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thesis_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thesis_template.zip) |

---

### Business and Legal | أعمال وقانوني

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `articles_of_incorporation` | Articles of incorporation | عقد التأسيس | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/articles_of_incorporation_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/articles_of_incorporation_template.zip) |
| `business_plan` | Business plan | خطة عمل | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/business_plan_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/business_plan_template.zip) |
| `cap_table` | Capitalization table | جدول رأس المال | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cap_table_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cap_table_template.zip) |
| `contractor_agreement` | Contractor agreement | اتفاقية مقاول | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/contractor_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/contractor_agreement_template.zip) |
| `employment_agreement` | Employment agreement | اتفاقية عمل | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/employment_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/employment_agreement_template.zip) |
| `financial_model` | Financial model | نموذج مالي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/financial_model_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/financial_model_template.zip) |
| `founders_agreement` | Founders agreement | اتفاقية المؤسسين | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/founders_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/founders_agreement_template.zip) |
| `ip_assignment` | IP assignment | تنازل عن الملكية الفكرية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/ip_assignment_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/ip_assignment_template.zip) |
| `nda` | Non-disclosure agreement | اتفاقية عدم إفصاح | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/nda_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/nda_template.zip) |
| `non_compete` | Non-compete agreement | اتفاقية عدم منافسة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/non_compete_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/non_compete_template.zip) |
| `operating_agreement` | Operating agreement | اتفاقية تشغيل | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/operating_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/operating_agreement_template.zip) |
| `partnership_agreement` | Partnership agreement | اتفاقية شراكة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/partnership_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/partnership_agreement_template.zip) |
| `pitch_deck` | Pitch deck slides | شرائح عرض تقديمي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/pitch_deck_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/pitch_deck_template.zip) |
| `privacy_policy` | Privacy policy | سياسة الخصوصية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/privacy_policy_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/privacy_policy_template.zip) |
| `service_agreement` | Service agreement | اتفاقية خدمة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/service_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/service_agreement_template.zip) |
| `shareholder_agreement` | Shareholder agreement | اتفاقية مساهمين | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/shareholder_agreement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/shareholder_agreement_template.zip) |
| `stock_option_plan` | Stock option plan | خطة خيارات الأسهم | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/stock_option_plan_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/stock_option_plan_template.zip) |
| `terms_of_service` | Terms of service | شروط الخدمة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/terms_of_service_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/terms_of_service_template.zip) |

---

### Education and Personal | تعليمي وشخصي

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `certificate` | Certificate | شهادة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/certificate_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/certificate_template.zip) |
| `cheatsheet` | Cheatsheet | ورقة مرجعية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cheatsheet_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cheatsheet_template.zip) |
| `cv` | Curriculum vitae | السيرة الذاتية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cv_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cv_template.zip) |
| `exam` | Exam paper | ورقة امتحان | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/exam_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/exam_template.zip) |
| `flashcard` | Flashcards | بطاقات تعليمية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/flashcard_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/flashcard_template.zip) |
| `homework_assignment` | Homework assignment | واجب منزلي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/homework_assignment_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/homework_assignment_template.zip) |
| `lecture_notes` | Lecture notes | ملاحظات محاضرة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lecture_notes_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lecture_notes_template.zip) |
| `resume` | Resume | سيرة ذاتية مختصرة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/resume_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/resume_template.zip) |
| `syllabus` | Course syllabus | خطة مقرر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/syllabus_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/syllabus_template.zip) |
| `technical_report` | Technical report | تقرير تقني | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/technical_report_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/technical_report_template.zip) |

---

### Finance and Accounting | مالية ومحاسبة

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `financial_statement` | Financial statement | بيان مالي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/financial_statement_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/financial_statement_template.zip) |
| `invoice` | Invoice | فاتورة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/invoice_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/invoice_template.zip) |
| `quotation_offer` | Quotation / offer | عرض سعر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/quotation_offer_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/quotation_offer_template.zip) |
| `receipt` | Receipt | إيصال | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/receipt_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/receipt_template.zip) |

---

### Letters and Correspondence | رسائل ومراسلات

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `business_letter` | Business letter | رسالة عمل | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/business_letter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/business_letter_template.zip) |
| `cover_letter` | Cover letter | رسالة تغطية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cover_letter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cover_letter_template.zip) |
| `recommendation_letter` | Recommendation letter | رسالة توصية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/recommendation_letter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/recommendation_letter_template.zip) |
| `thank_you_letter` | Thank-you letter | رسالة شكر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thank_you_letter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/thank_you_letter_template.zip) |

---

### Marketing and Communications | تسويق واتصالات

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `brochure` | Brochure | كتيب | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/brochure_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/brochure_template.zip) |
| `newsletter` | Newsletter | نشرة إخبارية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/newsletter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/newsletter_template.zip) |
| `one_pager` | One-pager | صفحة واحدة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/one_pager_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/one_pager_template.zip) |
| `press_release` | Press release | بيان صحفي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/press_release_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/press_release_template.zip) |

---

### Personal and Life | شخصي وحياتي

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `calendar` | Calendar | تقويم | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/calendar_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/calendar_template.zip) |
| `planner` | Weekly planner | مخطط أسبوعي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/planner_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/planner_template.zip) |
| `recipe_book` | Recipe book | كتاب وصفات | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/recipe_book_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/recipe_book_template.zip) |
| `wedding_invitation` | Wedding invitation | دعوة زفاف | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/wedding_invitation_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/wedding_invitation_template.zip) |

---

### Presentations | عروض تقديمية

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `conference_talk` | Conference talk | محاضرة مؤتمر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/conference_talk_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/conference_talk_template.zip) |
| `lecture_slides` | Lecture slides | شرائح محاضرة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lecture_slides_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lecture_slides_template.zip) |
| `sales_pitch` | Sales pitch | عرض بيع | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/sales_pitch_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/sales_pitch_template.zip) |
| `webinar` | Webinar | ندوة إلكترونية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/webinar_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/webinar_template.zip) |

---

### Project Management | إدارة المشاريع

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `budget_tracker` | Budget tracker | متتبع ميزانية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/budget_tracker_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/budget_tracker_template.zip) |
| `change_request` | Change request | طلب تغيير | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/change_request_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/change_request_template.zip) |
| `communication_plan` | Communication plan | خطة اتصال | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/communication_plan_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/communication_plan_template.zip) |
| `cpm_diagram` | CPM diagram | مخطط CPM | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cpm_diagram_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/cpm_diagram_template.zip) |
| `decision_log` | Decision log | سجل قرارات | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/decision_log_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/decision_log_template.zip) |
| `gantt_chart` | Gantt chart | مخطط جانت | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/gantt_chart_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/gantt_chart_template.zip) |
| `issue_log` | Issue log | سجل مشكلات | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/issue_log_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/issue_log_template.zip) |
| `kanban_board` | Kanban board | لوحة كانبان | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/kanban_board_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/kanban_board_template.zip) |
| `kickoff_document` | Kickoff document | وثيقة انطلاق | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/kickoff_document_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/kickoff_document_template.zip) |
| `lessons_learned` | Lessons learned | الدروس المستفادة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lessons_learned_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/lessons_learned_template.zip) |
| `meeting_agenda` | Meeting agenda | جدول أعمال اجتماع | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/meeting_agenda_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/meeting_agenda_template.zip) |
| `meeting_minutes` | Meeting minutes | محضر اجتماع | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/meeting_minutes_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/meeting_minutes_template.zip) |
| `milestone_tracker` | Milestone tracker | متتبع معالم | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/milestone_tracker_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/milestone_tracker_template.zip) |
| `procurement_plan` | Procurement plan | خطة مشتريات | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/procurement_plan_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/procurement_plan_template.zip) |
| `project_charter` | Project charter | ميثاق مشروع | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/project_charter_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/project_charter_template.zip) |
| `raci_matrix` | RACI matrix | مصفوفة RACI | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/raci_matrix_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/raci_matrix_template.zip) |
| `risk_register` | Risk register | سجل مخاطر | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/risk_register_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/risk_register_template.zip) |
| `stakeholder_register` | Stakeholder register | سجل أصحاب المصلحة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/stakeholder_register_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/stakeholder_register_template.zip) |
| `status_report` | Status report | تقرير حالة | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/status_report_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/status_report_template.zip) |
| `wbs` | Work breakdown structure | هيكل تقسيم العمل | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/wbs_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/wbs_template.zip) |

---

### Technical and Engineering | هندسي وتقني

| Template | Description (EN) | الشرح (AR) | Open in Overleaf | Download ZIP |
|---|---|---|---|---|
| `api_reference` | API reference | مرجع API | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/api_reference_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/api_reference_template.zip) |
| `datasheet` | Datasheet | صحيفة بيانات | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/datasheet_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/datasheet_template.zip) |
| `schematic` | Schematic sheet | مخطط كهربائي | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/schematic_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/schematic_template.zip) |
| `technical_spec` | Technical specification | مواصفات تقنية | [Open](https://www.overleaf.com/docs?snip_uri=https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/technical_spec_template.zip) | [ZIP](https://raw.githubusercontent.com/NibrasAz7/arabic-latex-templates/main/zips/technical_spec_template.zip) |

---

## Citing | الاقتباس

If you use these templates in academic work, please cite:

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

---

## License | الرخصة

LaTeX Project Public License v1.3c (LPPL-1.3c) -- see [LICENSE](LICENSE).
