# Guide des bots

## Dynobot (Garde rouge tolérant)

Dynobot est un bot multifonction. Pour le configurer, vous devez être membre de l'équipe technique.
(La page de configuration se trouve ici)[https://www.dynobot.net/]


### Commande d'acceptation des invité.e.s

La commande ``!public`` prend en paramètre le nom de la personne à passer en invité.e. Elle change les rôles de la personne et affiche une annonce dans #discussions_publique. Elle s'utilise de la façon suivante :

```
!public LeNom#1234
```

Son code source est le suivant :

```
{require:Admis-e-s}
{delete}
{!role $1+ +A interroger, +Invité-e-s, -Nouveaux-lles}
{silent}
{respond:#discussions_publiques}
Bienvenue dans le salon publique, $1+ ! Tu peux discuter ici avec tout le monde en attendant le vocal de validation.
```

La ligne ``{require:Modération}`` permet de n'autoriser que l'équipe de modération à utliser cette commande.
La ligne ``{delete}`` indique à Dynobot de supprimer la commande tapée du salon.
La ligne ``{!role +Admis-es, -A intéroger, -Invité-e-s, -Nouveaux.lles}`` permet de supprimer les rôles ``A intéroger``, ``Invité-e-s`` et ``Nouveaux.lles`` et d'ajouter le rôle ``Admis-es``.
La ligne ``{silent}`` permet de ne pas afficher le message automatique de Dynobot quand la commande ``!role`` est utilisée.
La ligne ``{respond:#general}`` indique où afficher le message, indépendament d'où est tapée la commande.
Le reste de la commande représente le message à afficher. Le symbole ``#1+`` est remplacé par tout ce qui suivra après ``!admission ``, c'est à dire le nom de l'utilisateur

### Commande d'acceptation des admis.es

La commande ``!admission`` prend en paramètre le nom de la personne à accepter. Elle change les rôles de la personne et affiche une annonce dans #general. Elle s'utilise de la façon suivante :

```
!admission LeNom#1234
```

Son code source est le suivant :

```
{require:Modération}
{delete}
{!role $1+ +Admis-e-s, -A interroger, -Invité-e-s, -Nouveaux-lles}
{silent}
{respond:#general}
Bienvenue $1+ ! Maintenant que tu es admis-e, n'hésite pas à lire la {#constitution} et à suivre notre compte Twitter @LaCommuneNet. Tu peux t'ajouter tes propres étiquettes en cliquant sur ton pseudo, et n'hésite pas à nous dire si tu es concerné-e par un salon non mixte. Si tu as des abonnements à des journaux, des compétences en informatique ou en langue, tu peux aussi te mettre les rôles correspondants. Bonne continuation camarade !
```

La ligne ``{require:Modération}`` permet de n'autoriser que l'équipe de modération à utliser cette commande.
La ligne ``{delete}`` indique à Dynobot de supprimer la commande tapée du salon.
La ligne ``{!role +Admis-es, -A intéroger, -Invité-e-s, -Nouveaux.lles}`` permet de supprimer les rôles ``A intéroger``, ``Invité-e-s`` et ``Nouveaux.lles`` et d'ajouter le rôle ``Admis-es``.
La ligne ``{silent}`` permet de ne pas afficher le message automatique de Dynobot quand la commande ``!role`` est utilisée.
La ligne ``{respond:#general}`` indique où afficher le message, indépendament d'où est tapée la commande.
Le reste de la commande représente le message à afficher. Le symbole ``#1+`` est remplacé par tout ce qui suivra après ``!admission ``, c'est à dire le nom de l'utilisateur

## FredBoat

FredBoat est un bot pour difuser de la musique dans les salons vocaux.

## DuckHunt (chasse aux fafs)

## NotSoBot

## La Commune

Le code source de ce bot est [disponible ici](https://github.com/DiscordLaCommune/BotVote).

### Bannir une personne

Utilisez la commande ``@La Commune ban @LeNom#1234`` pour bannir @LeNom#1234. Attention, cette commande est limité à raison d'un ban par personne et par jour. Vous pouvez aussi kicker une personne avec la commande ``@La Commune kick @LeNom#1234``.

### Sujet des salons

Le bot La Commune peut répéter un ordre du jour ou une annonce dans un salon. Pour cela, utilisez la commande suivante : ``@La Commune topic Mon Message``. « Mon Message » va être alors affiché régulièrement dans ce salon. Pour supprimer ce message, utilisez la commande ``@La Commune topic``.

## Réseau Antifa

## People's Democratic Bot
