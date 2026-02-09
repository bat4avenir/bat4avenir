# Accès PDF via QR Code (site statique)

Ce dépôt contient une page statique `index.html` qui lit un paramètre `?code=XXXX` et autorise l’accès au PDF si le code fait partie de la liste.

## Étapes rapides (GitHub Pages)

1. Mets `index.html` à la racine du dépôt.
2. Ajoute ton PDF (ex: `tonpdf.pdf`) à la racine **ou** dans un dossier (ex: `assets/`).
3. Dans `index.html`, remplace la variable `PDF_URL` par l’URL publique finale de ton PDF.
4. Active GitHub Pages : **Settings → Pages → Deploy from a branch → main / root**.

URL finale : `https://<ton-user>.github.io/<ton-repo>/?code=XXXX`

## Codes autorisés (30)

Les codes sont listés dans `codes.csv`.

## Génération des QR codes

Les images QR sont dans `qrcodes/` et encodent l’URL suivante (à compléter) :

`https://<ton-user>.github.io/<ton-repo>/?code=CODE`

Remplace le domaine dans `make_qr_base_url.txt` puis régénère si besoin.
