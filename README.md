# projectagl

1.Introduction du projet :


Choix du sujet et description générale :


La domotique représente un système innovant qui offre la possibilité de gérer et d'automatiser divers équipements domestiques tels que l'éclairage, le chauffage, la climatisation, les serrures et les appareils électroménagers. 


Notre domotique aura le nom de CasaControl.


Son objectif premier est d'améliorer le confort, la praticité et l'efficacité énergétique de la maison.


Motivations :


Même si ce projet n’était pas notre premier choix, mais cette technologie a captivé notre intérêt pour plusieurs raisons : 


-	Selon une enquête de Vodafone, 84% des entreprises utilisent l'IoT dans leur activité en 2021. Puisque l'IoT fournit les bases technologiques nécessaires à la création de systèmes domotique, on doit être plus informé sur ces deux domaines.
-	On veut en savoir plus sur la domotique.
-            On veut travailler sur un système qui respecte l’environnement.
-	Le comfort est l’un des besoins essentiels des clients de nos jours. C’est pour cela qu'on veut être renseigné sur ce système tant demandé.
-            Les personnes en situation de handicap et les personnes âgées ont parfois des difficultés, voire même une incapacité totale à effectuer les activités quotidiennes de manière autonome.




Le périmètre du projet :


Le projet CasaControl vise à développer un système domotique complet et personnalisable, offrant une gamme variée de fonctionnalités pour répondre aux besoins individuels des utilisateurs. 

Les services attendus par l’utilisateur, qui sont regroupés sous le terme "domotique", concernent principalement 
:
Le confort (commande à distance d'appareils ou équipements,..).
La sécurité (protection contre les intrusions, détection d'incendie. 
L'économie d'énergie (gestion du climatiseur, d’éclairage..).

En effet, notre système permet de piloter d’une façon simple et confortable l’ensemble
des équipements électriques notamment :l’éclairage, les ouvrants et le système d'alarme.

De plus, l’utilisateur a besoin d’un tel système de pilotage, lorsqu’il est engagé dans
son travail. Par exemple, lorsqu’il part le matin de son logement, il peut oublier de désactiver
le climatiseur ou d’ouvrir les fenêtres. En outre, lorsque l’utilisateur sort en déplacement
inattendu, il peut oublier aussi d’activer le système alarme.
Donc, le but de notre application est de surmonter ces problèmes en offrant le service
« CasaControl » avec lequel il peut, par une simple application de son téléphone portable ou
bien son ordinateur commander les équipements électriques de son domicile à distance.


L’ interface de l’utilisateur permet d’indiquer l’état et de piloter les équipements électriques suivants :

Les portes (porte garage, porte principale…).
Les fenêtres
Le système alarme.
L’éclairage (les lampes).
Les climatiseurs.
La télévision

Cette application sera embarquée dans le Raspberry Pi.





2.Spécifications du projet :

a) Notions de base et contraintes du projet :


Les systèmes domotiques se basent sur l'utilisation de capteurs, d'actionneurs et de contrôleurs pour surveiller l'environnement domestique et prendre des décisions en fonction des données collectées. 

Par exemple, un capteur de mouvement peut détecter la présence de personnes dans une pièce et réguler automatiquement l'éclairage.


La domotique permet un contrôle à distance via des appareils tels que les smartphones, tablettes ou ordinateurs, offrant ainsi aux utilisateurs la possibilité de gérer leurs équipements même lorsqu'ils sont absents.



Les contraintes peuvent être des obstacles à ces notions de ce système, tels que :


L’intégration étroite de capteurs (par exemple, capteurs de mouvement, détecteurs de fumée) et d'une variété d’actionneurs (comme les lumières, les serrures intelligentes).

La nécessité de télécharger un programme informatique pour établir la communication avec le système domotique et contrôler les appareils connectés.

La réactivité en temps réel du système pour garantir un contrôle et une surveillance efficaces des équipements connectés, incluant des critères tels que le temps de réponse, la gestion énergétique..

La communication avec les dispositifs de manière cohérente et fiable, en prenant en compte les protocoles de communication spécifiques à chaque dispositif.

La collecte, le traitement et l’analyse efficaces de grandes quantités de données afin de fournir des fonctionnalités telles que l'automatisation des tâches, la détection d'anomalies..


La mise en œuvre des protocoles de sécurité robustes pour protéger les données sensibles sur la vie privée et la sécurité des utilisateurs en transit et au repos, ainsi que pour sécuriser l'accès aux appareils connectés.

Le fonctionnement de manière fiable, même dans des conditions imprévues ou en cas de défaillance d'un composant.


Considération des besoins et des préférences des utilisateurs dans la conception des interfaces utilisateur pour qu’elles soient conviviales, faciles à utiliser et intuitives .

b) Description des acteurs et fonctionnalités attendues du projet :




Notre système domotique va offrir une gamme variée de fonctionnalités répondant aux besoins et aux préférences individuels des utilisateurs.


Notre projet possède un seul type d’acteur qui est l’utilisateur.


L’utilisateur : cet acteur a le droit de se servir de notre plateforme domotique à distance ou
localement en utilisant son téléphone portable ou bien son ordinateur. Il interagit avec le logiciel via une interface utilisateur graphique (IHM).


Voici une description détaillée des fonctionnalités présentées :


Contrôle de l'éclairage : possibilité d'allumer/éteindre des lumières.


Gestion de l’économie de  l'énergie : optimisation de la consommation énergétique en régulant les équipements selon les besoins réels et en détectant les gaspillages.


Surveillance de la maison, en temps réel et à distance : détection des intrusions, des fuites d'eau, des incendies, etc., grâce à des capteurs et des caméras de surveillance avec stockage des enregistrements ( dans le cloud ou sur un support local ) et réception des alertes lors des scénarios anormaux ( via des appareils connectés sur smartphone ou ordinateur par exemple ).


Automatisation des tâches : la possibilité d’ouvrir/ fermer les portes et les volets, à distance pour les visiteurs autorisés. 


3) Les diagramme de cas d’utilisation :


a)Diagramme de cas d’utilisation générale de notre système domotique :


A ce stade là, nous présentons le diagramme de cas d’utilisation général de notre système domotique
indiqué dans
 la figure 1 :
![CAP]![Capture d'écran 2024-04-29 123711](https://github.com/nouhabennasr/projectagl/assets/168307999/10896dd5-e7a6-442d-9776-060e61a69d9c)
![CAP]![Capture d'écran 2024-04-29 123822](https://github.com/nouhabennasr/projectagl/assets/168307999/564c1f74-87ab-438c-967b-926b696263a3)


L’utilisateur doit s’authentifier afin de pouvoir gérer la liste des équipements électriques soit à distance soit localement.


b)Diagramme de cas d’utilisation restreint de notre système domotique :


Le fonctionnement de notre système domotique peut être décrit par le cas d’utilisation de la figure 2 :
![CAP]![Capture d'écran 2024-04-29 124001](https://github.com/nouhabennasr/projectagl/assets/168307999/d1e30396-a8e0-44fa-a6da-d713145cd438)
![cap]!![image](https://github.com/nouhabennasr/projectagl/assets/168307999/f2968004-36d1-4706-a59c-fc408cb048ce)

La figure 2 résume les cas d’utilisation de l’utilisateur : « gérer la plateforme domotique » :

«Configurer les équipements électriques » : l’utilisateur peut définir les paramètres et les fonctionnalités de l'équipement pour une utilisation et un contrôle appropriés.

«Consulter les états des équipements électriques » : l’utilisateur peut visualiser l’état de chaque équipement électrique du système domotique.

«Piloter les différents équipements électriques » : l’utilisateur peut démarrer ou arrêter chacun des équipements électriques du système domotique à distance ou localement. Par exemple allumer/éteindre une lampe, ouvrir/fermer un volet, activer/désactiver le système d’alarme ou bien régler la température dans les 
différentes pièces…

«Afficher la liste des équipements électriques » :  l’utilisateur peut voir la liste des équipements électriques.

«Ajouter des équipements électriques » :  l’utilisateur peut intégrer physiquement et initialement l'équipement au système domotique afin de rendre l'équipement visible et accessible au système domotique.

«Supprimer des équipements électriques » :  l’utilisateur peut supprimer l’équipement électrique.

c)Diagramme de cas d’utilisation détaillé de “Piloter les équipements électriques” :


Le fonctionnement de pilotage de la plateforme domotique peut être décrit par le cas
d’utilisation. En effet, l’utilisateur distant a le choix de démarrer, arrêter les équipements
électriques de notre système domotique.
![cap]!![image](https://github.com/nouhabennasr/projectagl/assets/168307999/01afe037-1c47-4f70-bc05-4d6aafe18ac3)


« Activer un équipement électrique» :l’utilisateur peut allumer une lampe, ouvrir un volet ou bien activer le système d’alarme.

« Désactiver un équipement électrique» : l’utilisateur peut éteindre une lampe, fermer un volet ou bien désactiver le système d’alarme.

« S’authentifier » : l’utilisateur doit s’authentifier.


d)Diagramme de cas d’utilisation détaillé  :


Le diagramme ci-dessous représente les fonctionnalités principales du système CasaControl, une plateforme de gestion domotique permettant aux utilisateurs de contrôler efficacement leurs équipements électriques.


![cap]!![image](https://github.com/nouhabennasr/projectagl/assets/168307999/0f6154a3-e3a2-4ee8-a5f2-29ff7354a11a)

![cap]!![Capture d'écran 2024-04-29 124559](https://github.com/nouhabennasr/projectagl/assets/168307999/96fd6a8d-ee32-4f9a-9e52-129b8dfe500b)

S'authentifier :
Permet à l'utilisateur de se connecter au système CasaControl, assurant ainsi la sécurité et l'accès contrôlé aux fonctionnalités.

Activer un équipement électrique :
L'utilisateur peut activer un équipement électrique sélectionné dans le système.

Désactiver un équipement électrique :
L'utilisateur peut désactiver un équipement électrique sélectionné dans le système.

Piloter les différents équipements électriques :
L'utilisateur peut contrôler divers aspects des équipements électriques tels que la puissance, la température et la vitesse, et est inclus dans plusieurs autres cas d'utilisation.

Afficher la liste des équipements :
Offre à l'utilisateur une vue globale de tous les équipements connectés, facilitant ainsi la gestion et le suivi.

Consulter les états d'un équipement électrique :
Permet à l'utilisateur de visualiser l'état actuel d'un équipement électrique, ce qui est essentiel pour surveiller les performances et diagnostiquer les problèmes éventuels.

Ajouter un équipement électrique :
L'utilisateur peut ajouter un nouvel équipement électrique au système en saisissant les informations nécessaires telles que le type, la marque et le modèle.

Supprimer un équipement :
L'utilisateur peut supprimer un équipement électrique existant du système.

Configurer un équipement électrique :
L'utilisateur peut configurer les paramètres d'un équipement électrique existant tels que son nom, sa description et son groupe.


4)Élection des cas d’utilisation pour le sprint 1; Priorité des cas d’utilisation :


Dans l'ordre de priorité des cas d'utilisation pour un système domotique, l'ajout d'un équipement est placé en première position ( must ) , suivi de la liste des équipements disponibles (required )  et enfin de l'activation des équipements ( must ).

Cette hiérarchisation reflète l'importance de répondre aux besoins immédiats et spécifiques des utilisateurs, en accordant la priorité à l'extension du système avec de nouveaux équipements ( haute priorité ),  à leur activation pour une utilisation effective ( haute priorité) et à l’affichage de la liste des équipements ( priorité moyenne ).

→Ainsi, ajouter un équipement est crucial pour offrir une expérience utilisateur optimale, suivi par l’activation des équipements disponibles, tandis que l’affichage des équipements répond aux besoins immédiats des utilisateurs, contribuant ainsi à une gestion proactive de l'environnement domestique.



Description du cas d'utilisation : Ajouter un équipement


Acteur principal : Utilisateur


Préconditions :






L'utilisateur est connecté au système CasaControl : login (non nul et non vide ) et mot de pass ( non nul et non vide )


Le client existe.


Le système affiche un formulaire à remplir avec les informations nécessaires telles que le type, la marque, le modèle, etc. ( champs non vides et non nuls )


L’équipement n'existait pas auparavant.




Login(¬ null ∧ ¬ vide)(Λ)Mot de passe(¬ null ∧ ¬ vide)(Λ)client existe(Λ)champs(¬ null ∧ ¬ vide)(Λ)équipement inexistant




Post-conditions : Ajout d’un équipement établi 


Le nouvel équipement électrique est ajouté avec succès au système CasaControl et est prêt à être utilisé par l'utilisateur.








