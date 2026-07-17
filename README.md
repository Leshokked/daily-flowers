# Jurassic Magic — Daily Flowers

A tiny, self-contained web toy: arrange a bouquet in a Jonas Wood / Picasso room and
send it as a link. The **entire arrangement lives in the URL** (everything after the `#`),
so there's no backend, database, or build step — it's one static `index.html`.

Made for Instagram Story link stickers and DMs.

## Live site

Hosted on GitHub Pages: `https://<username>.github.io/daily-flowers/`
(or a custom domain — see below).

## How it works

- Spin the dial, tap **+** to drop flowers in the vase.
- Tap the background for a new room.
- **Download** saves a 1080×1350 PNG (Instagram Story size).
- **Share** copies a link with the whole bouquet baked in — paste it into a Story
  link sticker or a DM. Whoever opens it sees exactly what you arranged.

## Enable GitHub Pages

1. Push this folder to a GitHub repo.
2. Repo → **Settings → Pages**.
3. Source: **Deploy from a branch** → Branch: `main` → Folder: `/ (root)` → **Save**.
4. Wait ~1 minute; the URL appears at the top of that Pages screen.

## Custom domain (optional)

To serve at e.g. `flowers.jurassicmagic.xyz`:

1. Add a file named `CNAME` to this repo containing exactly: `flowers.jurassicmagic.xyz`
2. At your DNS registrar, add a **CNAME record**: `flowers` → `<username>.github.io`
3. Back in **Settings → Pages**, enter the custom domain and enable **Enforce HTTPS**.

## Updating

Edit `index.html` and push. GitHub Pages redeploys automatically in ~1 minute.
