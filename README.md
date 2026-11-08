# Birthday Wishes, Made Personal

A responsive birthday-wish request page. Visitors provide the recipient's name, birthday, relationship, preferred tone, and a personal detail; the page updates a preview as they type.

## Request Delivery

The site is static and does not store submissions or include a server-side form handler. Submitting prepares an email draft to the platform owner. The visitor must review and send it in their email app. No details are sent automatically.

## Deploy

The GitHub Actions workflow enables Pages if needed and publishes the contents of `site/` whenever a commit is pushed to `main`. The deployment source should be **GitHub Actions** in the repository's Pages settings.

## Local Preview

Open `site/index.html` in a browser. The form handoff uses the visitor's configured email application.