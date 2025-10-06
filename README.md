# CIMENCAM — HSE Days (Static Page)

Cette page HTML/CSS simple affiche deux boutons : **Survey** et **Playlist**.
Elle est prête pour un déploiement gratuit sur **Vercel** (ou Netlify/GitHub Pages).

## Liens utilisés
- Survey : https://drive.google.com/file/d/1KPt32GxsKTqqp0baPmssp64oY6sXDJFu/view?usp=sharing
- Playlist (Google Drive folder) : https://drive.google.com/drive/folders/1rzs6Dtu1RGGPNfiDK9CtWUXp-FpiR5xW?usp=drive_link
- Logo : https://share.google/images/T2zsXHZMLmRbocWPF (si non valide, remplacez par une URL publique accessible)

## Déploiement sur Vercel (UI Web)
1. Créez un nouveau dépôt GitHub (ex: `cimencam-hse-days`).
2. Ajoutez `index.html` à la racine du dépôt, commit & push.
3. Allez sur https://vercel.com → **Add New… → Project** → importez le repo.
4. Framework = *Other* (ou *Static*), **Build Command** = *none*, **Output** = `/` (racine).
5. **Deploy**. L’URL publique obtenue peut être mise derrière votre **QR code**.

## Déploiement sur Vercel (CLI)
```bash
npm i -g vercel
vercel login
vercel deploy --prod
```
*(à lancer dans le dossier qui contient `index.html`)*

## QR code
- Utilisez https://qrcodemonkey.com ou https://goqr.me et collez l’URL publique Vercel.
- Option : ajoutez un logo sur le QR.

## Notes
- Google Drive doit autoriser l’accès en lecture **“Toute personne disposant du lien”**.
- Si le logo ne s’affiche pas, remplacez la valeur `src` dans `<img class="logo" src="...">` par une URL valide (Drive en partage public **ou** un hébergement public).
