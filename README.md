# Madeleinne portfolio

A local, responsive portfolio based on the supplied CV, with Bogor, Indonesia as the location. The design includes the updated user-supplied portrait. No CV download is provided.

## Review locally

Run `npm run dev` (or `node server.mjs`) and open http://127.0.0.1:5173. No dependency installation is needed. The server binds only to this computer and serves only the dist folder. You can also open dist/index.html directly, although clipboard access depends on your browser.

## Files

- dist/index.html: profile, experience, education, and contact content
- dist/styles.css: desktop and mobile layouts
- dist/app.js: mobile navigation and copy-email interaction
- dist/assets/madeleinne.jpg: updated portrait supplied as img_mad.jpeg
- server.mjs: local preview server

Run `npm run check` for JavaScript syntax checks.

The original CV stays outside the served folder and is ignored by Git. The website omits the home street address, birth date, and marital status. Contact uses the email address supplied in the CV.

## Deployment

The repository is `deleinne/madelPortfolio`; `jczx` contributes as a collaborator. The workflow in `.github/workflows/deploy.yml` publishes only `dist/` to GitHub Pages on pushes to `main`, or when run manually.

Before the first deployment, create the repository and select **Settings → Pages → Build and deployment → Source → GitHub Actions**. The repository requires access from the connected GitHub account before the initial push. A successful deployment run reports the live URL.

Workflow reference: https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
