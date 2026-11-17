# Birthday Celebration

A responsive, single-page birthday-wish request experience. The visitor enters
details about the recipient and receives an on-page preview of the requested
wish before choosing whether to pass the request along.

## Visitor experience

The form collects the recipient's name, birthday, relationship to the visitor,
preferred tone, and a personal detail. The preview updates in the browser as
the visitor fills in the form.

Submitting does **not** send data to a backend. Instead, the page prepares an
email draft in the visitor's configured email application. The visitor can
review, change, or discard that draft; they must explicitly send it themselves.
The repository contains no server-side submission endpoint, database, or
automatic message delivery.

## Project layout

- `site/index.html` — the website and client-side interaction
- `.github/workflows/pages.yml` — GitHub Actions workflow that publishes the
  `site/` directory to GitHub Pages on pushes to `main` or manual dispatch
- `.github/workflows/jekyll-docker.yml` — additional repository workflow

## Run locally

Open `site/index.html` in a browser. The form-to-email handoff depends on the
visitor's device having an email application configured.

## Deploy to GitHub Pages

Before the first deployment, the repository owner must enable Pages in
**Settings → Pages** and select **GitHub Actions** as the source. The workflow
then builds the static artifact from `site/` and deploys it. After enabling
Pages, run **Deploy Birthday Wishes to GitHub Pages** from the Actions tab or
push a new commit to `main`.

## Privacy and limitations

The page has no server-side storage or analytics implementation in this
repository. If the visitor elects to send the prepared email, its contents are
handled by their email provider. Review the draft before sending.