# Startup Solutions Lab prototype

A responsive, static GitHub Pages prototype demonstrating the proposed functional experience of a university-powered startup solutions lab.

## Included

- Branded public landing page
- Four-stage lab model
- Interactive demonstration sprint workspace
- Five-step founder challenge intake
- Browser-local draft persistence and printable challenge brief
- Interactive startup financial health check with Plotly
- Filterable sprint portfolio
- Student opportunity board
- Searchable toolkit
- Sample JSON data
- Accessible, responsive layout
- GitHub Actions Pages deployment

## Run locally

Because the site loads JSON through `fetch`, use a local web server rather than opening `index.html` directly.

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish on GitHub Pages

1. Create a new GitHub repository, for example `startup-solutions-lab`.
2. Upload all files and folders from this package to the repository root.
3. Commit to the `main` branch.
4. In repository **Settings > Pages**, set **Source** to **GitHub Actions**.
5. Open the **Actions** tab and verify that the deployment workflow completes.

The included workflow publishes the entire repository as a static site.

## Replace demonstration content

- Sprint cards: `data/sprints.json`
- Toolkit: `data/toolkit.json`
- Student roles: `data/opportunities.json`
- Page copy and layout: `index.html`
- Brand styling: `assets/css/style.css`
- Interactions: `assets/js/app.js`

## Privacy boundary

The intake form is intentionally front-end only. It stores an optional draft in the visitor's browser using `localStorage`. It does not transmit data. Do not add confidential startup information to the repository. A production implementation should connect intake, authentication, private project records, and document storage to institutionally approved services after governance and security review.

## Prototype notice

Names and partnership references are used for concept demonstration. Project, milestone, and opportunity data are fictional. Review institutional brand standards, accessibility, privacy, security, legal, and partnership approvals before public launch.
