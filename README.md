# Birthday Wishes, Made Personal

A responsive birthday-wish request page. Visitors provide the recipient's name, birthday, relationship, preferred tone, and a personal detail; the page updates a preview as they type.

## Request Delivery

The site is static and does not store submissions or include a server-side form handler. Submitting prepares an email draft to the platform owner. The visitor must review and send it in their email app. No details are sent automatically.

## Deploy

Before the first deployment, the repository owner must enable Pages in **Settings → Pages** and choose **GitHub Actions** as the source. GitHub does not allow this workflow token to create the Pages site. After that one-time setting, the workflow publishes `site/` on pushes to `main`.

After enabling Pages, rerun **Deploy Birthday Wishes to GitHub Pages** from the Actions tab or push a new commit.

## Local Preview

Open `site/index.html` in a browser. The form handoff uses the visitor's configured email application.