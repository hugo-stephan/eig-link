

# Préambule

La Loi pour une République Numérique de 2015 oblige les
administrations à publier les documents administratifs qu’elles
produisent sous licence libre.  Le code source d’un logiciel est
assimilé à un document administratif, donc il doit lui aussi être
publié sous licence libre.

Ce document a pour vocation de guider les EIG dans la publication et
la gestion de leurs projets de logiciels libres.

Il propose quelques outils pour avancer pragmatiquement : il ne
prétend pas couvrir ces problématiques de façon exhaustive et il n’a
pas vocation à être un référentiel juridique.


# Comprendre les licences libres


## Des licences pour les logiciels et les contenus

La « culture libre » mobilise deux types de ressources : le *code
source* de logiciels et des *contenus autres* (textes, images, etc.)

Lorsqu’on évoque les licences libres, on pense spontanément à celles
qui couvrent les *logiciels libres*, mais certaines licences Creative
Commons sont aussi des licences libres.

Par exemple : le noyau Linux est publié sous licence libre GPLv2 et
les contenus de Wikipédia sont publiés sous licence Creative Commons
by-sa 3.0.

Étalab a publié une licence qui peut couvrir aussi bien les logiciels
que les contenus, la Licence Ouverte 2.0 ([pdf](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf)).


## Les quatre libertés garanties par les licences libres

Les licences libres sont des *contrats* passés entre l’auteur d’un
logiciel et un utilisateur, celui-là accordant à celui-ci ces quatre
libertés :

-   la liberté **d'utiliser** le logiciel ;

-   la liberté **de copier** le logiciel ;

-   la liberté **d'étudier** le logiciel ;

-   la liberté **de modifier** le logiciel et de redistribuer les versions
    modifiées.

Ce principe est commun à *toutes* les licences libres.


## Les deux grandes familles de licences libres

Il y a deux grandes familles de licences libres :

-   les licences dites « **copyleft** », qui garantissent que les versions
    redistribuées du logiciel (modifié ou non) sont publiées avec les
    mêmes garanties sur les libertés de l’utilisateur ;

-   les licences dites « **permissives** », qui permettent à des versions
    redistribuées du logiciel (modifié ou non) d’être publiées sous des
    conditions ne garantissant pas les quatre libertés fondamentales de
    l’utilisateur.

La licence copyleft la plus connue est la licence [GNU GPL](https://fr.wikipedia.org/wiki/Licence_publique_g%25C3%25A9n%25C3%25A9rale_GNU) (General
Public license).

Les licences permissives connues sont les licences [BSD](https://fr.wikipedia.org/wiki/Licence_BSD), [MIT](https://fr.wikipedia.org/wiki/Licence_MIT), [Apache](https://fr.wikipedia.org/wiki/Licence_Apache).

Les deux institutions de référence pour l’évaluation des licences
libres sont la [Free Software Foundation](https://fr.wikipedia.org/wiki/Free_Software_Foundation) et l’[Open Source Initiative](https://opensource.org/).


## Quelques exemples

-   Le cadriciel [Bootstrap](https://getbootstrap.com/) est publié sous licence MIT.

-   Le logiciel [openssh](https://www.openssh.com/) est publié sous licence BSD.

-   Le noyau [Linux](https://www.linux.org/) est publié sous GPLv2.

-   Le serveur [HTTP](https://httpd.apache.org/) du projet Apache est publié sous licence Apache.

-   Les logiciels du projet [GNU](https://www.gnu.org/) sont généralement publiés sous GPLv3+.


# Choisir une licence libre pour vos codes sources

Vous êtes dans l’un de ces trois cas :

1.  Vous contribuez à un logiciel libre existant.
2.  Vous fourchez (*forkez*) un logiciel libre existant.
3.  Vous écrivez un nouveau logiciel libre.

Nous ne nous intéressons pas aux fourches « techniques », celles où le
fait de fourcher ne sert qu’à pouvoir envoyer des correctifs sur le
logiciel parent.

Quel enjeu de licence pour chacun des trois cas ?

-   **Vous contribuez à un logiciel libre existant:** La loi pour une
    République Numérique autorise les agents publics à contribuer à
    des logiciels libres existant.  Si vous êtes dans ce cas,
    veuillez vous référer à la [Politique de Contribution Open source](https://disic.github.io/politique-de-contribution-open-source/*),
    qui vient d’être publiée en version 1.  Les administrations sont
    en train de se familiariser avec cette politique : n’hésitez pas
    à faire part de vos remarques à votre administration.

-   **Vous fourchez (*forkez*) un logiciel libre existant:** si le logiciel
    parent est sous licence copyleft, votre version modifiée sera
    sous la même licence (ou sous une autre licence copyleft
    compatible) ; si le logiciel parent est sous licence permissive,
    vous pouvez publier votre version sous la licence permissive ou
    copyleft que vous voulez, l’usage courant étant d’utiliser la
    même licence que le logiciel parent.
    
    Par exemple : vous fourchez un thème bootstrap publié sous
    licence MIT.  L’usage courant est de publier votre version sous
    licence MIT.  Mais vous pouvez aussi publier votre thème sous la
    licence copyleft GNU GPLv3, à condition d’indiquer quelles sont
    les parties héritées, couvertes par la MIT, et quelles sont les
    parties nouvelles, couvertes par la GNU GPLv3.

-   **Vous écrivez un nouveau logiciel libre:** le choix entre une licence
    permissive ou copyleft se fera selon votre stratégie et/ou selon
    les choix faits par d’autres logiciels similaires écrits dans le
    même langage.

Pour le détail sur la compatibilité des licences voir [ce tableau](https://vvlibri.org/fr/guide-de-lauteur-libre-gerer-des-licences-differentes-compatibilites-de-licences/tableau-de) et
ces [explications](https://www.gnu.org/licenses/license-compatibility.fr.html) de la FSF.

À noter que la question de la licence libre se pose au moment de la
*publication* de votre code.


## Les licences autorisées pour l’administration publique

Étalab publie [la liste des licences autorisées](http://www.data.gouv.fr/fr/licences) pour les codes sources
de l’administration publique.

Si la licence libre que vous souhaitez utiliser ne figure pas dans
cette liste, vous pouvez écrire à `homologation.licence@data.gouv.fr`
pour demander à faire homologuer la licence choisie.


# Bien communiquer autour de votre code


## Soyez clair sur la maintenance

-   [ ] Qui est mainteneur (le nom d’une personne et une adresse email).

-   [ ] Si la maintenance est *passive* (vous répondez aux questions et
    aux demandes d’amélioration mais vous ne travaillez pas activement
    sur le code) ou *active* (vous travaillez activement sur le code).


## Trouvez un nom adéquat pour votre logiciel

Éviter les noms génériques: "app", "donnees", etc.


## Ajoutez les informations essentielles à vos dépôts de code

-   [ ] Une description claire en anglais
-   [ ] Des tags (au moins #EIG #VOTRE\_DEFI)
-   [ ] Un lien vers un site web s’il y en a un
-   [ ] Un fichier README en anglais
-   [ ] Un fichier LICENSE avec le texte de la licence
-   [ ] Un fichier CONTRIBUTING en anglais qui explique comment contribuer


## Allez droit au but dans votre fichier README

-   [ ] L’auteur © [Votre administration] [Vous]
-   [ ] Une façon de tester le logiciel
-   [ ] Un point de contact avec le mainteneur
-   [ ] Une indication des contributions acceptées
-   [ ] La licence libre utilisée
-   [ ] Pour EIG : une mention finale "Projet développé dans le cadre du
    programme « Entrepreneur d’intérêt général »" avec un lien vers le
    [site du programme](https://entrepreneur-interet-general.etalab.gouv.fr/).


## Guider les contributeurs sur Github

Sur Github, vous pouvez ajouter un fichier `ISSUE_TEMPLATE` dont le
contenu sera inséré dans les nouveaux tickets ("issues") ouverts, et
`PULL_REQUEST_TEMPLATE` pour les *pull requests*.

Vous trouverez un exemple pour ISSUES\_TEMPLATE [ici](https://www.talater.com/open-source-templates/#/page/98) et de la
documentation [ici](https://help.github.com/articles/helping-people-contribute-to-your-project/).


## Rédigez une documentation utile

-   [ ] Avez-vous une documentation ?
-   [ ] Votre documentation est-elle rédigée en anglais ?
-   [ ] Avez-vous des spécifications ou un cahier des charges ?
-   [ ] Avez-vous une documentation orientée utilisateur ?
-   [ ] Avez-vous une documentation orientée développeur ?
-   [ ] Votre documentation explique-t-elle comment contribuer ?
-   [ ] Votre documentation est-elle accessible sous des formats ouverts ?
-   [ ] Analysez-vous les visites du site web de votre documentation ?
-   [ ] Votre documentation est-elle publiée sur un site web ?
-   [ ] Les noms de vos variables/fonctions sont-ils parlants ?
-   [ ] Avez-vous des docstrings dans vos fonctions/variables ?
-   [ ] Avez-vous des commentaires dans votre code ?
-   [ ] Générez-vous de la documentation à partir des commentaires et/ou des docstrings de votre code ?
-   [ ] Votre documentation est-elle éditée sous un système de gestion de versions ?
-   [ ] Votre documentation indique-t-elle comment signaler une erreur ?
-   [ ] Avez-vous testé votre documentation auprès des utilisateurs ?
-   [ ] Votre documentation est-elle publiée sous licence libre ?
-   [ ] Votre documentation contient-elle une section de remerciements ?
-   [ ] Votre documentation contient-elle une section sur l’historique du projet ?


# Impliquer des utilisateurs et contributeurs

Il ne suffit pas de publier un logiciel sous licence libre pour en
faire un « bien commun » : il faut aussi animer son développement et
mobiliser une communauté de contributeurs.


## Des degrés d’ouverture des projets libres

Ci-dessous un tableau pour présenter différents « dégrés » d’ouverture
de projets libres :

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">Degré</th>
<th scope="col" class="org-left">Publié</th>
<th scope="col" class="org-left">Licence libre</th>
<th scope="col" class="org-left">Maintenance</th>
<th scope="col" class="org-left">Versioning</th>
<th scope="col" class="org-left">README</th>
<th scope="col" class="org-left">Bug tracker</th>
<th scope="col" class="org-left">Packaging</th>
<th scope="col" class="org-left">Contribution</th>
<th scope="col" class="org-left">Tests</th>
<th scope="col" class="org-left">Documentation</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-right">-1</td>
<td class="org-left">Non</td>
<td class="org-left">?</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">?</td>
<td class="org-left">?</td>
<td class="org-left">?</td>
<td class="org-left">?</td>
<td class="org-left">?</td>
<td class="org-left">?</td>
<td class="org-left">?</td>
</tr>


<tr>
<td class="org-right">0</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">1</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">2</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">3</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">4</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">5</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">6</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">7</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">8</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
<td class="org-left">Oui</td>
</tr>
</tbody>
</table>

-   **Publié:** votre logiciel est disponible quelque part
-   **Licence libre:** la licence libre de votre logiciel est clairement indiquée
-   **Maintenance:** on sait si la maintenance est active et qui la gère
-   **Versioning:** le code est publié via un système de gestion de version (git)
-   **README:** votre dépôt contient un fichier README en anglais
-   **Bug tracker:** vous utilisez un système de remontée et de suivi de bugs public
-   **Packaging:** votre logiciel peut être installé facilement
-   **Contribution:** vous indiquez clairement comment contribuer
-   **Test:** votre logiciel contient une suite de tests unitaires
-   **Documentation:** vous maintenez la documentation de votre logiciel


## Des règles de bonne conduite au sein d’un projet libre

Des règles simples, claires et explicites vous aident à maintenir une
collaboration respectueuse et constructive au sein de votre projet.

Voir le <https://www.contributor-covenant.org> pour un exemple.


# Pourquoi ouvrir son code ?

-   Pour **respecter la loi** pour une République Numérique.

-   Pour être **transparent** : par exemple, si le code de votre
    administration met en oeuvre un algorithme au sujet duquel le
    citoyen est en droit de demander des explications.

-   Pour **contribuer aux biens communs numériques** : tous les systèmes
    d’information reposent directement ou indirectement sur des
    logiciels libres : en ouvrant son code, l’administration participe à
    cette mise en commun du code.

-   Pour **trouver des testeurs** : en ouvrant votre code et en le rendant
    facile à installer, vous multipliez les possibilités de le tester.

-   Pour **impliquer des développeurs extérieurs** : si vous allez au-delà
    de la simple mise à disposition du code sous licence libre et vous
    mobilisez pour construire une communauté, vous pourrez bénéficier de
    contributions extérieures.

-   Pour **améliorer votre code** : coder « in the open » est une façon de
    se contraindre à adopter des bonnes pratiques qui touchent à la fois
    la technique (structurer son code, le tester) et la communication
    (écrire une documentation, répondre aux questions des utilisateurs,
    etc.)


# Les réticences à surmonter pour l’ouverture

-   **« Nous allons nous faire pirater notre serveur »:** Publier le code
    source d’une application web va permettre à d’autres de la tester
    et de faire remonter les éventuels problèmes de sécurité.

-   **« Nous allons montrer du code sale »:** Oui.  Cela vous incitera à
    le nettoyer.

-   **« Ouvrir le code va nous donner plus de travail »:** Non si
    l’ouverture correspond au « degré zéro » de l’ouverture, à savoir
    la simple mise à disposition sous licence libre.  Oui si votre
    stratégie d’ouverture implique un degré supplémentaire, avec une
    maintenance active.

-   **« Nous allons exposer des problèmes de sécurité »:** Oui, cela
    permet de mieux les corriger.

-   **« Notre code est inutile sans certains paramètres »:** Dans ce cas,
    les utilisateurs pourront toujours vérifier que votre code fait
    bien ce qu’il est supposer faire, avec ou sans la connaissance
    des paramètres.

-   **« Nous allons exposer des données confidentielles »:** Au moment de
    publier le code source de votre application, veillez à ne pas y
    laisser traîner de mots de passe ou de clefs secrètes.

-   **« Nous ne pourrons plus breveter notre logiciel »:** Il n’est pas
    possible de breveter des logiciels en Europe.

-   **« Nous ne pourrons plus exploiter commercialement notre code »:** Vous ne pourrez pas faire reposer votre modèle de financement sur
    la vente d’un logiciel fermé mais il existe de nombreux modèles
    économiques autour du logiciel libre.

Les réticences les plus fréquentes portent sur les problèmes de
sécurité et les problèmes d’exploitation commerciale.


# Quelques ressources utiles


## Du côté de la mission Étalab

-   La liste des licences libres pour l’administration :
    <https://www.data.gouv.fr/fr/licences>

-   La politique de contribution Open Source :
    <https://github.com/disic/politique-de-contribution-open-source>

-   La licence ouverte 2.0 :
    <https://www.etalab.gouv.fr/licence-ouverte-open-licence>


## Ressources extérieures

-   Des guides sur l’open source en général : <https://opensource.guide>

-   [Open source Guidance](https://www.gov.uk/government/publications/open-source-guidance) : par le gouvernement britannique

-   [18F Open Source Style Guide](https://open-source-guide.18f.gov/) : par l’agence états-unienne 18F

-   Une explication des licences Creative Commons dans [cette
    présentation](https://www.slideshare.net/bzg/ressources-libres-pour-lducation-lesquelles-et-pourquoi-15552125) sur les ressources pédagogiques libres.

-   [Sept idées reçues sur le logiciel libre](https://bzg.fr/sept-idees-recues-sur-le-logiciel-libre.html)


## Conventions de style

Voici un tableau des « guides de style » pour différents langages :

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Langage</th>
<th scope="col" class="org-left">Coding style</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">Python</td>
<td class="org-left"><https://www.python.org/dev/peps/pep-0008/></td>
</tr>


<tr>
<td class="org-left">Clojure</td>
<td class="org-left"><https://github.com/bbatsov/clojure-style-guide></td>
</tr>


<tr>
<td class="org-left">Ruby</td>
<td class="org-left"><https://github.com/bbatsov/ruby-style-guide></td>
</tr>


<tr>
<td class="org-left">Javascript</td>
<td class="org-left"><https://eslint.org></td>
</tr>


<tr>
<td class="org-left">PHP</td>
<td class="org-left"><https://www.php-fig.org/psr/psr-2/></td>
</tr>


<tr>
<td class="org-left">R</td>
<td class="org-left"><https://google.github.io/styleguide/Rguide.xml></td>
</tr>


<tr>
<td class="org-left">Go</td>
<td class="org-left"><https://golang.org/doc/code.html></td>
</tr>
</tbody>
</table>
