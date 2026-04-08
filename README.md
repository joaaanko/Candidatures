# Modification fluide d'éléments de candidature

Ce projet permet de maintenir facilement un CV à jour, de le générer, puis de l’archiver automatiquement selon une structure organisée par entreprise et par date.

## Structure

Voici l'arborescence du dosser `CV/` :

``` bash
.
├── CV_Ko_Joan.Rmd        # Source principale du CV (R Markdown)
├── cv.css                # Feuille de style pour la mise en forme du CV
├── favicon.ico           # Icône utilisée lors du rendu HTML/PDF
├── output/
│   └── [entreprise]/     # Dossier par entreprise ciblée
│       └── [AAAA-MM]/    # Version du CV par date (année-mois)
│           └── cv.pdf    # CV généré pour cette candidature
└── README.md             # Documentation du projet
```

## Utilisation

1.  Modifier le contenu de `CV/CV_KO_Joan.Rmd` (sentez-vous libre de modifier les noms des fichiers) pour que le CV soit **complet**, quitte à tenir sur plusieurs pages.
2.  Sauvegarder et knitter (sur Rstudio on peut activer le knitting automatique lors de la sauvegarde)

L'exécution du script réalise une sauvegarde à la même racine que le CV en `.pdf` et `.html` une copie du fichier `.Rmd`utilisé.

Ainsi, pour modifier par conséquent les CV pour les diverses entreprises, il suffit de prendre le CV complet et commenter les lignes que l'on souhaite enlever.

Le but est que l'intégralité de ce qui peut être mis dans le CV reste dans le fichier `CV/CV_KO_Joan.Rmd` et qu'on commente des lignes pour ajuster son CV pour les différents besoins des différentes entreprises.

## TODO

-   [ ] mettre `output/` une arborescence au dessus

-   [ ] Faire code pour lettres de motivation
