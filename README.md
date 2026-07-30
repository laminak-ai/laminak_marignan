# 1515 — Marignan, le choc des géants

Une expérience pédagogique interactive consacrée à la bataille de Marignan et à l’avènement de François Ier.

Le projet mêle récit historique, illustrations, frise animée, reconstitution jouable en pseudo-3D, évolution simulée des effectifs, quiz et ressources pédagogiques téléchargeables.

![Aperçu de la bataille interactive](./site/assets/DemoLaminak_bataille-marignan.png)

## Découvrir l’expérience

Le parcours présente :

- l’avènement de François Ier en 1515 ;
- les ambitions françaises dans le duché de Milan ;
- le contexte politique des guerres d’Italie ;
- le déroulement des combats des 13 et 14 septembre 1515 ;
- les charges suisses, la résistance française et l’arrivée des Vénitiens ;
- la retraite suisse et les conséquences diplomatiques de la victoire ;
- un quiz de cinq questions pour vérifier les acquis.

## Bataille interactive

La reconstitution permet de suivre en direct les principales phases de l’affrontement :

- progression et formation des lignes françaises ;
- assauts des colonnes suisses ;
- pertes et effectifs estimés évoluant pendant l’animation ;
- arrivée des renforts vénitiens sur le flanc ;
- repli final des Suisses.

> Cette séquence est une reconstitution pédagogique stylisée. Les unités affichées ne représentent pas individuellement tous les combattants et les chiffres proposés restent des ordres de grandeur historiques.

### Commandes

| Action | Commande |
|---|---|
| Déplacer la caméra selon son orientation | `ZQSD` ou flèches |
| Orienter et incliner la caméra | Glisser avec la souris |
| Zoomer | Molette |
| Contrôler la simulation | Lecture, pause et rejouer |
| Agrandir la scène | Plein écran |

## Le thème royal 👑

Lors de la première visite, le bouton **« Armer le thème royal »** autorise la lecture audio. Le thème de François Ier se déclenche ensuite à l’approche des passages qui lui sont consacrés, avec un volume limité à 10 % et des fondus d’entrée et de sortie.

Cette activation manuelle initiale est nécessaire à cause des règles de lecture automatique des navigateurs.

## Ressources pédagogiques

La rubrique **Ressources** donne accès directement à :

- `Marignan-1515-Presentation.pptx` — support de cours projetable ;
- `Marignan-1515-Cours-illustre.docx` — cours illustré à consulter ou imprimer ;
- `Marignan-1515-Cahier-activites.docx` — exercices et activités.

Les fichiers sont stockés dans [`downloads/`](downloads/).

## Technologies

- HTML5 sémantique ;
- CSS3 responsive et animations ;
- JavaScript natif ;
- Canvas 2D pour la reconstitution en perspective ;
- Web Audio / élément audio HTML5 ;
- aucune dépendance externe et aucune étape de compilation.

## Lancer le site localement

Le projet peut être ouvert directement avec `index.html`. Pour un comportement identique à GitHub Pages, il est toutefois préférable d’utiliser un petit serveur HTTP local.

Avec Python :

```bash
python -m http.server 8000
```

Puis ouvrir :

```text
http://localhost:8000
```

## Publier avec GitHub Pages

1. Créer un dépôt GitHub et placer le contenu de ce dossier à sa racine.
2. Envoyer les fichiers sur la branche `main`.
3. Ouvrir **Settings → Pages** dans le dépôt.
4. Dans **Build and deployment**, choisir **Deploy from a branch**.
5. Sélectionner la branche `main`, le dossier `/ (root)`, puis enregistrer.

Le site sera ensuite disponible à une adresse de la forme :

```text
https://VOTRE-PSEUDO.github.io/NOM-DU-DEPOT/
```

Tous les chemins utilisés par le projet sont relatifs et compatibles avec un déploiement dans un sous-dossier GitHub Pages.

## Arborescence

```text
.
├── index.html
├── styles.css
├── script.js
├── battle-check.png
├── assets/
│   ├── illustrations historiques
│   └── Walen-HEADPHONK.mp3
└── downloads/
    ├── Marignan-1515-Presentation.pptx
    ├── Marignan-1515-Cours-illustre.docx
    └── Marignan-1515-Cahier-activites.docx
```

## Accessibilité et compatibilité

- navigation adaptée aux écrans mobiles et aux ordinateurs ;
- textes alternatifs sur les illustrations principales ;
- commandes clavier disponibles dans la bataille interactive ;
- interface utilisable sans activer la musique.

Un navigateur moderne est recommandé pour profiter du Canvas, du plein écran, des animations et des transitions audio.

## Crédits

- Conception pédagogique, développement et direction artistique : projet **Marignan 1515** réalisé avec Laminak.
- Musique du thème royal : **Walen — HEADPHONK**, fichier provenant de `freetouse.com`.
- Les documents proposés au téléchargement sont destinés à accompagner le cours et les activités.

## Licence

Aucune licence générale n’est déclarée pour le moment. Les illustrations, la musique et les documents pédagogiques peuvent relever de conditions d’utilisation distinctes. Vérifiez les droits applicables avant toute redistribution publique ou réutilisation commerciale.
