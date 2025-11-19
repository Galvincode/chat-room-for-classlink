# Chat Room for Classlink

This repository hosts a simple static site that embeds a Minnit chat instance.

How the site is published
- The site files are in the `docs/` directory.
- A GitHub Actions workflow at `.github/workflows/deploy-pages.yml` automatically deploys the `docs/` folder to GitHub Pages when you push to `main`.

Site URL
- Once the workflow runs successfully, the site will be available at:

	`https://galvincode.github.io/chat-room-for-classlink/`

If you prefer to enable Pages from the repository settings instead, go to Settings → Pages and select `main` / `docs` as the source.

Editing the chat
- To edit the embedded Minnit chat, modify `docs/index.html` and update `docs/styles.css` for styles. Push changes to `main` and the workflow will redeploy the site.

Troubleshooting
- If you don't see the site after a few minutes, open the repository's Actions tab to inspect the Pages workflow run and logs.
- If the Minnit embed doesn't show up, check the Minnit dashboard to ensure the embed is allowed for the origin `https://galvincode.github.io`.
