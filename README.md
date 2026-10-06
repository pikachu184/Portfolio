# pikachu184 — Developer Portfolio

A responsive, accessible portfolio for the public GitHub profile at [github.com/pikachu184](https://github.com/pikachu184). Repository cards and public profile statistics load from GitHub's unauthenticated public API. The site uses plain HTML, CSS, and JavaScript, with no build step or runtime dependencies.

## Requirements

- A modern browser
- A static file server for local development (optional but recommended)

## Run locally

Open `index.html` in a browser, or serve the folder with any static server. For example, with Node.js installed:

```sh
npx serve .
```

Then open the local URL printed by the server.

## Development

Edit `index.html`, `styles.css`, and `app.js`. The account handle is set in `app.js` as `USERNAME`. The portfolio intentionally displays only public GitHub data and does not claim experience, education, credentials, contact details, or skills that were not supplied.

## Production build

There is no compilation step. The production site consists of the static files in this repository. Before deploying, open the site in a browser and confirm the GitHub API can load the profile and repository cards. GitHub may apply unauthenticated API rate limits; the page shows a graceful fallback when data is unavailable.

## Deploy to Vercel

1. Import this repository in [Vercel](https://vercel.com/new).
2. Select **Other** as the framework preset.
3. Leave the build command and output directory empty (the repository root is served as static files).
4. Deploy.

The included `vercel.json` configures clean static hosting and security headers. No environment variables or secrets are required.

## Files

- `index.html` — semantic page structure and metadata
- `styles.css` — responsive dark theme, layout, and reduced-motion support
- `app.js` — accessible mobile navigation and public GitHub API integration
- `favicon.svg` — lightweight site icon
