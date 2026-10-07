# Le Billot & le Square

Prototype Astro de six pages commerciales, avec deux emplacements complémentaires pour les informations légales. Identité provisoire. Aucun achat en ligne.

## Installation

Node.js 22.12 ou supérieur (Node 24 recommandé).

```sh
npm install
npm run dev
```

Pour générer le site : `npm run build`. Résultat dans `dist`.

## Ajouter au dépôt GitHub

Extraire l’archive. Dans le dépôt `GuilhemVR/testbillotetsquare`, sélectionner Add file puis Upload files. Déposer le contenu du dossier du projet, notamment `package.json`, `astro.config.mjs`, `src` et `public`, à la racine du dépôt. Ne pas téléverser le ZIP lui-même ni créer un niveau de dossier supplémentaire. Le README peut remplacer la présentation initiale. Ne jamais déposer node_modules.

## Cloudflare Pages

Connecter uniquement le dépôt `testbillotetsquare`. Branche : main. Commande de construction : `npm run build`. Dossier de sortie : `dist`. Racine : vide. Node : 24 (variable NODE_VERSION si nécessaire).

Un sous-domaine pages.dev permettra de consulter le prototype sans domaine personnalisé. Le site sera accessible publiquement à cette adresse sauf configuration d’une protection Cloudflare Access. Dépôt privé ne signifie pas site privé.

## État du prototype

- Accueil, deux boutiques, produits, maison, carte de saison.
- Menu responsive et déroulant des boutiques accessible au clavier.
- Photo d’ouverture originale manquante : fond temporaire, emplacement explicitement indiqué.
- Les photographies de façades ne sont disponibles que dans la maquette globale : emplacements neutres en attendant les originaux ou les nouvelles prises de vues.
- Photos de produits IA exclues.
- Appels et itinéraires désactivés : aucune coordonnée non vérifiée n’est utilisée.
- Catégories et textes à confirmer avec Alain.
- Aucun compte Instagram inventé, aucune carte ou prix inventés.
- Les pages légales sont des emplacements, pas des textes finalisés.
- Le prototype demande aux moteurs de ne pas l’indexer (meta, robots.txt, _headers). Cela ne constitue pas une protection d’accès. Retirer ces consignes lors de la publication définitive.

## Fichiers à modifier

`src/layouts/Layout.astro` : en-tête et pied de page.
`public/style.css` : apparence et adaptations mobile.
`src/pages/` : contenu de chaque page.
`public/` : emplacement des futures photographies et de la carte PDF.

Avant publication : confirmer identité, domaine, photos, textes, coordonnées, carte, mentions légales et confidentialité ; activer les liens de contact ; contrôler à nouveau le site et obtenir l’accord client.

## Vérification réalisée

Compilation Astro réussie : 8 pages générées. Liens internes contrôlés. La vérification visuelle dans un navigateur reste à effectuer : le navigateur de test n’a pas pu être installé dans cet environnement.
