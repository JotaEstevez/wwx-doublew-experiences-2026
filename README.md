# wowinX × doubleW — Experiences Catalog 2026

Interactive HTML catalog of immersive VR experiences for the **wowinX** ecosystem and its commercial layer **doubleW**. Built from the official 2026 Dossier, it segments the offer by client typology and structures packages, technical deliverables, lead times and customization levels for each.

> Live preview: enable GitHub Pages on this repo (see below) and the site will be served at `https://<owner>.github.io/wwx-doublew-experiences-2026/`.

---

## What's inside

- **12 VR experiences** across 5 categories (Compite · Diviértete · Entrena · Conecta · Another Reality)
- **4 client segments** with recommended packages
- **4 commercial packages**: Starter · Pro · Signature · Custom
- **Customization matrix** by package
- **Process** (5 steps, brief → activation)
- **Video modal system** ready to plug YouTube / Vimeo / MP4 URLs

## Project structure

```
.
├── index.html              # Full single-page catalog (self-contained CSS + JS)
├── assets/
│   ├── exp/                # Experience hero images (cropped from dossier)
│   ├── full/               # Full-bleed banners (ecosystem, cases, world map…)
│   └── pages/              # Original dossier page renders (reference)
└── README.md
```

No build step. No dependencies. Pure HTML + CSS + JS.

---

## Run locally

```bash
# Option 1 — any static server
npx serve .

# Option 2 — Python
python3 -m http.server 8080
```

Then open `http://localhost:8080/`.

---

## Deploy

### GitHub Pages (recommended)

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under *Source*, select **Deploy from a branch**.
4. Branch: `main` · Folder: `/ (root)` → **Save**.
5. After ~1 minute the catalog is live at:
   `https://<owner>.github.io/wwx-doublew-experiences-2026/`

> **Private repos:** GitHub Pages on private repositories requires GitHub Pro / Team / Enterprise. On the Free plan, switch the repo to public to expose the Pages URL.

### Other hosts

The site is 100% static — drop the folder into Netlify, Vercel, Cloudflare Pages, or any S3 + CloudFront setup. No build command needed.

---

## Connect the videos

Open `index.html` and locate the `VIDEOS` object near the bottom of the `<script>` block:

```js
const VIDEOS = {
  "vssoccer-1v1": "",          // paste YouTube / Vimeo / MP4 URL
  "vssoccer-ia": "",
  "vsbasket": "",
  "sp-keeper": "",
  "sp-header": "",
  "sp-rhythm": "",
  "vertigoal-foot": "",
  "vertigoal-scaler": "",
  "vertigoal-airstriker": "",
  "academy": "",
  "aidols": "",
  "bftalks": ""
};
```

Supported automatically:

- **YouTube** — `https://www.youtube.com/watch?v=XXXX` or `https://youtu.be/XXXX`
- **Vimeo** — `https://vimeo.com/123456789`
- **Direct MP4** — `https://cdn.your-domain.com/clip.mp4`

Commit and the change is live on the next Pages build.

---

## Brand & contact

**wowinX** — Infrastructure for XR, AI and Web3 experiences.
**doubleW** — Commercialization, marketing and communication layer that turns wowinX innovations into real business.

- Europe HQ — Madrid · 75 Albasanz Street
- Middle East HQ — Dubai · IFZA Business Park
- Contact — [juana.estevez@wowinx.com](mailto:juana.estevez@wowinx.com)

---

## License

© 2026 wowinX × doubleW. All rights reserved. Internal commercial use.
