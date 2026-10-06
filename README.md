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
