# Site de dessins & commissions

Page de présentation avec les réseaux, un diaporama de dessins et une page de commissions avec les prix.

## Modifier le site

Tout se règle dans le bloc `CONFIG` au début du `<script>` dans `index.html` :

- `pseudo`, `bio`, `email`
- `reseaux` : colle le lien de chaque compte dans `url`
- `prix` : les tarifs tête / buste / corps entier, en noir & blanc et en couleur
- `commissionsOuvertes` : `true` ou `false`
- `delai` : le délai affiché
- `imagesAccueil` : les dessins qui défilent derrière le pseudo
- `dessins` : les dessins du carrousel

## Ajouter des dessins

1. Crée un dossier `images` dans le dépôt et mets-y tes dessins (jpg, png ou webp).
2. Dans `CONFIG`, indique leur chemin, par exemple :

```js
imagesAccueil: ["images/perso1.jpg", "images/perso2.jpg"],
dessins: [ { image: "images/perso1.jpg" }, { image: "images/perso3.jpg" } ],
```

Pense à réduire la taille des images (moins de 500 Ko chacune) pour que le site charge vite.

## Mettre le site en ligne

Settings → Pages → Source : « Deploy from a branch » → branche `main`, dossier `/ (root)` → Save.
Le site sera disponible à l'adresse `https://<ton-pseudo-github>.github.io/<nom-du-depot>/`.
