# Brew & Bloom — demo website

**Live demos:**
- Cloudflare Pages (main): https://drinkbrewandbloom.pages.dev/
- Cloudflare Pages (older): https://brew-and-bloom-demo.pages.dev/
- GitHub Pages: https://saadahmed-pixel.github.io/brew-and-bloom-demo/

A static, responsive 5-page demo site. No build step, no server code, no database — just HTML, CSS, images and a little browser JavaScript.

## What's in this folder

| File | What it is |
| --- | --- |
| `index.html` | Landing page (home) |
| `why-us.html` | Why us |
| `story.html` | Our story |
| `menu.html` | Menu / "Order now" destination |
| `commercial.html` | Bonus animated canvas commercial (not linked in the nav) |
| `styles.css` | All shared styling |
| `assets/` | Photos and commercial stills |
| `favicon.svg` | Browser tab icon |
| `coffee-store-demo.zip` | Zipped copy of the site, handy for uploading |

> **Demo behaviour:** the newsletter forms only show a thank-you message. Nothing is stored and no emails are sent. Buttons like "Shop the roast" link to the menu page. This is intentional for a demo.

---

## Option A — Netlify Drop (fastest, no account needed to start)

1. Open **https://app.netlify.com/drop** in your browser.
2. Drag the whole **`coffee-store`** folder from File Explorer onto the dashed box.
   - (You can also click "browse" and select the folder. If your browser asks for a ZIP, use `coffee-store-demo.zip` instead.)
3. Wait a few seconds. Netlify publishes the site and gives you a URL like `https://random-name.netlify.app`.
4. Click the URL — your demo is live.
5. **Optional:** create a free account and click *"Claim site"* so the URL doesn't expire and you can edit it later.

To update the site later: drag the folder again (or, after claiming it, use *Deploys → Drag & drop a folder*).

---

## Option B — Vercel (free, needs a GitHub account)

1. Create a free account at **https://github.com** and a new repository (e.g. `brew-and-bloom-demo`).
2. Upload all files from this folder into that repo (GitHub web UI: *Add file → Upload files* — select everything, including `assets/`).
3. Create a free account at **https://vercel.com** and choose *Continue with GitHub*.
4. Click **Add New → Project**, import your repo, and click **Deploy** (no settings needed — it detects plain HTML).
5. You get a live URL such as `https://brew-and-bloom-demo.vercel.app`.

To update later: edit/upload files in GitHub — Vercel redeploys automatically.

---

## Option C — GitHub Pages (free, GitHub only)

1. Create a GitHub repo named anything you like (e.g. `brew-and-bloom-demo`).
2. Upload all files from this folder to the repo's **main** branch. `index.html` must be at the root.
3. In the repo, go to **Settings → Pages**.
4. Under *Build and deployment*, set **Source: Deploy from a branch**, then choose **main** and **/ (root)**. Save.
5. After ~1 minute your site is live at `https://<your-username>.github.io/<repo-name>/`.

To update later: push/upload changes to the repo.

---

## Preview on your own computer first

In this folder, run one of these:

```bash
# Python 3
python -m http.server 8000
```

or open the folder in VS Code and use the **Live Server** extension.

Then visit **http://localhost:8000**. (Opening `index.html` directly also works, but a local server behaves most like the real host.)

---

## Optional extras

- **Custom domain:** all three hosts let you add a domain you own in their settings (Netlify/Vercel also provide free HTTPS).
- **Turn the demo into a real shop:** that needs a backend, product database, payments and real form handling — a separate project. This folder is deliberately demo-only.
