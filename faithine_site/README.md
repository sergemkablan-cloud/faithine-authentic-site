
# Faithine Authentic — Site statique (gratuit)

Ce dossier contient le mini‑site prêt à déployer pour vérifier les cartes **by Faithine**.

## Déploiement gratuit (2 options)

### A. GitHub Pages
1. Crée un dépôt `faithine-authentic` sur GitHub.
2. Uploade l’intégralité de ce dossier à la racine.
3. Dans **Settings → Pages**, choisis **Deploy from branch** (branche `main`, dossier `/root`).
4. Ton site sera disponible sur `https://<ton_pseudo>.github.io/faithine-authentic/`.

### B. Netlify (recommandé)
1. Va sur https://app.netlify.com/ et clique **New Site from Git**.
2. Connecte ton repo GitHub, build settings: *Static*, pas de build command.
3. Publie → tu obtiendras une URL du type `https://faithine.netlify.app`.
4. (Optionnel) Connecte ton domaine `faithine.cards` à Netlify.

## Comment ajouter une nouvelle carte
- Ajoute une entrée dans `data/cards.json` avec un **id** unique (ex: `ROBIN026`), le **personnage**, le **numéro**, l’URL de l’image.
- Crée le QR avec le lien : `https://<ton_domaine>/verify/?id=<ID>`
- Imprime ce QR sur le sticker holographique.

## Où changer les images
- Remplace les URLs `image_url` dans `data/cards.json` par tes vraies images hébergées (Netlify, GitHub, ou un CDN).

## Styles & logo
- Le style global est dans `assets/styles.css`.
- Le logo vectoriel est `assets/logo-faithine.svg` (modifiable dans Illustrator/Figma).

## Données d’impression (VDP)
- Utilise `data/cards.csv` pour imprimer les stickers numérotés : chaque ligne contient l’ID, le personnage, le numéro d’édition et l’URL de vérification.

— © 2025 by Faithine — Authentic Edition
