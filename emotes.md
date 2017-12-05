# Comment créer une émote avec un fond transparent ?

Prenons par exemple le logo de La Commune. Imaginons que vous vouliez créer une émote reprenant le cube avec le texte, sans le fond rouge.
Vous avez cette image : 
![logo au début](La_commune_depart.png)
Et vous voudriez obtenir celle-ci : 
![logo à la fin](la_commune_final.png)
Pour cela, il faut faire disparaitre le fond rouge de l'image. Ce guide vous explique la démarche à suivre.

Ce guide fonctionne pour les émotes créées sous Gimp. Si vous n'avez pas ce logiciel, vous pouvez le trouver 
[ici](https://www.gimp.org/fr)

## 1ère étape : création de calque
Ouvrir l'image avec Gimp 
Vous obtenez ceci : 
![Aperçu de Gimp](Logo_La_commune_1.png)
Faire un clique droit sur l'image > calque > dupliquer le calque. Vous obtenez alors une copie de l'image, comme on peut le voir ici :
![Création d'une copie de l'image](Logo_la_commune_2.png)
Puis clique droit sur l'image > calque > fusionner vers le bas
Cette étape permet de fusionner l'originale avec la copie, qui devient en quelque sorte le « background », que l'on pourra enlever pour faire un fond transparent.

## 2ème étape : détourage
Cette étape est celle du détourage, dans laquelle vous allez sélectionner l'image à séparer du fond. 
Pour cela, allez dans outils > outils de sélection > sélection à main levée
Pour plus de confort et de précision, vous pouvez zoomer sur l'image. Pensez à bien fermer le contour. 

## 3ème étape : suppression du fond
Dans cette étape, vous allez supprimer le fond avec ctrl+ x. Pour cela, deux situations sont possibles :
  * si c'est l'image qui est sélectionnée, aller dans sélection > inverser, afin de sélectionner le fond.
  * si c'est le fond qui est sélectionné, il n'y a rien à faire
Une fois le fond sélectionné, faire Ctrl + x. Le fond disparaît.
![Le logo après diparition du fond](Logo_la_commune_3.png)
Puis sélection > aucun pour désélectionner l'image
Ensuite, il faut enlever le plus de fond transparent possible, pour ne garder que l'image qui nous intéresse. Pour cela : Outils > outils de sélection > sélection rectangulaire pour sélectionner l'image, puis Image > Rogner selon la sélection. 

## 4ème étape : enregistrement du résultat
Vous obtenez votre image, avec un fond transparent, prête à être sauvegardée pour devenir une émote. Il vous faut l'enregistrer avec l'extension .png.
Pour cela : Fichier > exporter sous 
Nommez votre fichier avec l'extension .png : le_nom.png . Dans notre exemple, notre emote s'appelle Lacommune.png
Cliquez sur « export ». Une fenêtre apparaît, cliquez de nouveau sur « export »
![Exporter l'image créée](logo_la_commune_4.png)
C'est terminé, votre image est prête à être ajoutée aux autres émotes du serveur.

