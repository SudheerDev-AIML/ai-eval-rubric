# AI System Evaluation Rubric

A structured, interactive evaluation framework for AI-powered programs and interventions. Built for non-technical program evaluators who need to assess whether an AI system is ready for real-world deployment.

**Live demo:** [https://sudheerdev-aiml.github.io/ai-eval-rubric/](https://sudheerdev-aiml.github.io/ai-eval-rubric/)

> AI systems break a core evaluation assumption: same inputs don't always produce same outputs. This rubric helps you ask the right questions before deployment — and document your findings.

---

## What it does

Walks evaluators through six dimensions of AI readiness, collects yes/no responses against 24 evidence-based criteria, and generates a visual scorecard you can print or share.

The six dimensions:

1. **Accuracy** — Does it get the right answer?
2. **Latency** — Does it respond in time for real-world use?
3. **Safety** — Does it refuse or flag when it should?
4. **Fairness** — Does it perform equally across groups?
5. **Cost** — Is it sustainable at the scale of deployment?
6. **Compliance** — Does it meet regulatory and policy requirements?

Each dimension produces a 0–4 score. The scorecard combines them into an overall readiness percentage, a hexagonal radar chart, a per-dimension breakdown, an evidence-quality reference table, and a prioritized list of gaps to address before deployment.

## Who it's for

- Program evaluators assessing AI vendors or pilots
- Foundations and funders reviewing AI-funded interventions
- Policy and procurement teams writing evaluation requirements
- Anyone who needs a structured conversation with an AI vendor

No technical AI background required.

## How to use it

1. Open the live link above (or `index.html` locally).
2. Enter the system name, deployment context, and target population.
3. Walk through the six dimensions, checking criteria your system clearly meets.
4. Review the scorecard. Print or save as PDF for your records.

All data stays in your browser. Nothing is uploaded, stored, or transmitted anywhere.

## Run locally

This is a single self-contained HTML file with zero dependencies. Either:

```bash
# Option 1: just open the file
open index.html

# Option 2: serve it locally (recommended for fonts to load reliably)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy your own copy

The app is one static file, so it works on any static host (GitHub Pages, Netlify, Vercel, S3, your own server). To fork and deploy via GitHub Pages:

1. Fork this repo or upload `index.html` to a new repo.
2. Go to **Settings → Pages**.
3. Under **Source**, choose `main` branch and `/ (root)` folder. Save.
4. Wait ~1 minute. Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

## Tech

- Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build step
- Inter font from Google Fonts
- Hexagonal radar chart drawn with the native Canvas API
- Light and dark mode via `prefers-color-scheme`
- Print-optimized stylesheet for clean PDF export

## License

MIT — use, fork, adapt, share. Attribution appreciated.

## Credits

Built by **Sudheer Kumar** for the AEA / MTI Hackathon 2026. Framework synthesized from production AI deployment experience at enterprise scale, translated into terms evaluators can use.
