# Minisite de MozFr pour Firefox OS

URL : http://firefoxos.mozfr.org/

##Dev

### GitHub

Anthony : Création un label sur le github pour les issues où on aurait besoin de quelqu'un de la communication pour nous aider à décider. Du coup, une première demande d'aide : https://github.com/mozfr/firefoxosminisite/issues/12

J'ai crée une branche sur le dépôt firefoxosminisite (la branche refonte).

MoniqueB :

* http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/
* http://christopheducamp.com/2013/12/16/gitHub-pour-nuls-partie-2/

&lt;mentalo /&gt; : Pour ceux qui préfèrent apprendre en vidéo plutôt qu'en lisant, essayez ceci : http://fr.openclassrooms.com/informatique/cours/gerer-son-code-avec-git-et-github (inscription nécessaire par contre).

La partie 2 suffit pour apprendre à se servir de Github, mais la 1 explique les concepts de base, ça reste utile pour comprendre de quoi on parle. Mais vous pouvez sauter la 3e, elle n'est pas nécessaire pour une utilisation basique.

En une grosse heure de vidéo vous devriez être des champions.

Dattaz : [[Github_pour_les_nuls|Github pour les nuls]]

### Objectifs

Flore : Suite à la réunion du groupe comm' ce soir, on a trouvé du boulot à faire pour les web dév :D

En gros, on a une meilleure idée de ce que doit être le minisite.

Le design de la page d'accueil serait dérivé de celui en cours de dev pour Mozilla  https://www-demo5.allizom.org/en-US/?version=a2 . Dont le code source est disponible (mais je ne sais pas où), Théo ou dattaz devrait pouvoir nous dire où le trouver.

Il faudrait aussi un blog indépendant de celui de mozfr. Et la préférence irait à un Wordpress. À cause des plugins disponibles, d'un thème OneMozilla déjà dispo.

L'idée, bien évidemment, c'est que les tuiles soient des contenus dynamiques. Par exemple, la tuile menant au blog devrait afficher un extrait du dernier billet publié…

En plus des dev qui s'étaient déjà proposés (Anthony, dattaz, Siraj, Monsieur Tino, Guillaume, &lt;mentalo /&gt;) ou parmi eux, ce serait pas mal d'avoir un designer, si on a besoin d'adapter le design ou d'intégrer un peu mieux certains trucs.

D'autant que si la même équipe peut, par la suite, redonner un coup de peinture à tout le reste du site et en tout dernier au forum (une fois que phpBB 3.1 sera sorti), ça serait top.

Tout le dev pour mozfr se passe sur github https://github.com/mozfr/firefoxosminisite , je pense que Pascal peut vous expliquer comment ça se passe.

Voilà… Aurélien devrait envoyer un cahier des charges un peu plus complet, mais voilà une première idée. Dites-nous ce que vous en pensez, si c'est possible, combien de temps ça pourrait prendre, si vous avez d'autres propositions / questions.
----

Laurent (ReUp) : Pour les contenus qui seront sur la _home_ :

* des contenus qui vont venir du wordpress (donc articles de blog). Idéalement, si certains posts peuvent être « featured » (je crois qu'on dit comme ça pour les thèmes WP) vs d'autres qui sont moins mis en avant, c'est top.
* des contenus qui vont venir des réseaux sociaux Firefox OS (Twitter + Facebook). À confirmer avec la communauté mais il faudrait pouvoir faire une validation a priori afin de mettre en avant le tweet qui est intéressant, le commentaire de Facebook qui est le plus inspirant etc. Le type de rendus est probablement ce qu'on voit sur le site de Pepsi : http://www.pepsi.com/en-gb/d/ où ils choisissent quels tweets mettre en avant. Peut être faut-il en mettre seulement 2 ou 3 maximum afin de ne pas surcharger la home ?
* des contenus qui vont venir de Geckozone. Pareil, idéalement une mise en avant de la meilleure question / du meilleur fil avec modération a posteriori (pas sûr que ce soit automatisable) http://forums.mozfr.org/viewforum.php?f=35 .
----

Aurélien : début de __cahier des charges__:

Adresse : http://firefoxos.mozfr.org

Délai de livraison souhaité : __mi-octobre 2014__

__Objectif__du site : rassembler les contenus élaborés par la communauté pour le lancement digital de FFOS en France et devenir le point de référence des utilisateurs et futurs utilisateurs de FFOS en France.

__Charte graphique * 

Maquette de base : https://www-demo5.allizom.org/en-US/?version=a2

Code : https://github.com/mozilla/bedrock/compare/homepage-prototype-two et https://github.com/mozilla/bedrock/commit/b1b72aa56cbca0d0f442264a501f6643d832c5f9 (merci Théo !)

Je pensais reprendre les couleurs du logo de Mozfr afin d'établir une charte graphique cohérente que l'on pourra réutiliser pour l'ensemble du site mozfr.org , et qui soit différente de celle du futur mozilla.org.

__Charte éditoriale__:

cf mail de Laurent, soit (voir aussi [[FirefoxOS/LancementEnFrance/RéseauxSociaux]]) :

* contenus issus de Facebook : https://www.facebook.com/firefoxosfr
* contenus issus de Twitter : https://twitter.com/firefoxosfr
* contenus issus de G+ : https://plus.google.com/102403271624576887074/about
* contenus issus de YouTube : https://www.youtube.com/user/FirefoxOSfr/
* contenus issus de Geckozone : http://forums.mozfr.org/viewforum.php?f=35
* contenus issus de Bonjour Mozilla : http://bonjourmozilla.fr/
* contenus issus du Wordpress

__Gestion du contenu__: objectif si possible que l'équipe comm puisse mettre à jour les contenus sur le minisite __de façon autonome__, sans passer par l'intervention de l'équipe Webdev.
----

Natalia : Pour l'objectif du 15 octobre, on peut faire ça progressivement.
----

Aurélien : pour la maitrise de GitHub, dans tous les cas l'objectif est d'avoir le site en ligne le plus tôt possible =&gt; je propose qu'on s'organise en interne dans l'équipe com pour voir qui saurait mettre à jour les contenus dans un premier temps et que ceux qui savent permettent à ceux qui ignorent (comme moi donc) de devenir des pros du truc en un temps record.