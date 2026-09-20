# CHANGELOG — cv

## [1.3.0] — 2026-09-09

### Changed
- [x] Full CV rewrite for Ismael POUANSI KOLOKO (École Polytechnique, tutoring, certifications, football)
- [x] Source renamed to `CV_POUANSI_Ismael.tex` / output `CV_POUANSI_Ismael.pdf`
- [x] Workflow `build-pdf.yml` + README + AGENTS updated to the new name and repo (`ismael-Ing-1/cv`)

---

## [1.4.0] — 2026-09-20

### Added
- [x] PSC (École Polytechnique, with CMA CGM): deep learning for vessel ETA prediction to cut fuel consumption and CO2 emissions

### Changed
- [x] Languages: English (Intermediate), Chinese (Beginner)
- [x] IT Skills: Python, C++, Java
- [x] Sports: football stated as competitive level
- [x] Interests: add drawing
- [x] ENS Yaoundé: remove preparatory classes, note Software Engineering specialisation and Cameroon's first engineering school
- [x] École Polytechnique: mention France's top engineering school, dates 2025--2028
- [x] LinkedIn URL shortened to `in/ismael-pouansi`

---

## [Unreleased]

### Changed
- [x] Education titles state each school's national standing: École Polytechnique (France's top leading school), ENS Yaoundé (Cameroon's top engineering school)
- [x] École Polytechnique: add advanced Mathematics, Physics, and Computer Science coursework
- [x] Formatting: eased line and item spacing for readability, still one page

---

## [1.2.0] — 2026-09-05

### Added
- [x] HR header: centered pitch + 6-month research internship sought from end of March 2027
- [x] Quantified DxO entry (eye-state CNN, blur corpus) from the culling-presentation deck
- [x] `scripts/check-dashes.sh`: fail on em-dash (`---`) outside comments, runs first in `make check`
- [x] `make build` (always rebuilds, no timestamp check); bare `make` shows help
- [x] `make check`: dashes → build → 1-page gate (also gates `make push`)

### Changed
- [x] Repo renamed `cv-atf` → `cv` (GitHub `KpihX/cv`, GitLab `kpihx/cv`, remotes `github`/`gitlab`)
- [x] Skills rewritten in plain language; software/cloud/infra merged
- [x] Page geometry bottom `0.45in` → `0.3in` to hold 1 page

### Removed
- [x] `make clean` target

---

## [1.0.0] — 2026-03-22

### Added
- [x] Initial CV source: moderncv banking style, blue theme, pdflatex
- [x] Sections: Education, Professional Experience, Projects Highlights, Technical Skills, Extracurriculars & Awards
- [x] GitLab CI pipeline (`.gitlab-ci.yml`): pdflatex double-pass, PDF + PNG artifacts (1 year)
- [x] GitHub Actions pipeline (`.github/workflows/build-pdf.yml`): pdflatex, PDF artifact, auto-preview PNG commit, Release on tag
- [x] README with CI badges and preview image
- [x] Source renamed to `CV_POUANSI_Ismael.tex` / output `CV_POUANSI_Ismael.pdf`

### Fixed
- [x] Color rendering: `\moderncvcolor` must precede `\moderncvstyle` in moderncv v2.4.1 (banking loads `\colorlet{sectioncolor}{color1}` at package load time)
- [x] Bold lost on entry titles: switched from XeLaTeX to pdflatex + `lmodern` + T1 encoding
- [x] Name tint: forced `firstnamecolor = color1` (banking default is `lastnamecolor!60`)
- [x] GitLab CI YAML: removed nested block scalar (`|`) inside script list items
- [x] XeLaTeX `\cventry` inside `\begin{itemize}` conflict: removed outer itemize wrappers

---

*Format: [Keep a Changelog](https://keepachangelog.com) · Versioning: [SemVer](https://semver.org)*
