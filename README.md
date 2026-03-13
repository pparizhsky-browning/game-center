# game-center

## Netlify Deploy

This repository is preconfigured for Netlify static hosting.

1. Push this repo to GitHub.
2. In Netlify, choose `Add new site` -> `Import an existing project`.
3. Select this repo and keep build settings empty/default:
	- Build command: *(leave blank)*
	- Publish directory: `.`
4. Deploy.

### Included Netlify readiness

- `netlify.toml` at repo root with publish settings.
- Redirects for `bstars/*` -> `Bstars/*` to avoid case-sensitive path breaks.
- Long-cache headers for static assets.
- Explicit Unity/WebAssembly headers for files in `slope/Build`.
- A root `/js/main.js` shim file used by bundled game templates.
