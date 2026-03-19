# Changelog

All notable changes to the FENITH meta-repository are documented here.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/).

---

## [v0.7.0] — 2026-03-19

### Added
- `index.md` for GitHub Pages (Cayman theme landing page)
- Table of Contents in README
- GitHub stars and forks badges
- Missing GitHub Releases for v0.2.2, v0.3.1, v0.3.2

### Changed
- Publication statuses: P-IS → Accepted, P-CR → Accepted, P-C2 → Presented
- At a Glance: "2 pending" → "2 accepted"
- Keyword case fixed (`omop-OHDSI` → `omop-ohdsi`)
- Repo description changed to English
- `_config.yml` enriched with baseurl and show_downloads
- Gantt timeline: thesis writing ends 2026-05, defense TBD
- CHANGELOG.md brought up to date (v0.5.1–v0.6.2)

---

## [v0.6.2] — 2026-03-19

### Fixed
- Link checker: added doi.org, scholar.google.com, researchgate.net to ignore list (403 on bot requests)

---

## [v0.6.1] — 2026-03-19

### Changed
- `docs/papers/INDEX.md`: Title column moved before File, File in `<small>` text
- Citation badge: static Google Scholar count (21) replacing Semantic Scholar

---

## [v0.6.0] — 2026-03-19

### Added
- SECURITY.md with responsible disclosure policy
- `docs/README.md` documentation guide
- Hover tooltips on Cluster column in RQ tables (EN + IT)
- Thesis delivery milestone (2026-05-31) in Gantt timeline

### Changed
- CONTRIBUTING.md: added How to Cite section and RQ reference in issues
- Repository structure tree updated (SECURITY.md, docs/README.md)
- 10 new GitHub Topics synced with README keywords
- Repository homepage set to fenith.org

---

## [v0.5.2] — 2026-03-19

### Changed
- RQ tooltips switched from `<abbr>` to markdown link titles (GitHub-compatible)

---

## [v0.5.1] — 2026-03-19

### Added
- Hover tooltips on RQ references in cluster tables (`<abbr>` tags — later replaced in v0.5.2)

---

## [v0.5.0] — 2026-03-19

### Added
- RQ column (Research Questions mapping) in all 4 cluster tables
- RQ annotations in `docs/architecture.md` Mermaid diagram
- DOI badge and CI badge in README header
- `_config.yml` for Jekyll GitHub Pages (Cayman theme)
- `git submodule update --remote --merge` command in Getting Started

### Changed
- Repository Structure tree updated (added `assets/`, `.github/`, `CITATION.cff`, etc.)
- Architecture diagram rewritten with all 16 repos, RQ tags, and color-coded clusters

### Removed
- Internal research Excel file removed from git tracking (added to `.gitignore`)

---

## [v0.4.1] — 2026-03-19

### Changed
- Acknowledgements section refined (English, role-based descriptions)
- Supervisor and tutor titles corrected

---

## [v0.4.0] — 2026-03-19

### Added
- Images moved to `assets/` directory (best practice)
- Institutions & Collaborations section (Universitas Mercatorum, OPBG, BTH)
- Acknowledgements section (supervisors, institutions, hospital participants)
- GitHub Actions link checker workflow (weekly + on push)
- GitHub Pages enabled
- CHANGELOG.md
- Submodule branch tracking (`branch = main`)

### Changed
- `docs/papers/INDEX.md` enriched with titles, status, DOI
- Pinned repos on GitHub profile

---

## [v0.3.2] — 2026-03-19

### Fixed
- BTH internship end date corrected to 09/2026

### Changed
- Images stacked vertically with detailed collapsible legends (Fig. 1, Fig. 2)

---

## [v0.3.1] — 2026-03-19

### Added
- FL Algorithms section — 38 unique algorithms catalogued across 3 platforms (collapsible)
- Internships in Gantt timeline (OPBG 18mo, BTH 18mo) in red

### Changed
- At a Glance updated to 38 algorithms

---

## [v0.3.0] — 2026-03-19

### Added
- Dual title (EN primary, IT collapsible)
- Research Questions (4 RQ with cluster mapping, EN + IT)
- At a Glance metrics section
- Mermaid Gantt timeline (2023–2026)
- Datasets overview — 35 datasets across 3 platforms (collapsible)

---

## [v0.2.2] — 2026-03-19

### Changed
- Publications status updated (P-IS, P-CR, P-C2)
- Keywords refined

---

## [v0.2.1] — 2026-03-19

### Added
- Image captions for Diagram and Infographic
- Keywords section (16 research topics)

---

## [v0.2.0] — 2026-03-19

### Added
- Badges (license, submodules, papers, last commit)
- Publications table with full titles, venues, status, DOI
- CITATION.cff with ORCID and foundational paper BibTeX
- Author section (ORCID, Google Scholar, ResearchGate, website)
- Architecture diagram (Mermaid) in `docs/architecture.md`
- Papers INDEX.md
- CONTRIBUTING.md
- FENITH Diagram and Infographic in README

### Fixed
- Clone URL corrected (FENITH → FENITH2)

---

## [v0.1.7] — 2026-03-19

### Added
- Centered FENITH logo and link to www.fenith.org in README header

---

## [v0.1.6] — 2026-03-19

### Changed
- CIDE2 grouped with CIDE in Applications table

---

## [v0.1.5] — 2026-03-19

### Added
- DHFLPL2 (systematized) and DHFLPL (original/legacy) submodules in Foundations
- Seminal paper P-M MDPI 2024 (21 citations) linked

---

## [v0.1.4] — 2026-03-19

### Changed
- CIDE description refined: Federated Learning Health Data Platform

---

## [v0.1.3] — 2026-03-19

### Added
- CIDE2 submodule (XFL deepfake detection)
- P-C2 publication linked to CIDE2

### Changed
- CIDE description updated to reflect actual paper content

---

## [v0.1.2] — 2026-03-19

### Changed
- Reordered Applications table for consistency

---

## [v0.1.1] — 2026-03-19

### Changed
- P-M linked to Foundations with citations count
- P-C2 decoupled from CIDE, marked as TBD

---

## [v0.1.0] — 2026-03-19

### Added
- Initial meta-repository structure
- 13 Git submodules (platforms, applications, governance, foundations)
- README.md with project overview and publication mapping
- LICENSE (CC BY-NC-SA 4.0)
- .gitignore
- `docs/thesis/` — 5 thesis documents
- `docs/papers/` — 11 paper PDFs
- `docs/questionnaire/` — 15 survey materials
