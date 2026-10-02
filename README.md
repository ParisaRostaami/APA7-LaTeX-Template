# APA 7 LaTeX Student Template

A ready-to-use LaTeX template for writing student papers in **APA 7th edition** style, with a full step-by-step guide for students who have never used LaTeX.

Created by **Parisa Rostami**.

<p align="center">
  <a href="https://github.com/ParisaRostaami/APA7-LaTeX-Template/raw/main/APA7_Student_Template.zip"><b>⬇ Download the template (.zip)</b></a>
  &nbsp;·&nbsp;
  <a href="guide/APA7_LaTeX_Student_Guide.pdf"><b>📘 Read the student guide (PDF)</b></a>
  &nbsp;·&nbsp;
  <a href="examples/sample-output.pdf"><b>📄 See a sample output</b></a>
</p>

---

## Quick start (Overleaf, no installation)

1. Download **[APA7_Student_Template.zip](https://github.com/ParisaRostaami/APA7-LaTeX-Template/raw/main/APA7_Student_Template.zip)**. Do not unzip it.
2. Sign in to [Overleaf](https://www.overleaf.com) and click **New Project → Upload project**.
3. Select the zip file. Overleaf creates the project and compiles it.
4. Open `main.tex`, fill in the title-page block, and start writing.
5. Add your sources to `references.bib` and cite them with `\parencite{key}` or `\textcite{key}`.
6. Click **Recompile**, then download your PDF.

> **Mac + Safari:** if Safari unzips the download into a folder, right-click the folder and choose **Compress**, then upload the new `.zip`.

## What the template handles for you

| APA 7 requirement | Handled automatically |
|---|---|
| 1-inch margins, US Letter | ✅ |
| Times New Roman–style 12 pt font | ✅ |
| Double spacing, 0.5-inch paragraph indent, ragged right | ✅ |
| Page numbers top right, no running head (student paper) | ✅ |
| Student title page (title, authors, affiliation, course, instructor, due date) | ✅ layout; you fill in the fields |
| Five APA heading levels | ✅ format; you choose the level |
| Table and figure numbers and titles | ✅ |
| In-text citations and reference list (via `biblatex-apa` + Biber) | ✅ |

## Repository contents

```
APA7-LaTeX-Template/
├── APA7_Student_Template.zip    ← upload this to Overleaf
├── template/                    ← the same files, unzipped (for Git users)
│   ├── main.tex                 ← your paper
│   ├── references.bib           ← your sources
│   ├── figures/                 ← your images
│   └── LICENSE
├── guide/
│   ├── APA7_LaTeX_Student_Guide.pdf
│   └── APA7_LaTeX_Student_Guide.docx
├── examples/
│   └── sample-output.pdf        ← what the template looks like compiled
├── .gitignore                   ← keeps LaTeX temporary files out of Git
└── LICENSE
```

## The student guide

The [student guide](guide/APA7_LaTeX_Student_Guide.pdf) starts from zero and covers:

- what LaTeX and Overleaf are, and the LaTeX basics you need;
- APA 7 student paper rules and what the template does for you;
- every part of the template: the title page, headings, citations and references, tables, figures, equations, code, and appendices;
- structuring a project report, writing as a team, and a submission checklist;
- troubleshooting common errors, plus an FAQ;
- a cheat sheet, working locally with Git, and seven hands-on exercises.

An editable Word version is also in the [`guide`](guide/) folder.

## Working locally

You need a TeX distribution (TeX Live, MacTeX, or MiKTeX) with the `apa7`, `biblatex-apa`, `newtx`, and `csquotes` packages, and Biber. Then:

```bash
git clone https://github.com/ParisaRostaami/APA7-LaTeX-Template.git
cd APA7-LaTeX-Template/template
latexmk -pdf main.tex
```

## Credits and license

Template and guide © 2026 **Parisa Rostami**, licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). You may share and adapt them for non-commercial purposes with credit. **Papers you write with this template belong to you.**

The template builds on the [`apa7`](https://ctan.org/pkg/apa7) class by Daniel A. Weiss and the [`biblatex-apa`](https://ctan.org/pkg/biblatex-apa) style by Philip Kime, which are distributed under the LaTeX Project Public License and are not covered by this repository's license.

Found a problem or have a suggestion? Please [open an issue](https://github.com/ParisaRostaami/APA7-LaTeX-Template/issues).
