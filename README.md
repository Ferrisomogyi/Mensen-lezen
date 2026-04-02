# Mensen Lezen — PWA

72 technieken om iedereen te doorgronden. Installeerbaar als Chrome-app.

---

## Deployen op GitHub Pages — Stap voor stap

### 1. Maak een nieuwe repo op GitHub

- Ga naar https://github.com/new
- Naam: `mensen-lezen` (of wat je wilt)
- **Public** aanvinken
- Klik **Create repository**

### 2. Upload de bestanden

**Optie A: Via de browser (makkelijkst)**

1. In je nieuwe lege repo, klik **"uploading an existing file"**
2. Sleep alle 5 bestanden erin:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. Typ een commit message (bijv. "Initial deploy")
4. Klik **Commit changes**

**Optie B: Via terminal**
```bash
cd mensen-lezen-pwa
git init
git add .
git commit -m "Initial deploy"
git branch -M main
git remote add origin https://github.com/JOUW-USERNAME/mensen-lezen.git
git push -u origin main
```

### 3. Zet GitHub Pages aan

1. Ga naar je repo → **Settings** → **Pages** (linkermenu)
2. Bij **Source**: kies **Deploy from a branch**
3. Bij **Branch**: kies **main** en **/ (root)**
4. Klik **Save**
5. Wacht 1-2 minuten

### 4. Open je app

Je app staat nu op:
```
https://JOUW-USERNAME.github.io/mensen-lezen/
```

### 5. Installeren als Chrome-app

1. Open de URL in Chrome
2. Klik op het **installatiesymbool** in de adresbalk (rechterkant, lijkt op een computertje met een pijl)
   - Of: drie puntjes → "Installeren" / "App installeren"
3. Klik **Installeren**
4. De app verschijnt nu als losse app op je desktop/telefoon

---

## Features

- 72 technieken in 7 categorieën
- Zoekfunctie
- Favorieten (lokaal opgeslagen)
- Tik op kaart om details te zien
- Willekeurige techniek knop
- Werkt offline na eerste bezoek
- Installeerbaar als Chrome/mobiele app

---

## Uitbreiden

Om technieken toe te voegen, open `index.html` en voeg een nieuw object toe aan de `T` array:

```javascript
{id:73, c:"invloed", t:"Titel van techniek", b:"Uitleg van de techniek."},
```

Categorieën uitbreiden: voeg toe aan de `CATS` array.

---

*Ferri Somogyi · Mensen Lezen v1.0*
