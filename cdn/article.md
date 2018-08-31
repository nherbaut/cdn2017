---
title: Fiabilité et sincérité des systèmes blockchain
author:
  - Nicolas Herbaut:
      institute:
        - Université Paris 1 Panthéon Sorbonne
      email: nicolas.herbaut@univ-paris1.fr
  - François-Vivien Guiot:
      institute: Université Toulouse 1 Capitole
      email: francois-vivien.guiot@ut-capitole.fr

bibliography: cdn/bibliography.bib
project:
  title:  Fiabilité et sincérité des systèmes blockchain
...

# Intro #

Le terme de « Système », repris cinq fois dans le programme, est un terme qui a priori fait sens aussi bien pour les juristes que pour les « vrais » scientifiques. Malgré son absence dans notre glossaire, il devrait donc constituer un bon vecteur de convergences. Il n’est cependant pas certain que la notion fasse tout à fait sens de la même façon pour les uns et pour les autres.
Ainsi, si dans le domaine du numérique on devrait accepter de retenir le système comme un « ensemble d’éléments qui dépendent réciproquement les uns des autres de manière à former un tout organisé », au sein de la doctrine juridique on s’arrêtera également et peut-être davantage sur une seconde acception qui voit dans le système un « ensemble d’idées logiquement solidaires et tendant à offrir une vue cohérente d’un objet ou d’un champ d’étude ».
D’un côté le système est l’objet de la pensée, tandis que de l’autre il est une qualité de la pensée elle-même – pensée qui vise alors à la systématisation.

Quoiqu’il en soit de ces nuances, il me semble que la notion de système a soulevé lors de nos travaux préparatoires une même préoccupation chez les différents intervenants, qu’ils soient juristes ou scientifiques : celle de la confiance. Peut-on avoir confiance dans le système ? Que l’on appréhende le système construit par les algorithmes, en tant que tel, ou dans sa relation avec une pratique qu’il entend « disrupter », la mécanisation, l’automatisation, ou – plus globalement – la logicisation sont ou restent sources de méfiance.

C’est ainsi à travers la double problématique de la fiabilité et de la sincérité que nous avons décidé de converger à propos d’un objet d’intérêt commun, les systèmes Blockchain.
Il s’agissait pour le juriste d’adopter une approche critique suivi de longue date par la recherche en informatique visant à démythifier le caractère infaillible comme l’objectivité des systèmes informatisés.

Il existe un terme qui exprime très bien cela : celui de « système inéquitable numérique ». Le « SIN » a pour objet de désigner un système qui pêche par ce qu’il fait peser le coût de certains dysfonctionnements sur l’utilisateur – lequel sera évidemment la partie juridiquement et économiquement faible en cas de litige [^litige]

[^litige]: Il est possible de prendre un exemple topique avec le cas du défaut de validation d’un titre de transport : l’utilisateur ne peut pas prouver qu’il a bien entendu le composteur biper à la présentation de sa carte numérique.

Dans certains cas, c’est au législateur qu’il est revenu d’intervenir pour rétablir l’équité face au système. En vertu de la loi, c’est ainsi à la banque d’assumer l’essentiel des risques liés à l’utilisation de la carte bancaire (même en absence d’opposition, la responsabilité de l’utilisateur est limitée à 150 euros en vertu de l’art. L 133-19 du Code mon. et fin.).

# Confiance dans les systèmes blockchain #

Compte tenu du rôle de plus en plus prépondérant des solutions Blockchain dans l'organisation de la vie économique et sociale des citoyens,  nous avons souhaité investir la question de la fiabilité et de la sincérité à la suite du constat d’un point commun entre nos travaux initiaux.

## Présentation de la blockchain ##

La blockchain est perçue comme un composant d'une architecture logicielle permettant d'atteindre un consensus distribué pour les données transactionnelles sans recourir un un tiers de confiance. Ces systèmes consistent en une base de donnée permettant la lecture et l'ajout d'information sous forme d'une liste d'enregistrements chaînés appelés les blocks. Par construction, les systèmes de blockchain ne peuvent être falsifiés ou modifiés puisque chaque block contient un marqueur temporel couplé à un lien vers le block précédent.
La blockchain offre l'assurance que les données ne peuvent être modifiées rétroactivement une fois enregistrées.

Un tel consensus décentralisé peut être atteint à l'aide d'algorithmes tels que proof-of-work (preuve de travail), proof-of-stake (preuve d'enjeu) ou un algorithmes dit tolérant aux fautes Byzanines (BFT).
Les blockchain peuvent être utilisé dans une grande variété de cas d'utilisation tels que les transactions financières comme Bitcoin, les dossier médicaux ou encore le contrôle des réseaux.

Les implémentations les plus répandues des blockchain, telle celle utilisée pour le réseau Bitcoin, ont démontré leur efficacité dans la gestion de transactions très simples, comme l'échange de devises. Néanmoins, le manque de moyen technique permettant une programmabilité extensible à d'autres cas d'utilisation plus complexe ont conduit au développement d'une nouvelle génération de blockchain. Celle-ci étant la sémantique des transaction au travers l'utilisation de "Smart Contracts".

Paris les différents essais lancés à grande échelle sur les marchés, l’épisode de *The DAO* a constitué notre point d’entrée dans la problématique de la confiance des systèmes Blockchain.

## The DAO ou l'échec de la confiance ##

*The Dao* a été fondé le 30 avril 2016, en tant qu'organisation autonome décentralisée et formait un fond d'investissement piloté directement par ses actionnaires, en fournissant un nouveau business model décentralisé appliqué à l'organisation des entreprises commerciales et organismes sans but lucratif.

Au démarrage de l'activité, il a été techniquement déployé sur la blockchain Ethereum et était dépourvu de structure managériale ou de conseil d’administration. Son code est publié sous licence open-source. Issu d'un financement participatif, il a détenu le record de capitalisation pour ce type de création.
En Juin 2016, une vulnérabilité dans son code a permis à des utilisateurs malveillants de siphonner un tiers de la valeur du fond.

En Juillet 2016, la communauté Ethereum a décidé de revenir en arrière sur ces transactions délictueuses en les supprimant des ces registres. Dans la controverse, une partie de la communauté, opposée à ce "hard fork" continue de maintenir la blockchain Ethereum dans son état non modifié sous le nom d'Ethereum Classic. Les deux communautés s'opposent de façon quasi philosophique sur ce retour en arrière.

* La communauté pro-fork **Ethereum** soutient que l'intentionnalité du smart contrat défectueux n'avait pas été respectés, et que les détenteurs de the DAO n'avait pas exprimés leur accord sur les transactions frauduleuses. Par conséquent, pour
* La communauté anti-fork **Etherum Classic** soutient que le code contenu dans les smarts contracts représente le plus haut niveau de vérité, et qu'il fait loi (code is law). Ces représentants arguent également que la propriété d'immutabilité de la blockchain, sur laquelle repose la confiance des utilisateurs doit être garantie.

Dans la suite de cet article, nous proposons un modèle pragmatique qui est un compromis entre les deux approches. D'une part, puisque qu'il est impossible aujourd'hui de prouver mathématiquement qu'un smart contrat ne peut être exploité par un utilisateur malveillant à des fins contraires à l'intentionnalité de l'auteur du contrat, nous proposons d'exprimer un ensemble d'invariant très simples, permettant de s'assurer que les cas limites ne peuvent entraîner d'exploitation abusive. D'autre part, nous proposons qu'une fois que les invariants ont été vérifiés, les transactions soit inscrites dans la blockchain de manière immutable.

## code is law vs code by law  ##

Il s'agit d’envisager la possibilité de concevoir des Smart Contracts  « non directement et automatique imposables », en ajoutant au système un mécanisme d’appel ou d’arbitrage au stade de l’exécution du contrat.
Au-delà d’une réflexion sur les valeurs du cyberespace, à laquelle nous invite le constitutionnaliste américain Laurence Lessig depuis le début des années 2000, il y a un enjeu très pragmatique : comme ce fut le cas pour toute innovation du monde économique, depuis la monnaie scripturale à Airbnb, c’est sur la confiance que repose la capacité des smart contracts à se développer.

 En pratique, il existe deux voix essentielles et complémentaires afin d’assurer une bonne diffusion de cette nouvelle technologie : il faut tout d’abord travailler sur l’architecture du système, c'est-à-dire sur le code lui-même afin de sécuriser son fonctionnement et l’automatisation de ses fonctions. Il faut ensuite réfléchir à la manière dont le droit peut ou doit garantir les parties contractantes, non plus uniquement de la bonne exécution des engagements réciproques, mais de l’existence des conditions propres à garantir une bonne auto-exécution du contrat. Cela revient à adopter deux approches :
une première, « code is law », qui tire les conséquences du fait que pour tout système numérique, c’est d’abord sa conception qui régule son fonctionnement ;
une seconde, « code by law », qui s’interroge sur la capacité du droit à investir ce système afin d’y exercer son pouvoir normateur.

# Code is Law #

Les smarts contract sont généralement écrits à l'aide de langages de programmation non spécialisés [^@dannen2017introducing] afin de permettre au développeur les réalisant une productivité similaire au développement d'applications traditionnelles.
On peut concevoir les smart contracts comme l'éxecution de code déterministe ayant comme entrée un état donné de la blockchain et produisant des sorties également inscrites dans la blockchain.
Entrées et sorties peuvent être considérées comme un ensemble de valeurs rattachées à un compte utilisateur, les contrats permettant de transférer des valeurs d'un compte à un autre.

Face aux difficulté de prouver formellement les smarts contracts exprimés dans un langage de programmation spécifique

# Code by Law #
## Réfutation de l'hypothèse du non-droit ##
Pour rebondir sur les propositions de Nicolas et envisager quelle pourrait être la réaction du droit face à un Smart Contract, il faut commencer par rappeler que le système juridique cette fois-ci repose sur une loi fondamentale : celle de sa complétude. Au risque de faire du « panjuridisme », et à l’image de la nature qui a horreur du vide, le juriste, le juge, ou n’importe quel autre enquiquineur trouvera toujours des éléments de droit à appliquer à une situation de fait – fût-ce au prix d’une réflexion intense ou du recours à beaucoup d’imagination. Le droit n’est-il pas la plus puissante école de l’imagination nous disait Giraudaux ? (voir Klaus Peter Berger, The creeping codification of the new lex mercatoria, Kluwers, 2nd éd., 2010, p. 290). Pour ne prendre qu’un exemple, des concepts tel que celui de lex numerica ou de lex informatica sont ainsi venus accompagner le développement du commerce électronique.
Cette capacité inventive du droit, même dans des domaines où l’Etat est a priori peu présent, va directement à l’encontre du sentiment de liberté, voire d’impunité, qui prédomine bien souvent chez les promoteurs du cyberespace.  Les promoteurs de the DAO le définissent ainsi comme un « Paradis libertaire », échappant à tout cadre juridique... dès lors que la communauté formée n’aurait pas formellement d’existence.
Sans être expert en droit des sociétés, il me semble cependant que la notion de société créée de fait, par exemple, est tout à fait capable de contourner l’absence de personnalité juridique préexistante.
En réalité, les promoteurs du Smart Contracts font une double erreur : ils pensent d’une part que l’auto-exécution évite toute possibilité de contentieux, et d’autre part, que l’absence de contentieux est l’indicateur de l’a-juridicité de la situation smartcontractuelle.
Ce qui est vrai, par contre, c’est que l’identification de la juridiction compétente, l’identification de la loi applicable, mais aussi celle de la solution qu’elle implique, restent des questions épineuses et certainement source d’incertitudes pratiques. Si l’on peut alors parler de « non-droit », au sens d’« une baisse plus ou moins considérable de la pression juridique » (Carbonnier), cette baisse n’est qu’un phénomène transitoire et non pas un état stable.
Lors de travaux menés à bordeaux en 2016 par une équipe pluridisciplinaire, nous avons eu l’occasion de le constater à propos des monnaies virtuelles : critère de rattachement, statut pénal, qualification juridique sont autant de problématiques pour le moment largement non résolues à défaut d’un contentieux suffisant ou d’adoption de législation ad hoc.
De manière générale, le rapport entre la technologie numérique et le monde juridique est bien souvent biaisé dans les analyses proposées par les tenants des smart contracts. A titre d’exemple, Nick Szabo qui est des plus anciens promoteurs de cette technologie, considère que le contrat est un texte qui implicitement demande à un juge d’ordonner à une partie d’effectuer un paiement ou de livrer une prestation à l’autre sous certaines conditions. C’est une vision franchement très réductrice du contrat : elle prend l’hypothèse problématique de l’inexécution pour en faire l’essence du contrat. Pour reprendre l’analyse de Jean Carbonnier, elle n’envisage la vie du contrat que par la pathologie qui est susceptible de l’atteindre. Or, le Contrat a pour finalité première, à mon sens, de savoir à quoi l’on s’engage, de pouvoir déterminer la teneur de son engagement et les modalités de sa mise en œuvre. Ensuite, cette vision contentieuse du contrat simplifie à l’extrême en prenant un cas très particulier, l’absence d’exécution, comme seule hypothèse de saisine du juge. Bien souvent, l’exécution n’est pas quelque chose de binaire mais un continuum et tout l’enjeu en cas de litige sera d’interpréter le contrat afin de savoir à quoi s’étaient engagées les parties.
Pour en revenir au Smart Contracts non opposables proposés par Nicolas, je propose d’évoquer certaines des questions que le droit aura certainement à trancher en cas de développement de cette nouvelle technologie contractuelle.

## Adaptation du droit ##
La sécurité juridique, qui est la finalité de la construction juridique, pourrait imposer une intervention en amont et en aval  du déploiement d’un tel contrat. Si vous le voulez bien, je laisserai délibérément la question du lien de rattachement et on supposera par la suite que la compétence étatique est établie pour réguler les smart contracts et trancher les éventuels litiges.

### En amont ###

Je vois quatre points essentiels qui devraient justifier une intervention normative :
Il s’agit premièrement de la question du niveau de preuve de la fiabilité du système proposé. On peut penser que les smart contracts auront vocation à mettre en relation des parties entre lesquelles l’équilibre ne sera pas parfait, et qu’il sera parfois nécessaire de protéger celle qui se trouve en situation de dépendance. Asymétrie d’autant plus à craindre que le langage informatique du code est proprement incompréhensible pour le quidam... Il faut donc non seulement réfléchir au niveau de preuve requis à l’encontre de celui qui propose un smart contract, et par exemple s’interroger sur le recours à la validation formelle -  même si j’ai cru comprendre que c’était difficilement compatible avec l’open source ???,  mais il faut aussi s’interroger sur l’autorité compétente pour apprécier les informations fournies quant à la fiabilité du système et à la sincérité de l’information transmise. L’autorité des marchés financiers, qui veille à la protection de l'épargne et à l'information des investisseurs, ou encore le Mécanisme de surveillance unique mis en place par l’UE depuis la crise financière de 2008 et qui repose sur une mise en réseau de la BCE et des autorités nationales de contrôle prudentiel pourrait servir d’exemple.
Le modèle des autorités indépendantes en charge de la régulation d’un secteur d’activité me paraît en effet particulièrement adapté dans le cadre d’un domaine ultratechnique. En s’inspirant des mécanismes d’autorisations de mise sur le marché délivrées dans le secteur du médicament ou des variétés végétales par exemple, il est possible d’inventer une procédure de validation ou d’agrément applicable aux Smart Contracts.
Reste à savoir ensuite sur qui devrait reposer la responsabilité en cas de défaillance du système et à déterminer s’il convient d’envisager une obligation de moyen ou de résultat quant l’exigence de fiabilité...
Deuxième préoccupation que soulève la proposition de Nicolas : le statut de l’information. On voit que dans l’exécution de l’obligation contractuelle, l’information fournie par l’oracle est primordiale. Pour le juriste, le constat que les faits sont parfois prépondérants dans l’application de la règle de droit n’est pas une découverte. C’est tout l’enjeu de l’appréciation des faits ou de la qualification juridique. Bref, on peut s’interroger sur la nécessité de garantir la neutralité de l’information. Cette exigence peut même se décomposer en deux branches : neutralité dans le choix de l’oracle tout d’abord, et si l’on pense contrat d’adhésion et asymétrie du pouvoir contractuel on voit bien que le choix sera souvent imposé aux particuliers cocontractants, et neutralité du contenu de l’information, c'est-à-dire objectivité des données transmises
En étant un peu cynique, on peut se demander dans le cas du billet de train si l’Etat actionnaire unique de l’EPCI SNCF, n’aurait pas intérêt à ce que l’EPA Météo France soit généreux avec ses deniers – et réciproquement...
Là encore, le modèle de l’autorité administrative indépendante apparaît comme une piste intéressante...
Troisièmement, le droit devrait s’intéresser a fortiori au statut de l’arbitre.  D’abord et évidemment, il s’agit comme pour l’oracle de s’intéresser à son objectivité et à son indépendance vis-à-vis des parties dans une situation où bien souvent le smart contracts sera un contrat d’adhésion. On peut penser qu’à l’image de certaines clauses contractuelles existantes aujourd’hui qui méconnaissent l’ordre public, la loi devrait interdire certaines pratiques abusives comme par exemple le fait de confier l’examen de l’appel à une partie prenante au contrat.
Ensuite, il n’est pas inutile de se demander si l’arbitre ne doit pas être soumis à un certain nombre d’obligation déontologique. Par ex, dans le cas d’un contrat d’assurance vie, l’arbitre va être amené à manipuler des données personnelles couvertes en France par le secret médical... il faut donc trouver les moyens d’assurer le respect des obligations professionnelles en la matière. Dans cette hypothèse, l’arbitre devrait être un médecin-conseil comme c’est le cas pour l’assurance traditionnelle.
Enfin, en quatrième point, je voudrais revenir sur l’hypothèse du vol de clé évoqué par Nicolas comme un risque pour la sécurité des Smart Contracts. Le risque est d’autant plus grand dans le cas de recours par les particuliers à des logiciels de communication avec la blockchain que l’on désigne « wallet ». Ceux-ci stockent en effet l’information et sont susceptibles d’être piratés.
Pour endiguer ce risque, dans le cadre des monnaies virtuelles, l’Etat de New York a été le premier en 2014 a imposé un mécanisme de licence aux opérateurs du secteur. En vertu de cette « bitlicence », les plates-formes se voient imposer des obligations prudentielles, mais elles doivent également faire la preuve de la solidité de leur système informatique et de l’adoption de protocoles destinés à contrer les tentatives de piratage. Une fois obtenu l’agrément, elles restent tenues à l’obligation de présenter un rapport annuel.
Une telle construction est tout à fait transposable aux cas d’utilisations de clé pour souscrire ou activer des smart contracts via l’utilisation de Wallet.

### En aval ###

Si l’intervention ex ante de la règle de droit est de nature à éviter un certain nombre de complications, il n’empêche que l’exécution du Smart Contracts, tout automatique qu’elle soit, peut être source de contestations.
  - Legal enforceability of smart contracts is limited. Work
  is being done [84]) to make the technical rules of smart
  contracts legally enforceable and binding to all parties. Until
  then, what happens if, despite the verifiability of the whole
  process, a transacting entity disputes the outcome of a smart
  contract operation? A way to increase the chances of legal
  enforceability is to include a reference to the actual real-world
  cess called ‘‘dual integration’’ [85] and it works as follows:
  contract in the smart contract, and vice versa. This is a pro-
  the blockchain, and include that address in the real contract
  (a) deploy the smart contract in question, record its address on
  (b) hash the corresponding real-world contract, record its
  hash digest, store the real contract in a safe space (can be
  centralized, or decentralized [86]), (c) send a transaction to
  the smart contract that includes the real contract’s hash in its
  metadata; the contract then stores that piece of information
  in its own, internal database.11 In case of a legal dispute,
  you can point to the hash stored in the smart contract, then
  present the real-world contract (that is uniquely identified
  blockchain and the expected outcome in the physical world.
  by that hash) and prove the link between the actions on the
  Refer to CommonAccord [87] and Legal Markdown [85];
  both tools intend to make the creation of legal ‘‘real-world’’
  and corresponding smart contracts possible, via the use of
  templating systems.
→ est-ce bien nécessaire ! ? Tjrs cette idée sous-jacente qu’en soit le SC n’est pas un contrat... et reste a-juridique.
A quoi s’engage-t-on ? à l’output prime ou à l’output prévisible ? Comment rendre opposable l’output ? validation de l’output avant d’être inscrit sur blockchain (avec un output temporaire non-opposable qui va être passer par un autre contrat pour au bout d’un certain délai devenir opposable → possibilité de rétractation)
Est-ce que ça devient pas un contrat purement potestatif ?*

# Ouverture
Dans le cas du développement du commerce électronique international, la doctrine a utilisé les concepts de lex electronica  pour désigner l’apparition de normes informelles, de codes de bonnes pratiques, adoptés par les acteurs du secteur généralement regroupés en organisations transnationales plutôt que par les autorités étatiques. Il faut donc s’interroger en conclusion sur le caractère transposable de ce précédent au cas des Smart Contracts. Interrogation d’autant plus nécessaire que l’on observe effectivement dans le cadre d’initiative comme celle d’Hyperledger ou de clause.io une volonté des acteurs du milieu de coopérer pour établir des standards. → opensource : développement d’une stratégie d’occupation par IBM (pouvoir de marché !)
Techno-legal standards v. organisation privée à l'origine de la standardisation [standardization is one of the many benefits and drivers of open source software development]
Objectifs dans le recours aux standards (auxquels peut renvoyer la loi): The aim is to produce a technology layer that will advance the transition to legally enforceable smart contracts by incorporating widely accepted standards relating to transactional legal practice, the use of data and distributed ledgers in contracting, and dispute resolution.
inconvénient des standards: ils peuvent rester définis par les seuls acteurs du marché, et donc par les plus gros d'entre eux (ex de hyperledger: Si IBM a décidé de transmettre ses connaissances au projet open-source, c'est que l'entreprise s'est rapidement rendue compte qu'elle avait besoin d'un consortium pour pousser l'adoption de sa technologie. "La dimension de standardisation est primordiale, reconnaît Luca Comparini. Il est important que la technologie sur laquelle nous travaillons soit adoptée par une large communauté. Travailler sur Hyperledger est un investissement pour le futur : nous apportons de la valeur à la communauté et à terme IBM sera dans une très bonne position pour aider ses gros clients à se transformer en adoptant la technologie." --> l'open source est un moyen de diffuser son approche pour IBM :  "A terme, si la technologie Hyperledger perce, IBM sera l'un des seuls acteurs si ce n'est le seul à pouvoir vraiment manipuler le code et créer des applications", affirme Alexandre Stachtchenko. Même clause.io qui promeut abstraitement les standards sur divers support de communication (même revue scientifique via Houman Shadab) est partie-prenante en tant que société de conseils dans le legal tech: chercher moi à imposer des standards que des modèles de contrats)

C’est tjrs par un élément extérieur au système que vient la confiance, car c’est l’extériorité qui continue d’apparaître comme la garantie de son bon fonctionnement (expert qui procède à la vérification formelle, Oracle, Arbitre, Etat, etc...)

# Reference
