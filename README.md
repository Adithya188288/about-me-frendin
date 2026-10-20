# About Me

Personal site for Adithya Santhosh: who I am, what I've built, how I work, and
why Fredrin interests me. Plain static HTML and CSS — no build step, no
framework, no backend, no analytics.

Created with [Fredrin](https://fredrin.com).

## Files

| File | What it is |
|---|---|
| `site/index.html` | All page copy and structure. Edit text here. |
| `site/styles.css` | Layout, type, colour (accent is `--accent`), motion. |
| `site/fonts/` | Self-hosted Geist and Geist Mono (SIL Open Font License). |

## Run it locally

Any static file server works:

```sh
python3 -m http.server 4173 --directory site
# open http://localhost:4173
```

## Deploy

There is nothing to build. The site lives in `site/`; everything else in the repo
(README, AGENTS.md) stays out of the deployment.

**Cloudflare Pages**

1. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git.
2. Pick the `about-me-frendin` repository and the `main` branch.
3. Framework preset: **None**. Build command: leave empty. Build output directory: `site`.
4. Save and deploy. Every push to `main` redeploys; other branches get preview URLs.

**Any other static host** (Netlify, Vercel, GitHub Pages): publish the `site`
folder with no build command.
