# Contributing & Weekly Cadence

This archive grows on a recurring schedule. The goal is that adding a new report is a mechanical, repeatable drop — never a redesign.

## Naming convention

All report files are dated `YYYY-MM-DD` prefix so they sort chronologically in any file browser.

| Type | Directory | Pattern |
|---|---|---|
| Daily briefing | `reports/daily/` | `YYYY-MM-DD-daily-briefing.md` |
| Weekly momentum scan | `reports/weekly/` | `YYYY-MM-DD-<slug>.md` |
| Landscape / deep report | `reports/landscape/` | `YYYY-MM-<slug>.md` |
| Data feed | `data/` | `<slug>-YYYY-MM-DD.csv` |

Use the report's **publication date** for daily/weekly, and the **window-end date** when a report spans a range.

## Weekly drop checklist

1. **Add the file** to the correct `reports/` subdirectory using the naming pattern above.
2. **Link it in the README** under the matching section table (newest at the bottom of the table, or top — keep it consistent).
3. **Update the timeline data** if the report introduces datable events: add entries to the `EVENTS`, `NARRATIVE_THREADS`, or `ENTITIES` arrays in [`timeline/AITimeline.jsx`](timeline/AITimeline.jsx), then regenerate `index.html` (see below).
4. **Record the addition** in [`CHANGELOG.md`](CHANGELOG.md) with the date.
5. **Commit** using a conventional-commit message, e.g. `docs(daily): add 2026-06-20 horizon scan`.

## Regenerating the timeline (`index.html`)

`index.html` is generated from `timeline/AITimeline.jsx` so the JSX stays the single source of truth. After editing the JSX, rebuild:

```bash
python3 scripts/build_timeline.py
```

This strips the React import, wraps the component with the CDN-loaded React/Babel runtime, and writes a standalone `index.html` that requires no build toolchain.

## What does NOT go in this repo

The prompt systems, scan engines, and research playbooks that generate these reports are maintained privately. Only the finished intelligence products (reports, data, timeline) are published here.
