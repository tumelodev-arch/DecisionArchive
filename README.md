# Decision Archive

A local-first Architecture Decision Record workspace for preserving context, alternatives, rationale and consequences.

**Live demo:** https://tumelodev-arch.github.io/DecisionArchive/

## What it does

- Create, edit and delete decision records.
- Track proposed, accepted, superseded and rejected decisions.
- Capture context, rationale, alternatives, consequences, dates and tags.
- Search and filter by status or engineering area.
- Export Markdown and back up or restore validated JSON.

## Run locally

Open `index.html` in a modern browser. The application uses local HTML, CSS and JavaScript and has no build step or external runtime dependency.

## Data and privacy

Records stay in the current browser until exported or cleared. They are not sent to a server or shared across browsers. The archive is local to the current browser. It has no sign-in, shared workspace, cloud sync or access control. Review Markdown before adding it to a public repository. Do not store employer-confidential decisions or sensitive data.

## Tests

The repository includes Playwright end-to-end tests. Install dependencies and Chromium before running them.

```bash
npm install
npx playwright install chromium
npm run test:e2e
```

## Interface design

The interface uses the shared Engineering Field Notes design language, adapted for this app's main task. Primary controls have labelled actions, the mobile layout keeps actions reachable, and keyboard focus is visible. The app uses its own accent colour to make it recognisable beside the portfolio.

## Limitations

This is a browser-based practice application. A successful static deployment does not establish that it has a backend, authentication, shared state or production monitoring.
