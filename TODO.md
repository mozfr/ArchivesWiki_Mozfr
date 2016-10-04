Propositions de contributions !

## Développement Web

### www.mozfr.org

* __URGENT&nbsp;* Ajouter un calendrier / agenda sur la page d'accueil pour permettre de suivre facilement les événements à venir. __Je vais proposer un essai [anthony](http://wiki.mozfr.org/Utilisateur:Anthony)__
    * Essai disponible sur http://anthony-maton.eu:8001/ basé sur l'agenda du libre québécois avec les modifications nécessaires à un fonctionnement pour la France.
    * Une méthode simple pour y parvenir serai de créer une catégorie ou un tag événement sur le blog ; et lister dans un coin les articles associés.
    * _Je me suis permis de créer une page à part [http://wiki.mozfr.org/TODO-Agenda] pour pouvoir savoir ce qui est attendu avec plus de précisions_
* __URGENT&nbsp;* Créer une map des contributeurs francophones afin de rajouter une page sur le site &quot;Qui sommes-nous et où sommes-nous ?&quot; __Pris en charge par [quentinlamamy](http://wiki.mozfr.org/Utilisateur:Quentinlamamy)__
* Proposer une meilleure page « [Participer](http://mozfr.org/participer) » via la WikiPage [[MozFR:Participer]] ou directement via [[Github pour les nuls|github]]&nbsp;: https://github.com/mozfr/static).
* Modifier le lecteur RSS utilisé en page d’accueil pour qu’il ne montre que les ~250 premiers mots de chaque billet, sans image (https://github.com/mozfr/www) — les modifications pouvant être reversées au projet moonmoon (la classe !) __Pris en charge par [quentinlamamy](http://wiki.mozfr.org/Utilisateur:Quentinlamamy)__

### wiki.mozfr.org
 [Bug tracker sur Github](https://github.com/mozfr/wiki/issues)
* Corriger les problèmes et [améliorer le thème gmo](https://github.com/mozfr/wiki/tree/master/skins/gmo/style)
    * affichage de la barre d'édition
* Ajouter la connexion avec Persona. D'après les gens d'identity, il n'y a pas encore de plugin pour mediawiki et apparemment c'est chaud à faire, si ya un volontaire pour regarder ce serait vraiment un apport ultra important de la communauté française :) __Pris en charge par [quentinlamamy](http://wiki.mozfr.org/Utilisateur:Quentinlamamy)__

### planete.mozfr.org

* Proposer à des gens qui ont déjà ou vont probablement parler de Mozilla en français de les syndiquer sur le planète (avec un flux pour le tag mozilla sur leur blog par exemple)
* Rajouter un lien &quot;Afficher plus&quot; qui charge automatiquement d'autres billets en bas de la page.

### Geckozone

Faire un thème phpbb sympa et actualisable sans problème. 

### Remplacer eventBrite

On utilise eventBrite pour organiser des événements. Ce qui ne plait pas à tout le monde car cela fait appel à un service tiers qui incite fortement à s'enregistrer via facebook. Il faut pouvoir contacter toutes les personnes facilement (en cas d'annulation par exemple)

Il devrait être possible de le remplacer par un système de sondage comme surveymonkey (service hébergé) ou limesurvey (à installer sur un serveur). Peu être un pad sinon ? ou un framadate ?
Il serait intéressant de les évaluer. geb@ peut filer un coup de main.

### Applications Firefox OS=
* Suggestion d'application : https://frenchmoz.etherpad.mozilla.org/Applis-indispensable
* Application à tester : https://frenchmoz.etherpad.mozilla.org/marketplace-fr
* Application à coder : https://frenchmoz.etherpad.mozilla.org/openwebapp-fr
* Applications sur lesquelles communiquer : https://etherpad.mozilla.org/appdujour

## Développement

si vous voulez un mentor proche de vous, plusieurs bugs sont mentorés par des employés de Mozilla Paris.

### GFX
La liste des bugs mentorés par Nical : http://www.joshmatthews.net/bugsahoy/?gfx=1&cpp=1

### Javascript
La liste des bugs mentorés par Nicolas Pierron (nbp) : https://bugzilla.mozilla.org/buglist.cgi?list_id=9545573&resolution=---&resolution=DUPLICATE&emailtype1=exact&status_whiteboard_type=allwordssubstr&query_format=advanced&emailassigned_to1=1&status_whiteboard=mentor%20nbp&email1=nobody%40mozilla.org

__Nicolas Pierron vous propose une liste de 40 bugs &quot;faciles&quot;, parfaits pour commencer : https://bugzilla.mozilla.org/show_bug.cgi?id=1003801__

De plus, IonMonkey va avoir un nouveau backend pour revenir à baseline. A priori, il y a plein de petit bugs (facile) en prévision pour supporter plus d'optimisations. Si vous êtes intéressé, contactez nbp sur IRC ;-)

Yoric est mentor sur pas mal de bugs JS : https://bugzilla.mozilla.org/buglist.cgi?cmdtype=runnamed&namedcmd=mentored&list_id=9837312

### Media
La liste des bugs mentorés par Padenot : http://www.joshmatthews.net/bugsahoy/?media=1&cpp=1

### Firefox OS
Alexandre Lissy travail sur le support des claviers physiques/bluetooth dans b2g (pas de bug mentoré, mais il peut en ouvrir si besoin). Il peut prêter un device avec clavier physique.

### C++
Corriger des Bugs simples à moyens en C++ trouvé par _Scan-build_ (l'analyseur statique C/C++ de LLVM/Clang). [Scan-build aka Clang-analyzer](http://clang-analyzer.llvm.org/) est un outil développé par le projet [LLVM](http://llvm.org/). Il permet de trouver des bugs de programmation difficiles à trouver manuellement.

Beaucoup de ces bugs sont faciles à corriger (variables inutiles, incrémentation inutiles, etc). Par exemple, cet outil est utilisé pour générer les rapports de LLVM/Clang/LLDB: http://buildd-clang.debian.net/scan-build/
Les rapports sur Firefox ne sont pas (encore) publiques mais je (sylvestre chez mozilla point com) peux les envoyer.

Par exemple, une analyse de Firefox indique un certain nombre d'erreurs faciles à corriger:

* Dead assignment      867
* Dead increment       52
* Dead initialization  119

Note: Une partie des erreurs vient des logiciels utilisés/embarqués par Firefox dans ses sources, le processus sera différent pour ces bugs.

### Rust
[Rust](http://www.rust-lang.org/) est un langage de programmation bas-niveau, conçu principalement pour la programmation système, il embarque de nombreux concepts qui ont fait leur preuves. Et se veux _Type Safe_, _Thread Safe_ et performant par design.
#### Rustc
[Rustc](https://github.com/mozilla/rust/) est le compilateur de référence du langage Rust, c'est au travers de ce projet que tout le développement du à lieu.
De nombreux bugs sont faciles à prendre en main et la communauté sera ravi de les aider!

* Participer au développement sur Github: https://github.com/mozilla/rust/
    * Guide du nouveau contributeur: https://github.com/mozilla/rust/wiki/Note-guide-for-new-contributors
* Contribuer à une bibliothèque en Rust: https://github.com/mozilla/rust/wiki/Community-libraries
* Ou écrire soit même une bibliothèque en Rust.

#### Servo
Servo est un moteur de rendu Web en cours de développement chez Mozilla, il est écrit en Rust. https://github.com/mozilla/servo/wiki/Design

* Contribuer au code de Servo lui même: https://github.com/mozilla/servo
    * Rédiger des test.
    * Travailler sur les _students project_: https://github.com/mozilla/servo/wiki/Student-projects 
* Au plus long terme [Roadmap https://github.com/mozilla/servo/wiki/Roadmap].

### Application Firefox OS
gerard-majax est prêt à aider les gens voulant faire les applications suivantes :

* football
* appli tablette de gestion de potager (source : https://linuxfr.org/users/mickael/journaux/tomate-un-logiciel-pour-planifier-vos-cultures, https://github.com/MickaelG/tomate_cpp)

## MDN

### FxOS Security

* Proposition d'arroway : Écrire une page sur MDN (ou sur le wiki pour commencer) pour expliquer simplement les aspects sécurité dans Firefox OS pour les utilisateurs/trices. Ex: expliquer clairement ce que fait Do Not Track dans Firefox OS, ce que cela signifie pour un utilisateur que les applications soient sandboxées, etc. L'idée serait aussi d_essayer de mettre en valeur les features qui différencient FxOS (gestion des permissions, DNT...). 
Ressources: 
    * Security model overview: https://developer.mozilla.org/en-US/Firefox_OS/Security
    * Releases notes (cf. security section): https://developer.mozilla.org/en-US/Firefox_OS/Releases


## Traductions

* Les traductions ouvertes à tous, en cours et à venir sont répertoriées [dans cette liste de bogues](https://bugzilla.frenchmozilla.org/buglist.cgi?product=Traductions&component=Texte%20%C3%A0%20traduire&resolution=---).


### Instantbird

Instantbird n'a pas de traducteur actif pour le français actuellement. Alors n'hésitez pas ! 

### Webmaker

__Des personnes pour localiser et sous-titrer les vidéos du training Webmaker ? La première est ici : https://www.youtube.com/watch?v=IPTd8XRktaM__

### Firefox OS

__Nous recherchons au moins un nouveau contributeur actif pour Firefox OS ! Contactez Pascal (pascal@mozilla.com)__

###  Sumo (assistance aux utilisateurs des produits Mozilla
#### Pour les articles d'assistance de Thunderbird désormais sur SUMO aussi
Vincent (el cameleon) et j2m06 ont besoin de contributeurs pour les traductions, mises à jour etc.

#### Pour tous les produits Mozilla
On a besoin de contributeurs réguliers, bons traducteurs et bons en français.

## Support

[Geckozone](http://forums.mozfr.org/) manque de modérateurs et de personnes pour répondre aux questions. Rejoignez-les ! 


## Tests / QA

### Firefox Desktop

Eh oui car il n'y a pas que Firefox OS dans la vie, il y a Firefox desktop aussi ! Et si vous voulez qu'il cesse de perdre des parts de marché, vous pouvez nous aider en :

* devenant un bêta testeurs des [nightlies localisées](http://ftp.mozilla.org/pub/mozilla.org/firefox/nightly/latest-mozilla-central-l10n/).
* faisant des [rapport de bugs pour les sites qui ne fonctionnent plus sous Firefox](https://bugzilla.mozilla.org/enter_bug.cgi?product=Tech%20Evangelism&component=French) (c'est par exemple arrivé avec la Fnac à noël qui conseillait aux visiteurs d'utiliser un  autre navigateur !) et en prenant contact avec les dit sites.

### Firefox for Android

Même chose que pour Firefox Desktop.

### AMO/Marketplace

Notre cher Gerard-Majax est un peu seul à tout gérer et aurait bien besoin de :

* personnes qui relisent et vérifient les documentations traduites.
* contributeurs qui essayent, notent, et font des retours pour les applications. 

### Thunderbird

Ludovic (usul) recherche plus de personnes utilisant la bêta sous Windows.

## Design

### Transvision

Pascal adorerait avoir un logo pour le projet qu'il soutient, Transvision (http://transvision.mozfr.org/). Quelques pistes :

* il aimerait quelque chose de sérieux mais pas ennuyeux, qui peut s'adapter à plein de tailles, notamment les favicones, qui aille dans les tons actuels (on est dans le bleu ciel);
* ça pourrait être un T pour Transvision dans un cercle par exemple
* des lunettes peut-être (à cause de la vision)
Envoyez vos propositions à pascal@mozilla.com

### Mozilla Paris

Le Bureau de Mozilla Paris est désormais doté d'une équipe spécialement chargée d'organiser des événements.
Laquelle équipe aimerait bien avoir un thème Eventbrite spécial &quot;bureau de Paris&quot;.
Un volontaire ? Contactez thegennok@thegennok.com. 

### Flyers

Multiplication des événements oblige, la communauté aimerait bien en annoncer certains via des flyers que nous enverrions à des écoles d'informatique, des organismes, des institutionnels, etc. 
Si vous êtes volontaire, contactez thegennok@thegennok.com qui vous donnera des indications pour un événement précis. 


## Bonjour Mozilla

* Aidez-nous à traduire Bonjour Mozilla tous les jours ici : https://frenchmoz.etherpad.mozilla.org/bonjourMozilla
* Technique
    * Remplacer dcSocialize par un système basé sur https://github.com/panzi/SocialSharePrivacy (facebook like+share, twitter, google+).
    * Corriger des bugs CSS / refaire le thème en partant d'un thème dotclear récent (responsive design, tout ça…) en gardant les miniatures pour les archives parce que c'est mignon :D
    * Éventuellement trouver un moyen de mettre un bouton diaspora* plus tard.

## Packaging

Sylvestre@debian.org peut sponsoriser / mentorer.

### Packaging de Rust
Rust dans Debian/Ubuntu. Le résultat final serait d'avoir apt-get install rust fonctionnel. Et de suivre les changements upstream. Le travail a commencé https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=689207

### Packaging d'Instantbird
Instantbird dans Debian/Ubuntu. Similaire à Rust, on voudrait avoir apt-get install instantbird A noter que le logiciel a déjà été packagé dans le passé (http://packages.qa.debian.org/i/instantbird.html) mais a été supprimé par manque d'activité du précédent maintainer. De plus, upstream (ie: les développeurs de instantbird) sont intéressés par le travail et donc pourront aider autant que possible.


## Divers

### Bugzilla

Quelqu'un motivé pour faire un &quot;Bugzilla pour les Nuls&quot; (un tutoriel en français) pour les nouveaux ?

A tout le moins, on pourrait faire les sous-titres de cette vidéo déjà existante : http://www.youtube.com/watch?v=piT1pflOTDs

### planete.mozfr.org

* Proposer à des gens qui ont déjà ou vont probablement parler de Mozilla en français de les syndiquer sur le planète (avec un flux pour le tag mozilla sur leur blog par exemple)