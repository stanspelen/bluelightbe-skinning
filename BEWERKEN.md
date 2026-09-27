# Hoe pas je de site aan?

Alles is bewust eenvoudig gehouden. Geen build-stap: open de HTML-bestanden en pas aan.

## 1. Foto’s vervangen (belangrijkste)

| Map | Gebruik |
|-----|--------|
| `assets/skins/fs19/` | FS19 screenshots |
| `assets/skins/fs22/` | FS22 screenshots |
| `assets/skins/fs25/` | FS25 screenshots |
| `assets/skins/belgiepd/` | BelgiëPD skins |
| `assets/skins/fivem/` | Overige FiveM skins |
| `assets/logo.png` | Jouw logo (navigatie) |
| `assets/belgiepd-logo.png` | BelgiëPD logo |

**Stappen:**
1. Zet jouw screenshot in de juiste map (bijv. `police.jpg`)
2. Open de HTML-pagina (bijv. `belgie-pd.html`)
3. Zoek: `src="assets/skins/belgiepd/police.svg"`
4. Verander naar: `src="assets/skins/belgiepd/police.jpg"`

Tip: zelfde bestandsnaam houden = alleen de extensie aanpassen in de HTML.

## 2. Nieuwe skin-kaart toevoegen

Kopieer in de HTML een bestaand `<article class="project-card">...</article>` blok en plak het eronder. Pas aan:

- `src="..."` → jouw afbeelding  
- `<h3>...</h3>` → titel  
- `<p>...</p>` → beschrijving  
- `href="#"` → download/preview link  

## 3. Teksten

| Bestand | Wat je aanpast |
|---------|----------------|
| `index.html` | Home, hero, intro |
| `over-mij.html` | Over jou |
| `fs19.html` / `fs22.html` / `fs25.html` | FS skins |
| `belgie-pd.html` | BelgiëPD (geen shop) |
| `fivem.html` | Overige FiveM + commissies |
| `contact.html` | Contacttekst + Formspree |

## 4. Contactformulier (e-mail blijft verborgen)

1. Account op https://formspree.io  
2. Nieuw form → koppel jouw e-mail daar  
3. In `contact.html` vervang `YOUR_FORM_ID` in:
   `action="https://formspree.io/f/YOUR_FORM_ID"`

## 5. Online zetten (GitHub Pages)

Repo: https://github.com/stanspelen/bluelightbe-skinning  

1. GitHub → Settings → Pages  
2. Source: **Deploy from a branch** → `main` → `/ (root)`  
3. Site: `https://stanspelen.github.io/bluelightbe-skinning/`

Na een push is de site binnen 1–2 minuten live.
