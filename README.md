# Bayes' theorem — interactive

Single-page visualization of odds-form Bayes: posterior odds, likelihood ratio, and how the prior-to-posterior map bends.

## Open the live app

**GitHub Pages (already public):**

https://knuttmegg.github.io/bayes-theorem/

Open that URL on a phone or desktop browser. No install. The page is the repo-root `index.html`.

GitHub Pages is configured to publish the `main` branch from `/`. Merges to `main` update the live site.

## Host on Vercel (optional)

`vercel.json` forces a static deploy (no framework, no install/build):

1. Go to [vercel.com/new](https://vercel.com/new).
2. Import `knuttmegg/bayes-theorem`.
3. Leave Framework as **Other** (already set by `vercel.json`).
4. Deploy. Production URL will look like `https://bayes-theorem.vercel.app`.

Local CLI equivalent, from the repo root:

```bash
npx vercel
```

## GitHub Pages via Actions (optional)

The workflow in `.github/workflows/pages.yml` packages `index.html` as a Pages artifact on every push and pull request.

The site is already live from **Deploy from a branch** (`main` / `/`). To switch publishing to Actions:

1. Repo **Settings → Pages → Source → GitHub Actions**.
2. Run **Deploy GitHub Pages** from the **Actions** tab (`workflow_dispatch`).

## Local preview

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080
