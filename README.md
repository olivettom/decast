# La DecAst – Stuffs & épreuves TESO

Petite application web (PWA) pour consulter rapidement, depuis un téléphone ou un PC, les stuffs et les builds de raid de la guilde **La DecAst** (*The Elder Scrolls Online*, PS5-EU), ainsi que les sets des 14 épreuves.

**👉 Application : https://olivettom.github.io/decast/**

## Fonctionnalités

- **Recherche instantanée** par set (en français ou en anglais), épreuve (`vDSR`, `vLC`…), zone, classe ou rôle.
- **Filtres rapides** : Tank, Heal, DD, Support, Épreuves, Farm prio.
- **Fiches de build** par classe : gameplay, ultimes, maîtrises de classe, équipement pièce par pièce (traits, poids, enchantement, set).
- **Fiches « Stuffs à farmer »** par rôle, par ordre de priorité.
- **Fiches des 14 épreuves** : zone et sets, avec 🔥 (méta prioritaire) et ⭐ (fort) quand la feuille de guilde les signale.
- **Bouton « Copier pour Discord »** sur chaque fiche.
- **Fonctionne hors-ligne** une fois installée.

## Installer sur le téléphone

1. Ouvrir le lien ci-dessus dans **Chrome** (Android).
2. Toucher **« Installer l'application »** (ou menu ⋮ → *Installer l'application* / *Ajouter à l'écran d'accueil*).
3. Ouvrir l'appli une fois avec du réseau pour activer le mode hors-ligne.

Sur iPhone : Safari → Partager → *Sur l'écran d'accueil*.

## Contenu et limites

Les stuffs sont **à titre indicatif** : c'est une cible, pas une obligation. Faites au mieux avec ce que vous avez.

Les données viennent de la feuille « La Decast – Stuff pour tous » (à jour pour la U52). Certaines fiches sont incomplètes dans la feuille et le sont donc aussi ici :

- Heal Arcaniste : aucun set renseigné.
- Heal Gardien : sets de tête, épaules, bijoux et armes non renseignés.
- Gardien tank : maîtrise de classe 2 non renseignée.
- Templier, Loup-garou, Lame noire, Sorcier DPS : pas encore de fiche.

Les noms français des épreuves et de leurs sets viennent d'ESO-Hub (en partie traduit automatiquement) et peuvent différer légèrement du jeu. Pour la Cage d'Ossein, les noms anglais ne sont pas indiqués.

Pour toute question ou précision, voir un officier de La DecAst.

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `index.html` | L'application complète (HTML, CSS et JavaScript, sans dépendance) |
| `sw.js` | Service worker pour le mode hors-ligne |

## Mettre à jour

1. Modifier `index.html` (les données sont en haut du bloc `<script>`).
2. Si le contenu change, augmenter le numéro de version dans `sw.js` (`decast-u52-v2` → `v3`) pour que les téléphones rechargent la nouvelle version.
3. GitHub Pages republie en une à deux minutes.

## Crédits

- Contenu des stuffs : feuille de guilde La DecAst.
- Noms français des épreuves et sets : [ESO-Hub](https://eso-hub.com/fr).
- *The Elder Scrolls Online* est une marque de ZeniMax Media Inc. Projet de fans, non officiel.
