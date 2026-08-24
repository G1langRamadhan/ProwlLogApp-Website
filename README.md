# ProwlLog — Website

Landing page, Terms of Service, and Privacy Policy for **ProwlLog** — a cat-spotting app
where you pin the cats you meet on a map, snap their photos, and build a CATalog.
Plain static HTML/CSS — no build step, no dependencies.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Landing page (hero, features, how it works, pricing, support, footer) |
| `terms.html` | Terms of Service |
| `privacy.html` | Privacy Policy |
| `styles.css` | Shared styles |

## Preview locally

Open `index.html` in a browser, or run a tiny server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Host on GitHub Pages

1. Create a new repository and push these files to the `main` branch:

   ```bash
   git init
   git add .
   git commit -m "ProwlLog website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo>.git
   git push -u origin main
   ```

2. On GitHub: **Settings → Pages → Build and deployment**.
3. Set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`, then **Save**.
4. Your site goes live at `https://<your-username>.github.io/<repo>/` within a minute or two.

### Custom domain (optional)

Add a `CNAME` file containing your domain (e.g. `prowllog.app`) and configure the DNS
records shown in **Settings → Pages**.

## Editing

- Update the "Last updated" dates at the top of `terms.html` / `privacy.html` whenever you change them.
- Replace the `Download on the App Store` link (`href="#"` in `index.html`) with your real App Store URL once the app is live.
- Prices in the copy reflect the current in-app offering: **ProwlLog Pro** at $4.99/year (3-day free trial)
  and **Nine Lives** lifetime at $14.99. Keep these in sync with `ProwlLog.storekit` if they change.
