# navratri_aol – Shubh Navratri Photo Booth

Static, frontend-only photo booth. Users take a photo (or upload one) inside the Navratri frame, then save or share it. No build step, no backend.

## Run locally
```
npm run dev      # or: python3 -m http.server 8000
```
Open http://localhost:8000 (camera needs HTTPS or localhost).

## Deploy to Vercel
```
npm i -g vercel
vercel            # preview
vercel --prod     # production
```
Or push to GitHub and import the repo at vercel.com/new (Framework: Other, no build command, output dir: `.`).

## Files
- `index.html` – the whole app (HTML/CSS/JS)
- `frame.jpg` – original frame (used for the saved photo)
- `frame-base.jpg`, `garland-l.png`, `garland-r.png`, `banner.png`, `garland-tile-l.png`, `garland-tile-r.png` – frame split so the garlands animate and the message banner sits on top of the photo
