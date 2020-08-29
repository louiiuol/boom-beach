# Boom Beach V1



## Objectif

concevoir et implémenter le jeu Boom Beach en Java / Objet. Cet exercice commence avec une partie des bâtiments.

## Contexte

Boom Beach est un jeu de stratégie sur mobile dans lequel les joueurs gèrent un village avec différents types de bâtiments ou encore des barges de débarquement pour attaquer d’autres joueurs.
Il est conseillé de télécharger et installer le jeu pour avoir un maximum de détails, il n’est pas obligatoire de créer un compte. Cette installation peu être temporaire le temps de l’exercice.
Un tel jeu est idéal pour travailler la conception objet, avec notamment de l’héritage. Cependant si l’héritage n’a pas encore été vu ensemble, il y a deux stratégies : se documenter et s’auto former ou attendre qu’on voit l’héritage avant d’aller plus loin individuellement. Dans les deux cas il faudra s’attendre à du refactoring, ça fait partie du job !
Travailler dans un 1er temps avec des CRC Cards, afin de déterminer quelles sont les classes à écrire, les propriétés et les collaborateurs. Utiliser l’anglais pour travailler cette compétence transverse.
### Les bâtiments
Les bâtiments ont tous en commun d’avoir un niveau de progression (en commençant à 1) et un niveau de santé.
#### Bâtiments de ressource
Ils permettent de générer des ressources (or, fer, bois, pierre) servant à construire d’autres bâtiments. En plus de la santé, ils ont une capacité de stockage et de production par heure.
#### Bâtiments de réserve
Ils permettent de stocker les ressources générées, ils sont spécialisés par type de ressource. En plus de la santé, ils ont une capacité de stockage (autrement dit, ils sont proches des bâtiments de ressource mais ne produisent rien).
#### Bâtiments de défense
Ils permettent de défendre le village en cas d’invasion par d’autres joueurs réels ou I.A. En plus de la santé, ils ont en commun de provoquer des dégâts par seconde et une portée d’attaque (courte, moyenne, longue, très longue).
Certains bâtiments de défense ont une durée d’effet (en seconde). Ils provoquent une paralysie temporaire des troupes ennemies.

> Les différents bâtiments de défense :
> - Tour de sniper
> - Super canon
> - Lance-électro bombes (avec durée d’effet)
> - Mortier
> - Mitrailleuse
> - Canon
> - Lance-flammes
> - Lance-roquettes
