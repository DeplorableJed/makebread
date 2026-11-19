# Make Bread — makebread.org

The website for **Make Bread**, a 501(c)(3) nonprofit in Kirkland, WA that teaches teens and young adults how to invest safely, harness compounding and build real wealth.

## What's here

| Path | What it is |
|---|---|
| `index.html` | The whole homepage — one static HTML file, styles inline |
| `assets/` | Illustrations, logo and icons |
| `Dockerfile`, `Caddyfile` | Serves the site with Caddy on Railway |
| `railway.json` | Tells Railway to build from the Dockerfile |

## Editing the site

1. Edit `index.html` (or swap images in `assets/`).
2. Commit and push to `main`.
3. Railway picks up the push and redeploys automatically — usually live in a minute or two.

## Donation links

All giving buttons point to Stripe:

- One-time: `https://buy.stripe.com/00wbJ045j8vX8lFbxffAc00`
- Monthly $10 / $25 / $50 / $100: see the "Ways to give" section in `index.html`

Checks: Make Bread, 12010 NE 97th St., Kirkland, WA 98033

## Run it locally

```bash
docker build -t makebread . && docker run -p 8080:8080 makebread
# then open http://localhost:8080
```

Or simply open `index.html` in a browser.
