# Site A.P.P.L. — GitHub Pages

## Mise en ligne
1. Créez un dépôt GitHub public, par exemple `appl-site`.
2. Dans le dépôt, cliquez **Add file → Upload files**, et envoyez **le contenu décompressé du ZIP** (index.html, style.css, script.js, dossiers assets/, content/, admin/, videos/), pas le ZIP lui-même. Vous pouvez utiliser GitHub Desktop pour un envoi plus simple, surtout pour les vidéos.
3. Ouvrez **Settings → Pages → Build and deployment → Deploy from a branch**, choisissez **main** et **/(root)**, puis Save.
4. Le site sera accessible à une adresse du type `https://VOTRE-COMPTE.github.io/appl-site/` après le déploiement.

## Mise à jour sans programmation
- Pour changer les textes, projets, actualités, liens sociaux : ouvrez `content/site.json` dans GitHub → icône crayon → modifiez → **Commit changes**.
- Ou ouvrez `admin/index.html` depuis le site : chargez le fichier JSON téléchargé depuis GitHub, modifiez, vérifiez, téléchargez, puis remplacez `content/site.json` dans GitHub. **Cet éditeur n'est pas connecté à GitHub** et ne comporte pas de connexion administrateur.
- Ajouter une photo : déposer l'image dans `assets/` puis ajouter dans `galerie` une entrée telle que `{"image":"assets/ma-photo.jpg","legende":"Description validée"}`.
- Ajouter une actualité : dans `actualites`, ajouter `{"titre":"Titre","date":"2026-11-08","description":"Texte"}`.
- Ajouter un projet : dans `projets`, ajouter `{"titre":"Titre","statut":"Projet envisagé","description":"Texte"}`.
- Après chaque changement, attendre le déploiement GitHub Pages.

## Sécurité et limites
- GitHub Pages est **public et statique** : ne jamais y déposer de données de demandeurs d'aide, CIN, coordonnées privées, dossiers médicaux, clés secrètes, mots de passe ou listes de bénéficiaires.
- Les boutons de dons ne collectent **aucun paiement** tant que `don_url` n'a pas été configuré vers une plateforme vérifiée.
- Le bouton d'aide dirige vers le contact; il ne collecte **aucun formulaire confidentiel**.
- Les photos de deux adultes fournies sont incluses à la demande de l'utilisateur, mais **vérifier leur accord de publication avant mise en ligne**.
- Les vidéos sont dans `videos/`, **non affichées** tant que les droits de diffusion et leur contenu n'ont pas été vérifiés.
- Le statut juridique de l'association doit être confirmé auprès des autorités compétentes avant d'afficher une reconnaissance nationale.
- Les réseaux sociaux, e-mail et téléphone sont vides : renseigner les vrais liens dans `content/site.json`.
- Pour une véritable interface administrateur connectée, un formulaire privé, ou des paiements, prévoir un service externe sécurisé avec authentification et protection des données.
