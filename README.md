# MSPR R — Rendu

## Contenu du dossier

Ce dossier contient l'ensemble des éléments attendus pour la livraison du rendu :

- `MSPR_R.qmd` : source Quarto du rapport
- `MSPR_R.html` : version HTML rendue
- `data/mtcars_enrichi.csv` : jeu de données utilisé
- `README.md` : consignes de reconstruction et informations de livraison

## Reproductibilité

Le rapport a été conçu pour être **rebuild sans intervention manuelle** :

- les chemins utilisés sont **relatifs** ;
- `set.seed(123)` est défini dans le document ;
- les données sont fournies dans le dossier `data/` ;
- aucune modification manuelle n'est requise avant rendu HTML.

## Reconstruction du rapport

Depuis le dossier du projet :

```bash
quarto render MSPR_R.qmd
```

Ou, si besoin, avec R :

```bash
Rscript -e "rmarkdown::render('MSPR_R.qmd', output_format = 'html_document')"
```

## Dépôt Git attendu

Dépôt GitHub :

- https://github.com/AdamSawi/R

## Archive à livrer

Le zip final doit contenir :

- `MSPR_R.qmd`
- `MSPR_R.html`
- `data/mtcars_enrichi.csv`
- `README.md`

## Remarques

Le rapport s'appuie sur le dataset `mtcars`, enrichi avec des variables métier complémentaires pour faciliter l'analyse et l'interprétation business.
