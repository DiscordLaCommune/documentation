# Commandes

## Commande d'acceptation des invité.e.s

La commande ``!public`` prend en paramètre le nom de la personne à passer en invité.e. Elle change les rôles de la personne et affiche une annonce dans #discussions_publique. Elle s'utilise de la façon suivante :

```
!public @LeNom#1234
```

## Commande d'acceptation des admis.es

La commande ``!admission`` prend en paramètre le nom de la personne à accepter. Elle change les rôles de la personne et affiche une annonce dans #general. Elle s'utilise de la façon suivante :

```
!admission @LeNom#1234
```

## Bannir une personne

Utilisez la commande ``@La Commune ban @LeNom#1234`` pour bannir @LeNom#1234. Attention, cette commande est limité à raison d'un ban par personne et par jour. Vous pouvez aussi kicker une personne avec la commande ``@La Commune kick @LeNom#1234``.

## Sujet des salons

Le bot La Commune peut répéter un ordre du jour ou une annonce dans un salon. Pour cela, utilisez la commande suivante : ``@La Commune topic Mon Message``. « Mon Message » va être alors affiché régulièrement dans ce salon. Pour supprimer ce message, utilisez la commande ``@La Commune topic``.

## Gestion des messages partagés

Un message partagé est un message posté par le bot La Commune, et qui est modifiable par tout le monde.

Pour créer un message partagé, allez dans le salon souhaité, puis utilisez la commande suivante : ``@La Commune add-msg nom Mon texte``. Un message « Mon texte » va alors être posté par le bot. L'identifiant de ce message sera ``nom``. Pour l'identifiant du message, n'utilisez que les caractères alphanumériques et les tirets (-). N'utilisez pas d'espace.

Pour éditer un message partagé, utilisez la commande suivante depuis n'importe quel salon : ``@La Commune edit-msg nom Mon nouveau texte``. Le message posté par le bot va être édité et contiendra le texte « Mon nouveau texte ». Notez que vous devez avoir les droits d'écriture et de lecture dans le salon où est posté le message partagé.

Pour supprimer un message partagé, utilisez la commande suivante depuis n'importe quel salon : ``@La Commune delete-msg nom``. Le message identifié par ``nom`` sera supprimé. Notez que vous devez avoir les droits d'écriture et de lecture dans le salon où est posté le message partagé.

Pour afficher le code d'un message partagé, utilisez la commande suivante : ``@La Commune view-msg nom``. Cette commande fonctionne également avec l'ID Discord de tout les messages postés sur le salon courant. Ainsi, si vous utilisez la commande ``@La Commune view-msg 345955506877366273`` dans le salon #general, vous verez le code du message posté par un autre utilisateur.

## Organiser un vote populaire

Dans le salon #vote_populaire, utilisez la commande suivante : ``@La Commune vote Description`` (remplacez Description par un message explicatif. Lorsque le vote est actif, envoyez un @everyone dans le même salon.

Si vous souhaitez lancer un vote pour une durée plus courte, utilisez l'option ``hXX``. Par exemple, pour une durée de deux heures : ``@La Commune vote h2 Description``.

## Organiser un vote avec jugement majoritaire

Dans le salon #vote_populaire, postez le message suivant :
```
Comment fonctionne ce vote ?

Vous pouvez voter en cliquant sur une « réaction ». Vous recevrez alors une confirmation de vote via message privé. Vous pouvez changer votre vote à tout moment.

Cette élection fonctionne selon le système dit du jugement majoritaire ( https://fr.wikipedia.org/wiki/Jugement_majoritaire ). Le nombre de modérateur.rice.s est fixé à 4. Le nombre de technicien.ne.s est fixé à 2. **Si vous avez voté pour au moins un.e candidat.e, les autres candidat.e.s pour qui vous n'avez pas voté obtiendront une mention :regional_indicator_r: À rejeter**. Le scrutin est ouvert jusqu'au 30/11/2017 à 23:00

:regional_indicator_r: : À rejeter

:regional_indicator_i: : Insuffisant

:regional_indicator_p: : Passable

:regional_indicator_a: : Assez bien

:regional_indicator_b: : Bien

:regional_indicator_t: : Très bien
.
```
N'oubliez pas de changer la date limite du vote dans ce message.
Postez maintenant le nom du poste pour les candidat·e·s. Par exemple ```__**CANDIDATURES AU POSTE DE MODERATEUR.RICE**__```
Maintenant, pour chaque candidat·e, utilisez la commande suivante :  ``@La Commune vote judge short LeNom``, en remplaçant bien « LeNom » par le nom de la personne qui candidate. Attention, n'utilisez pas les mentions (@) sinon les confirmations de vote seront illisable.

Pour finir, lancez un @everyone, par exemple de la façon suivante : ``@everyone Le vote pour les modérateur.rice.s est ouvert ! Les instructions de trouvent plus haut.``
