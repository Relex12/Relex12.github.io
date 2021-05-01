---
layout: default
title: "Dictionaries"
permalink: fr/Dictionaries
---

# Dictionaries

Liste de dictionnaires pour Word-Machine

![](https://img.shields.io/badge/status-Up_to_date-green) ![](https://img.shields.io/github/license/Relex12/Dictionaries) ![](https://img.shields.io/github/repo-size/Relex12/Dictionaries) ![](https://img.shields.io/github/last-commit/Relex12/Dictionaries) ![](https://img.shields.io/github/stars/Relex12/Dictionaries)

Regarder sur GitHub

[![Dictionaries](https://github-readme-stats.vercel.app/api/pin/?username=Relex12&repo=Dictionaries)](https://github.com/Relex12/Dictionaries)

[Read in English](https://relex12.github.io/Dictionaries)

---

## Sommaire

* [Dictionaries](#dictionaries)
    * [Sommaire](#sommaire)
    * [Ce que c'est](#ce-que-c'est)
    * [Comment l'utiliser](#comment-l'utiliser)
    * [Licence](#licence)

<!-- table of contents created by Adrian Bonnet, see https://Relex12.github.io/Markdown-Table-of-Contents for more -->

## Ce que c'est

Ce dépôt offre une liste de dictionnaires qui peuvent être utilisés avec le générateur de mots [Word-Machine](https://relex12.github.io/Word-machine).

[![Word-machine](https://github-readme-stats.vercel.app/api/pin/?username=Relex12&repo=Word-machine)](https://github.com/Relex12/Word-machine)


## Comment l'utiliser

Si vous avez cloné les deux dépôts dans un même répertoire parent, c'est-à-dire que vous avez

```
$ tree
├── Dictionaries
│   ├── great-old-ones.txt
│   [...]
│   └── README.md
├── Word-machine
│   [...]
│   └── word-machine.py
[...]
```

alors vous pouvez taper la commande suivante

`python3 Word-machine/word-machine.py -d Dictionaries/great-old-ones.txt -g 10`

pour générer des mots semblables aux noms des Grands Anciens de H.P. Lovecraft.

## Licence

Ce projet est un petit projet. Le code source est donné librement à la communauté GitHub, sous la seule licence MIT, qui n'est pas trop restrictive.
