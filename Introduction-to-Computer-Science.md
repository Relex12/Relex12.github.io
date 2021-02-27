---
layout: default
title: "Introduction to Computer Science"
permalink: fr/Introduction-to-Computer-Science
---

# Introduction-to-Computer-Science
Introduction à l'algorithmique, la programmation et d'autres notions pour commencer l'informatique

![](https://img.shields.io/badge/language-French-blue) ![](https://img.shields.io/badge/status-In_progress-green) ![](https://img.shields.io/badge/type-Read_only-green) ![](https://img.shields.io/github/last-commit/Relex12/Introduction-to-Computer-Science)

---

## Sommaire

* [Introduction-to-Computer-Science](#introduction-to-computer-science)
    * [Sommaire](#sommaire)
    * [Introduction - Motivation](#introduction---motivation)
    * [Algorithmique](#algorithmique)
        * [Instructions](#instructions)
        * [Variables](#variables)
        * [Types](#types)
        * [Structure](#structure)
        * [Fonctions](#fonctions)

<!-- table of contents created by Adrian Bonnet, see https://github.com/Relex12/Markdown-Table-of-Contents for more -->

## Introduction - Motivation

Si vous lisez ceci, c'est soit que vous souhaitez découvrir cette chose obscure que l'on nomme la **programmation**, soit parce que vous êtes vous-même un programmeur et que vous souhaitez partager vos connaissances.

Si ce n'est pas votre cas, pas de panique : ceci est une introduction au monde merveilleux de l'informatique et de la programmation. Il n'est pas question de concepts avancés : après avoir lu cette page, vous ne serez pas en mesure de construire un site web, ni une application mobile, ni de faire de l'intelligence artificielle, ou toutes les autres aspects très séducteurs de l'informatique.

Ici, on s'attaque au commencement : de la même manière qu'il faut savoir marcher avant de courir et de sauter, vous aurez besoin de connaître ces bases avant de vous attaquer à des projets plus ambitieux.



## Algorithmique

> Pour commencer, qu'est-ce que c'est que ça, **l'algorithmique** ?

Il s'agit, selon Wikipédia, de "l'étude et la production de règles qui sont impliquées dans la conception d'algorithmes", ce qui n'est pas d'une grande aide.

Un **algorithme**[^1], c'est une suite d'instructions, qui se font dans un ordre bien défini : d'abord la première, puis la deuxième, et on continue jusqu'à la dernière instruction. La plupart des cours sur le sujet font la métaphore entre un algorithme et une recette de cuisine.

> Mais qu'est-ce que c'est qu'une **instruction** ? De quoi est-ce que l'on parle ?

Pour une recette de cuisine, une instruction est une action que la personne qui suit la recette devra effectuer. Pour un algorithme, il s'agit de **l'écriture dans un langage formel d'une opération**. Ces mots sont des termes techniques, nous reviendrons sur leurs sens plus tard. Pour l'instant, retenez juste qu'**une instruction sert à décrire à un ordinateur de manière très précise une opération à effectuer**.

[^1]: On parle ici d'algorithme au sens strict, rien à voir avec des choses nécessairement complexes, on pourrait aussi parler de programme.



### Instructions

> Quelles sont les instructions que l'on peut bien réaliser dans un algorithme ?

Le **jeu d'instructions** (ensemble des instructions possibles) dépend du type de langage que l'on utilise, mais certaines se retrouvent dans tous les langages : **déclaration de variable**, **affectation**, **appel de fonction**, **appel système**, **condition**, **boucle**.



Avant d'éclaircir tout cela, quelques notions :

> D'abord, qu'est-ce que c'est une variable ?

Sans rentrer trop dans le détail pour l'instant, une variable est définie par un nom, par exemple `ma_variable` et possède une valeur. Le type de valeur que peut prendre une variable (un nombre, un caractère, etc...) est défini par son **type**.

> Et une fonction, qu'est-ce que c'est ?

Une fonction, c'est une suite d'instruction que vous avez écrit vous même[^2] afin de simplifier le code. Le but est de décrire l'ensemble des instructions à réaliser pour une action donnée, il suffit ensuite d'appeler cette fonction à chaque fois que vous aurez besoin de l'action donnée (par exemple : trier une liste).

Comme une variable, une fonction possède un nom et un type, mais en plus d'une fonction, elle possède une liste d'arguments, ou paramètres, dont chacun possède un nom et un type de valeur, mais nous reviendrons dessus plus tard.

> Dans ce cas, l'appel système, c'est quelque chose qui ressemble à un appel de fonction ?

Pas exactement : la fonction est écrite dans le même langage que l'instruction qui l'appelle. Un appel système permet de faire appel à des fonctions du système d'exploitation (Windows, Linux, MacOs) afin de réaliser des actions spécifiques, par exemple : lire un fichier ou afficher du texte.[^3]



Nous pouvons maintenant revenir sur les instructions :


* une **déclaration de variable **permet de préciser au programme le nom d'une variable que l'on va utiliser.[^4]
* une **affectation** sert justement à donner une certaine valeur à une variable.
* un **appel de fonction** appelle ladite fonction, les instructions de la fonction sont insérées entre l'appel de la fonction et l'instruction qui suit.
* une **condition **rend le programme réactif : **si** \<une certaine condition\> **alors** \< telle instruction\>
* une **boucle **permet de répéter une suite d'instruction un certain nombre de fois

> Les trois premières, ça va, mais les conditions et les boucles, qu'est-ce que c'est ?

Il s'agit de structures particulières dont on se sert pour permettre au programme d'adapter son comportement.

L'instruction conditionnelle permet de faire ou de ne pas faire une ou plusieurs instructions selon une certaine condition. Imaginons par exemple que dans votre programme, vous possédez une variable `ma_variable`, et que selon sa valeur, vous souhaitez que le comportement du programme soit différent. Vous pouvez alors faire quelque chose qui ressemble au code ci-dessous :

```
si (ma_variable < 5) alors
	[...]
```

A la place de `[...]`, vous devrez placer la suite d'instruction qui correspond au comportement que doit avoir le programme lorsque `ma_variable` est strictement inférieur à 5.



Une boucle permet, comme son nom l'indique, de boucler sur une suite d'instructions un certain nombre de fois. Il existe plusieurs manières de réaliser des boucles, la première étant de préciser la condition nécessaire pour sortir de la boucle. Tant que cette condition n'est pas satisfaite, la suite d'instructions est répétée. Voici à quoi pourrait ressembler un tel programme :

```
tant que (ma_variable > 10)
	[...]
	ma_variable = ma_variable - 1
```

Il est possible que la condition pour sortir de la boucle ne soit jamais satisfaite, on parle alors de boucle infinie, mais nous y reviendrons.



Attention : dans les deux exemples ci-dessus, le code donné est *une représentation* d'un algorithme, en plus de ne pas être complet. Même si la nuance ne semble pas importante pour l'instant, mais nous en reparlerons lorsque l'on abordera les langages de programmation.



[^2]: certaines fonctions sont définies dans ce qu'on appelle une librairie, elles permettent de simplifier la vie du développeur, sans qu'il ait besoin de réaliser une fonction pour quelque chose de simple qui a déjà été fait avant lui.
[^3]: ces instructions font appel à du code du système d'exploitation, elles n'existent pas dans tous les langages et de toute manière, il existe dans toutes les librairies des fonctions qui réalisent les appels systèmes.
[^4]: la déclaration d'une variable permet d'ajouter une entrée dans la table des symboles, qui est utilisée d'abord lors de la compilation, puis pendant l'exécution.



### Variables

Il est temps à présent de s'attarder un petit peu plus sur les variables, sur la flexibilité qu'elles offrent est leur nécessité dans un programme. Une variable sert donc à récupérer la valeur à un moment donné dans le programme et à stocker cette valeur. Afin de retrouver la valeur, on définie la variable par son **nom de variable**, de cette manière on pourra récupérer la valeur plus tard.

> Mais quel peut être l'intérêt de stocker cette valeur ? Si l'on sait quelle valeur est stockée, alors c'est qu'on n'a pas besoin de la stocker.

La réponse se fait en plusieurs étapes.

Tout d'abord, votre programme va s'exécuter avec ce que l'on appelle des arguments. Sans rentrer dans le détail du fonctionnement de l'exécution, ces arguments vont permettre d'obtenir différents résultats après avoir déroulé toutes les instructions de votre programme. Le résultat est que, pour ces arguments par exemple, on ne sait pas toujours quelle est la valeur stockée dans une variable. Vous allez alors faire appel à cette variable pour récupérer ces valeurs que vous ne connaissez pas encore lors de l'écriture du programme.

Ensuite, une autre très bonne raison d'utiliser des variables, est de garder dans une seule variable une valeur qui possède un certain sens dans votre algorithme. Cela peut sembler très théorique, alors illustrons cela avec un exemple : admettions que votre algorithme cherche à calculer le déterminant d'un polynôme de degré 3, si vous ne savez pas ce que c'est, dîtes vous que c'est quelque chose en mathématiques qui nécessite un calcul très précis. Pour rappel, ce calcul est *Δ = b² - 4ac*, où *a*, *b* et *c* sont les nombres qui décrivent le polynôme en question. Dans ce cas, il serait très intéressant de déclarer une variable `delta`, et de faire l'affectation suivante :

```
delta = b*b - 4*a*c
```

Un dernier intérêt de l'utilisation de variable est l'économie de ressources. Pour l'instant, nous n'avons pas encore abordé la complexité d'un algorithme, mais sans rentrer dans les détails, lorsque vous écrivez votre programme, vous devrez limiter d'imposer à l'ordinateur des calculs qui ne sont pas nécessaires. Pour reprendre l'exemple du calcul de déterminant : à partir du signe du déterminant, on peut connaître la ou les racines du polynôme. Si l'on cherche également à calculer ces racines, et que l'on n'a pas stocké dans une variable la valeur du déterminant, alors il faudra le recalculer lors du calcul des racines. Au contraire, si la valeur du déterminant a été stockée dans une variable, alors il est possible d'utiliser cette valeur pour calculer les racines du polynôme.

>  Mais comment les utiliser, ces variables ?

Tout d'abord, vous devez les **déclarer**. En général[^5], cela se fait en précisant d'abord le **type**[^6] suivi du **nom**[^7] de la nouvelle variable. 

Les principaux[^8] types de variables sont les suivants :

* les nombres entiers, **int** ou integer, par exemple *0*, *3*, *256* ou *-4*
* les nombres réels flottants ou à virgule flottant, **float**, par exemple *2.5*, *0.01*, -*6.3* ou *10.0*
* les caractères, **char** ou character, par exemple *a*, *B*, *_* ou *8* (on parle ici du caractère 8, et non du nombre entier 8) 
* les chaînes de caractères, **string**, par exemple *Hello World!* ou *aAbBcC*
* les booléens, **bool**, qui peuvent avoir pour valeur **Vrai** ou **Faux**

Il existe également des types composés :

* liste
* (tuples
* dictionnaire)

Une fois que la déclaration est faite, il est possible d'utiliser la variable, c'est à dire de lui **affecter** une valeur. Cela se fait de la même manière que vu précédemment dans l'exemple avec le déterminant d'un polynôme : 



déclaration

* affectation
* opération
  * +, -, *, /, %
  * and, or, xor, not
  * <, >, <=, >=, ==, !=
  * :

[^5]: certains langages sont typés dynamiquement, il n'y a donc pas besoin de préciser le type des variables, il est même possible que la variable soit déclarée lors de la première affectation
[^6]: dans un langage orienté objet, les variables peuvent être d'un type primitif ou d'une classe 
[^7]: les noms de variables communément acceptés sont les suites de lettres (minuscules ou majuscules), chiffres et caractère underscore _, dont le premier caractère est une lettre
[^8]: tous ces types ne sont pas acceptés dans tous les langages, et certains types assez courant ne sont pas présentés ici, comme les doubles



### Types

> Bon, et à quoi elles ressemblent ces instructions ?

* entier
* caractère
* booléen
* tableaux
* chaîne de caractères ou string
* n-uplet
* structures



### Structure

* * condition

* * if
* else if
* else

* boucle

* * while
* for

### Fonctions

* appel de fonction
* * type
* arguments
* Complexité
* * spatiale
* temporelle







* Logique de réalisation
* * itératif
* récursif
* Programmation
* * Langages de programmation (analogie avec le langage naturel : une phrase différente dans chaque langue pour dire la même chose)
* * C, C#, C++, Java, Javascript, Ruby, Python, PHP, Go, SQL, etc...
* Assembleur
* Binaire, Hexadécimal
* Exécutable
* * compilation
* précompilation
* interprétation
* Compilation / interprétation
* * précompilation
* édition de liens
* Langage orienté objet
* * modélisation
* classes
* * attributs
* méthodes
* * getteur
* setteur
* constructeur
* héritage
* Développement
* * IDE
* * fichiers
* console
* workspace
* compilateur
* * éditeur
* console
* Bonnes habitudes
* * Noms de variables
* Nomenclature
* * low Camel Case
* underscore
* Commentaires
* * en bout de ligne  //
* avant une fonction   //
* en début de fichier   /*   */
* Lisibilité
* * indentation
* sauts de ligne
* Idéologie de programmation
* * Payant
* Gratuit
* Open Source
