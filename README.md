# Birthday Wishes, Made Personal

A responsive birthday-wish request page. Visitors provide the recipient's name, birthday, relationship, preferred tone, and a personal detail; the page updates a preview as they type.

## Request Delivery

The site is static and does not store submissions or include a server-side form handler. Submitting prepares an email draft to the platform owner. The visitor must review and send it in their email app. No details are sent automatically.

## Deploy

The GitHub Actions workflow publishes the contents of `site/` to GitHub Pages whenever a commit is pushed to `main`. In the repository's Pages settings, select **GitHub Actions** as the deployment source.

## Local Preview

Open `site/index.html` in a browser. The form handoff uses the visitor's configured email application.