# Eline Peper — CV website

Persoonlijke CV-site voor Eline Peper, verpleegkundige niveau 4.
Statische HTML/CSS-site, geen build step. Auto-deployt op Vercel via push naar `main`.

## Lokaal draaien

```bash
python3 -m http.server 8000
# of
npm run dev
```

Open daarna http://localhost:8000

## Bestanden

- `index.html` — volledige CV-pagina
- `style.css` — styling (Inter + Playfair via Google Fonts, geen build)
- `package.json` — dev script
- `vercel.json` — Vercel config

## Inhoud aanpassen

Alle inhoud staat direct in `index.html`. Bewerk gewone HTML-secties:
- Hero (boven) — naam, titel, contact, snelle stats
- Profiel
- Kernervaring (checklist)
- Werkervaring (artikels per rol)
- Opleiding
- Vaardigheden
- Relevantie LUMC
- Contact

## Deployen

```bash
git add -A
git commit -m "Update CV"
git push origin main
```

Vercel pakt push automatisch op vanuit https://github.com/robinbril/eline-cv.
