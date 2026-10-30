# Constellation Engineering Command Center

A static, GitHub Pages-ready interactive prototype for a Lead Software Engineer role. Includes digital product delivery dashboards, Azure architecture, data-product workflows, quality gates, team planning, and an offline local knowledge-base assistant.

## Deploy to GitHub Pages
1. Create a public GitHub repository and upload the contents of this folder to its root.
2. In **Settings → Pages**, select **Deploy from a branch**, then `main` and `/ (root)`; save.
3. Visit `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY/` after the deployment finishes.

Alternatively, the included `.github/workflows/deploy.yml` can deploy using GitHub Actions. In Settings → Pages, choose **GitHub Actions** as the source.

## Run locally
Open `index.html` directly, or run `python -m http.server 8080` and visit `http://localhost:8080`.

## Assistant model
The built-in assistant is **offline and deterministic**, answering from a curated knowledge base and offering guided workflows. It is not connected to a live LLM, company systems, or operational energy infrastructure. For production generative AI, add an authenticated backend proxy to Azure OpenAI/AI Foundry; never place an API key in browser JavaScript or GitHub Pages.

## Scope and security
All metrics, work items, incidents, and organizations in this demo are **illustrative synthetic data** and are not Constellation internal data. This is an independent portfolio/demo project and is not an official Constellation product. Browser localStorage persists demo work items and conversations on the device only. No external calls or analytics.
