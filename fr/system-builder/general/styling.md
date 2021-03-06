---
title: Styling
description: 
published: true
date: 2020-09-24T12:02:54.855Z
tags: 
editor: undefined
---

La mise en forme sur le *Systeme builder* utilise un système de **_"classes"_**.

Les classes sont des petite commandes que l'on ajoute à un composant pour le faire changer de sont apparence par défaut. On écris ses commandes dans le champs "Classes" du composant. Tout les composants possède ce champs.  
Vous pouvez donner plusieurs classes à un composant ; elles devraient toutes être séparés par un espace, et il ne devrait y a voir aucun espace initile après une classes.

Nous utilisons les classes de Bootstrap 4 comme base pour les classes de Let'role. Donc toutes les classes disponibles dans [les outils bootstrap](https://getbootstrap.com/docs/4.4/utilities/spacing/) sont aussi disponible dans le systeme builder.

Cela étant dit, vous devriez essayer de ne pas trop changer la conception par défaut de Let's Role. C'est particulièrement important si vous souhaitez que votre feuille soit officialisée.

# Couleur de fond
Les classes `highlight-1` et `highlight-2` changent la couleur de fond du composant.

# Espacement
Par défaut, il n'y a pas d'espace entre les composants, il sont donc collé les un aux autres. Les classes d'espacement permettent de donné un peu d'ordre et d'oxygène.
Il y deux type d'espacement :
## Les marges
Elles sont l'espacement exterieur du composant. Les autre composant ne pourront pas s'approcher d'un composant avec des marges.
## Les "padding"
Les padding (traduisez rembourage ou mattelasure) sont des espaces intérieur au composant : les composant à l'intérieur ne pourront pas toucher les bord du composant qui les contient avec un padding.

Ces classes on une nomenclature un peu spcécial, mais facile à comprendre grâce à cette [documentation](https://getbootstrap.com/docs/4.4/utilities/spacing/).  
En voici un bref résumé : `m[coté]-[n][chiffre]` :
* la première lettre est soit `m` pour marge soit `p` pour padding  
* le deuxième lettre désigne le coté ou appliquer l'espacement : gauche, droite, gauche et droite, haut, bas, haut et bas, associer respectivement au lettres l, r, x, t, b, y. S'il n'y a pas de lettre, l'espacement est de tout les cotés.
* Un tiret sépare l'endroit de l'espacement de sa valeur
* On peu ajouter un "n" devant le chiffre, pour appliquer un marge négative : au lieu de se séparé, les composants de superposeront. (Ne fonctionne pas avec les padding)
* Et enfin un chiffre entre 0 et 5 qui caractérise la taille de l'espace. (on peu mettre `auto` à la place d'un chiffre pour les marges)

# Mise en forme de text
On utilise les classe suivantes essentiellement dans les label et dans les choices.
## La taille du texte
Les classes `text-tiny`, `text-small`, `text-medium`, `text-large`, `text-giant`, `text-gargantuan` donnent une taille différente au texte (de gauche à droite, du plus petit au plus grand).

## Titre
La classe `text-title` donne l'aspect d'un titre au text.

## Mettre en gras
La classe `text-bold` met le texte en gras.

# Largeur et Hauteur
Vous pouvez donner une largeur et/ou une hauteur fixe (en pixel) à un composant grâce au commandes `w-[nombre]px` et `h-[nombre]px`.  
"w" Pour *width* qui signifie largeur, et "h" pour *height* qui signifie hauteur.

Les nombres de pixels que vous pouvez choisir en largeur sont 25, 50, 75, 100, 125 150, 175, 200 et 300. (Exemple `w-25px`) Les autre nombres (comm 80 ou 101) ne fonctionneront pas.  
Les nombres de pixels que vous pouvez choisir en hauteur sont tous ceux de la largeur, plus 400, 500, 600 et 700. (Exemple `h-700px`)
