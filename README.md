# performance-report-generator
# Performance Report Generator

A tool that turns raw psychometric data into detailed, individualized performance reports — powered by the Claude API.

## The problem

I coach founders and professionals on performance. To measure their progress, I built a proprietary model with specific indicators and metrics. Like a serious personality or performance assessment.

The model worked. Turning it into a personalized, insight-rich report for each participant did not scale. With a cohort of 200+ people and myself as the only resource, producing one meaningful report per person by hand was simply impossible.

## The solution

This app industrializes that process end-to-end:

1. **Ingest** — drop in the raw data (Excel: diagnostics, pre/post module assessments, capstone results). The app parses and structures it automatically.
2. **Compute** — it applies my proprietary performance model (ICP/IIP indices) to turn raw scores into interpretable indicators and progression metrics.
3. **Visualize** — charts render each participant's profile and pre/post progression.
4. **Generate** — the Claude API writes the narrative sections: an individualized reading of the person's journey, strengths, progression, and what it means in practice.
5. **Export** — a clean, printable report, ready to share with the participant.

## Why it matters

This is a small, concrete instance of a larger idea: **AI that multiplies what a single person can do, rather than replacing them.** The human judgment, the model, the framing, the interpretation logic, all stays mine. Claude handles the scale.

## Tech

- Single-file HTML/JS app (no backend, runs entirely in the browser)
- **Claude API** (Sonnet) for narrative generation
- SheetJS for Excel parsing, Chart.js for visualization
- The API key is entered by the user at runtime 

## Run it

Open `index.html` in a browser, enter your Anthropic API key, and drop in a data file. A demo dataset is included to try it without real data.
