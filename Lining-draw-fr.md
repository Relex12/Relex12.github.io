---
layout: default
title: "Lining draw"
permalink: fr/Lining-draw
---

# Lining-draw
Script en Processing pour créer des courbes à partir de lines uniquement

![](https://img.shields.io/badge/status-Finished-green) ![](https://img.shields.io/github/license/Relex12/Lining-draw) ![](https://img.shields.io/github/repo-size/Relex12/Lining-draw) ![](https://img.shields.io/github/languages/top/Relex12/Lining-draw) ![](https://img.shields.io/github/last-commit/Relex12/Lining-draw) ![](https://img.shields.io/github/stars/Relex12/Lining-draw)



Voir sur GitHub:

[![Lining-draw](https://github-readme-stats.vercel.app/api/pin/?username=Relex12&repo=lining-draw)](https://github.com/Relex12/lining-draw)

[Lire en anglais.](https://relex12.github.io/Lining-draw)


---

## Sommaire

* [Lining-draw](#lining-draw)
    * [Sommaire](#sommaire)
    * [Qu'est-ce que c'est ?](#qu'est-ce-que-c'est-)
    * [À quoi ça ressemble](#à-quoi-ça-ressemble)
    * [Comment l'utiliser](#comment-l'utiliser)
    * [Explication du code](#explication-du-code)
    * [Ce que vous pouvez changer](#ce-que-vous-pouvez-changer)
    * [Statut du dépôt : Terminé](#statut-du-dépôt-:-terminé)
    * [Compatibilité de Processing ](#compatibilité-de-processing-)
    * [À vous de jouer !](#à-vous-de-jouer-)

<!-- table of contents created by Adrian Bonnet, see https://github.com/Relex12/Markdown-Table-of-Contents for more -->

## Qu'est-ce que c'est ?

Lining-draw est un projet sur Processing qui permet de dessiner des formes variées à partir uniquement de lignes qui vont d'un bord à l'autre.

Il n'est possible de dessiner que des lignes, en incrémentant ou décrémentant leurs coordonnées.

## À quoi ça ressemble

Voici deux exemples de figures pré-enregistrées :

![Capture1](https://raw.githubusercontent.com/Relex12/Lining-draw/master/img/Capture1.PNG)

![Capture2](https://raw.githubusercontent.com/Relex12/Lining-draw/master/img/Capture2.PNG)

## Comment l'utiliser

[Processing](https://processing.org/) est requis.

1. Télécharger ou cloner le dépôt
2. Dans le dossier `drawing/`, lancer `drawing.pde`
3. Cliquer sur le bouton Run pour exécuter

## Explication du code

Dans le dossier `drawing/` il y a trois scripts :

* `drawing.pde` est le script que vous devrez exécuter, il appelle une fonciton `figure` dans une structure switch et définit les variables `step` et `maxVal`
* `figures.pde` est là où sont définies toutes les figures, vous pouvez y trouver la forme basique et la forme d'étoile à quatre rayons ci-dessus, parmi d'autres, et c'est là que vous êtes supposé en ajouter
* `fonctions.pde` fournit les fonctions pour les quatre angles haut/bas gauche/droite qui sont appelées pour chaque figure

## Ce que vous pouvez changer

Dans le script `drawing.pde`, vous pouvez modifier la taille de la fenêtre qui s'ouvre. En changeant la valeur de `step`, vous changez la densité de remplissage de la figure. La variable `figure` n'est utilisée que dans le switch en dessous pour changer rapidement de figure.

Vous pouvez ajouter vos propres figures dans le script `figures.pde`. Soyez bien sûr de comprendre comment les autres fonctionnent.

## Statut du dépôt : Terminé

Ce projet est un petit projet, l'auteur a travaillé tout seul dessus pendant peu de temps. Le code source est donné librement à la communauté GitHub, sous la seule licence MIT, qui n’est pas trop restrictive.

Si vous voulez ajouter des fonctionnalités, faîtes un fork sur le dépôt. Il n'est pas prévu d'accepter de Pull Requests, mais qui sait.

## Compatibilité de Processing 

Comme c'est un petit projet, le code n'a été testé que sous Processing 3 (3.5.4). J'espère que ça marchera pour toutes les anciennes et nouvelles versions.

## À vous de jouer !
