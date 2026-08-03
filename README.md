# Site de publication — Compresser Vidéo

Deux pages statiques, sans dépendance ni ressource externe. Elles servent
d'URL de politique de confidentialité pour la fiche Play, qui l'exige.

| Fichier | Locale de fiche Play | URL une fois déployé |
|---|---|---|
| `privacy-policy.html` | en-US (défaut) | `https://wrocketdev.github.io/video-compressor/privacy-policy.html` |
| `politique-confidentialite.html` | fr-FR | `https://wrocketdev.github.io/video-compressor/politique-confidentialite.html` |

Même dispositif que `wrocketdev/belote` : un dépôt public par application,
GitHub Pages servi depuis `main`.

## Déploiement

1. Créer un dépôt **public** `video-compressor` sur https://github.com/new
   (sans README, sans .gitignore — le contenu est déjà ici).

2. Depuis ce dossier :

```bash
git init -b main && git add -A && git commit -m "Politique de confidentialite" && git remote add origin https://github.com/wrocketdev/video-compressor.git && git push -u origin main
```

3. Activer Pages : *Settings → Pages → Source: Deploy from a branch →
   `main` / `/ (root)` → Save*. La mise en ligne prend une à deux minutes.

4. Vérifier que les deux URL répondent en 200 **avant** de les coller dans
   Play Console : une URL de politique injoignable est un motif de rejet.

## Ce que ces pages affirment

Qu'aucune donnée n'est collectée et qu'aucune connexion réseau n'a lieu.
**Cette affirmation n'est vraie qu'une fois le SDK AdMob retiré** (tâche en
cours). Si la publicité est finalement conservée en v1, ces deux pages sont
fausses et doivent recevoir les sections « publicité » et « consentement »
du modèle Belote avant toute publication — c'est une déclaration légale,
pas une formalité.
