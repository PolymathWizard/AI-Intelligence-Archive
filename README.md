# AI Intelligence Archive

**A standing record of the 2026 AI landscape — daily briefings, weekly momentum scans, and deep landscape analyses.**

*Human-Directed. AI-Enabled. Commercially Tested.* — [Barry Hurd Intelligence Lab (BHIL)](https://github.com/PolymathWizard)

---

This repository is a public, continuously growing archive of open-source AI intelligence products. It pairs a **written record** (briefings and reports) with an **interactive timeline** that maps how the events connect across companies, governments, and narrative threads.

New reports are appended on a weekly cadence. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the drop process and naming convention.

## ▶ The Timeline (start here)

The hero of this archive is an interactive intelligence timeline rendered from the daily and weekly record:

- **[Open the live timeline →](https://polymathwizard.github.io/AI-Intelligence-Archive/)** *(GitHub Pages)*
- Source: [`index.html`](index.html) — a standalone, zero-build page. Clone and open it directly in any browser.
- Component source: [`timeline/AITimeline.jsx`](timeline/AITimeline.jsx)

The timeline offers five lenses on the same record: a chronological **Timeline**, a **Threat Sphere** entity-relationship view, an **Entity Map**, a **Precognition** panel of forward signals, and a **Momentum** view of signal velocity.

## 📚 The Reports

### Daily Briefings — *Horizon Scans*
24-hour intelligence windows prepared for decision-makers, each with an executive narrative, scored signals, and strategic implications.

| Date | Edition |
|---|---|
| 2026-02-14 | [Daily Briefing & Horizon Scan](reports/daily/2026-02-14-daily-briefing.md) |
| 2026-02-15 | [Daily Briefing & Horizon Scan](reports/daily/2026-02-15-daily-briefing.md) |
| 2026-02-16 | [Daily Briefing — Presidents' Day Edition](reports/daily/2026-02-16-daily-briefing.md) |
| 2026-02-17 | [Daily Briefing & Horizon Scan](reports/daily/2026-02-17-daily-briefing.md) |

### Weekly Momentum — *Open-Source Velocity Scans*
Point-in-time forensic analysis of the open-source AI ecosystem: model releases, repository velocity, creators to watch, and competitive positioning.

| Window | Report |
|---|---|
| 2026-06-07 → 06-19 | [GitHub AI Momentum Command Center — Open-Weight Coding Models Breakout](reports/weekly/2026-06-19-github-momentum-command-center.md) |

### Landscape Analyses — *Deep Technical Intelligence*
Standalone, longer-form reports on a structural shift in the field.

| Period | Report |
|---|---|
| 2026-06 | [AI Skills, Agents & Harnesses — 2026 Landscape Analysis](reports/landscape/2026-06-ai-skills-agents-harnesses-landscape.md) |
| 2026-06 | [AI-Powered Second Brain Ecosystem — Technical Intelligence Report](reports/landscape/2026-06-second-brain-ecosystem.md) |

## 🗂 Data

| File | Description |
|---|---|
| [`data/cool-ai-things-2026-06-05.csv`](data/cool-ai-things-2026-06-05.csv) | Curated feed of open-source repos and open-weight model releases, with BHIL enrichment columns. See [`data/README.md`](data/README.md) for the schema. |

## 🧭 Methodology & evidence tiers

Every signal in these reports is graded against a consistent evidence-tier scheme so readers can separate confirmed fact from vendor claim and inference:

- **VERIFIED** — independently confirmed by primary sources.
- **CORROBORATED** — multiple credible sources agree.
- **STATED** — single-source or vendor-reported; not independently confirmed.
- **INFERENCE** — analyst judgment derived from available evidence.
- **CONTRADICTED** — sources conflict; flagged explicitly.

The prompt systems and engines used to *produce* these reports are maintained privately and are not included in this repository.

## Repository layout

```
AI-Intelligence-Archive/
├── index.html                 # Interactive timeline (the hero) — open directly
├── reports/
│   ├── daily/                 # Daily horizon scans  (YYYY-MM-DD-daily-briefing.md)
│   ├── weekly/                # Weekly momentum scans (YYYY-MM-DD-...md)
│   └── landscape/             # Deep landscape analyses
├── data/                      # Curated feeds (CSV) + data dictionary
├── timeline/                  # Timeline component source (AITimeline.jsx)
├── assets/                    # Shared static assets
├── CONTRIBUTING.md            # Weekly-drop cadence & naming convention
├── CHANGELOG.md               # Dated record of additions
└── LICENSE
```

## License

Report content is released under [CC BY 4.0](LICENSE) — share and adapt with attribution to Barry Hurd Intelligence Lab. The timeline code is available under the MIT terms noted in [`timeline/LICENSE`](timeline/LICENSE).
