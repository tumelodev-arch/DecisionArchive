# Decision Archive

A local-first Architecture Decision Record (ADR) workspace for documenting context, alternatives, rationale and consequences.

## Demo

**Hosted status:** not deployed yet. Enable GitHub Pages under **Settings → Pages → Build and deployment → Source = GitHub Actions**. After a successful deployment, the app should be available at [https://tumelodev-arch.github.io/DecisionArchive/](https://tumelodev-arch.github.io/DecisionArchive/).

**Run locally:** open `index.html` in a modern browser. The app has no build step or external runtime dependency.

## Features

- Create, edit and delete decision records.
- Track status: proposed, accepted, superseded or rejected.
- Record context, rationale, alternatives, consequences, date and tags.
- Search records and filter by status or engineering area.
- Export visible records as Markdown suitable for a repository.
- Back up and restore the complete archive as JSON with basic record validation.
- Persist the archive in browser local storage.

## Run locally

Open `index.html` in a modern browser. There is no build step or external runtime dependency. `styles.css` and `app.js` are loaded locally.

## Data and privacy

Records are stored in this browser only; they are not sent to a server or shared across browsers. Use synthetic or non-sensitive information. Clearing browser storage can remove locally saved records.

## Boundaries

The archive is local to the current browser; it has no sign-in, shared workspace, synchronization or access control. Markdown export is intended for manual review before adding a record to a public repository. Do not store credentials, customer data or employer-confidential decisions in the demo.
