# Minerva Building — site web

Ce dossier contient le site Minerva Building prêt à être publié avec **GitHub Pages**.

## Publication sur GitHub Pages

1. Créez un dépôt GitHub, par exemple `minerva-building`.
2. Décompressez ce dossier sur votre ordinateur.
3. Déposez `index.html` (et ce fichier `README.md`) à la racine du dépôt.
4. Sur GitHub, ouvrez **Settings → Pages**.
5. Dans **Build and deployment**, choisissez **Deploy from a branch**.
6. Sélectionnez la branche `main` et le dossier `/ (root)`, puis cliquez sur **Save**.
7. Attendez la fin du déploiement. GitHub affichera l’adresse publique du site dans la section Pages.

## Éléments à connaître avant la mise en ligne

- Le site est conçu en HTML/CSS/JavaScript intégré dans `index.html`. Les images sont intégrées au fichier HTML : aucun dossier d’images séparé n’est nécessaire.
- Les polices Google Fonts sont chargées depuis Internet. Le site reste utilisable si elles ne sont pas accessibles, avec des polices de remplacement.
- Le formulaire de candidature envoie les messages et CV à `Ste.minervabuilding@gmail.com` via FormSubmit. Lors du premier envoi, FormSubmit peut demander une confirmation d’activation envoyée à cette adresse. Faites un test après activation.
- Le bouton de demande de devis renvoie vers le formulaire Google Forms déjà indiqué dans le code.
- Le site essaie de charger `market.json` pour afficher des données de marché. Ce fichier n'est pas indispensable : en son absence, le bandeau conserve son contenu de base. Si vous souhaitez alimenter ce bandeau, ajoutez ultérieurement un fichier `market.json` à la racine du dépôt, avec cette structure :

```json
{
  "updated": "2026-11-04",
  "items": [
    { "k": "masi", "v": "12 345,67", "c": 0.42 }
  ]
}
```

Les clés de marché prévues dans le code sont notamment `masi`, `bat`, `cim`, `steel`, `cu`, `al`, `au`, `usd` et `eur`. Les valeurs doivent être vérifiées et mises à jour par l'entreprise.

## Contrôles recommandés avant diffusion

- Vérifier le numéro WhatsApp, l'adresse e-mail, l'adresse Google Maps et les liens sociaux.
- Tester les trois langues (français, anglais, arabe), l'affichage mobile, les galeries et les formulaires.
- Vérifier que les photos et illustrations utilisées peuvent être publiées par l'entreprise.
- Ne pas ajouter de mots de passe, clés API ou informations confidentielles dans le dépôt public.
