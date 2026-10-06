# Site LSF Énergie (maquette)

Maquette du nouveau site lsf-energie.fr : une page HTML autonome (`index.html`), sans étape de build.

## Déploiement

Hébergé sur Cloudflare Pages, connecté à ce dépôt GitHub : chaque push sur `main` redéploie le site automatiquement.

Réglages Cloudflare Pages :
- Framework preset : None
- Build command : (vide)
- Build output directory : `/`

## Modifier le site

Éditer `index.html`, puis :

```bash
git add index.html
git commit -m "Description du changement"
git push
```

## Non indexé

Le site de maquette n'est pas indexé par les moteurs de recherche :
- balise `<meta name="robots" content="noindex, nofollow">` dans `index.html`
- `robots.txt` qui interdit l'exploration
- en-tête `X-Robots-Tag: noindex, nofollow` posé par Cloudflare Pages via `_headers`

À retirer au moment de la mise en production sur lsf-energie.fr.
