# projectagl
![OIP (1)](https://github.com/nouhabennasr/projectagl/assets/168307999/2cf9d151-cd67-432a-b903-d422a4ab9f8f)



****************************************
Ministère de l’Enseignement Supérieur
****************************************
Université de Carthage
****************************************
Institut des Hautes Etudes Commerciales de Carthage
****************************************
![Blue Minimalist Smart Home Logo Design](https://github.com/nouhabennasr/projectagl/assets/168307999/49cbe121-3e0b-4258-86e2-a9721849046d)

Atelier de Génie Logiciel : Document de specification, conception preliminaire 
                            conception detaillée et preparation de tests unitaires 

                 Réalisé par :Nouha ben nasr ,Salima Boudinar et Ines Mazgar


 🚩 1.Introduction du projet :


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





 🚩 2.Spécifications du projet :

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


 🚩3) Les diagramme de cas d’utilisation :


a)Diagramme de cas d’utilisation générale de notre système domotique :


A ce stade là, nous présentons le diagramme de cas d’utilisation général de notre système domotique
indiqué dans
 la figure 1 :
 ![cas d'utilisation général](https://github.com/nouhabennasr/projectagl/assets/168307999/e7c5688b-f368-4f21-ba2b-b2f24959f242)

![Capture d'écran 2024-04-29 123822](https://github.com/nouhabennasr/projectagl/assets/168307999/564c1f74-87ab-438c-967b-926b696263a3)


L’utilisateur doit s’authentifier afin de pouvoir gérer la liste des équipements électriques soit à distance soit localement.


b)Diagramme de cas d’utilisation restreint de notre système domotique :


Le fonctionnement de notre système domotique peut être décrit par le cas d’utilisation de la figure 2 :
![Capture d'écran 2024-04-29 124001](https://github.com/nouhabennasr/projectagl/assets/168307999/d1e30396-a8e0-44fa-a6da-d713145cd438)
![image](https://github.com/nouhabennasr/projectagl/assets/168307999/f2968004-36d1-4706-a59c-fc408cb048ce)

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
![image](https://github.com/nouhabennasr/projectagl/assets/168307999/01afe037-1c47-4f70-bc05-4d6aafe18ac3)


« Activer un équipement électrique» :l’utilisateur peut allumer une lampe, ouvrir un volet ou bien activer le système d’alarme.

« Désactiver un équipement électrique» : l’utilisateur peut éteindre une lampe, fermer un volet ou bien désactiver le système d’alarme.

« S’authentifier » : l’utilisateur doit s’authentifier.


d)Diagramme de cas d’utilisation détaillé  :


Le diagramme ci-dessous représente les fonctionnalités principales du système CasaControl, une plateforme de gestion domotique permettant aux utilisateurs de contrôler efficacement leurs équipements électriques.


![image](https://github.com/nouhabennasr/projectagl/assets/168307999/0f6154a3-e3a2-4ee8-a5f2-29ff7354a11a)

![Capture d'écran 2024-04-29 124559](https://github.com/nouhabennasr/projectagl/assets/168307999/96fd6a8d-ee32-4f9a-9e52-129b8dfe500b)

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


 🚩 4)Élection des cas d’utilisation pour le sprint 1; Priorité des cas d’utilisation :


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

| Pré condition                        | Test 1 | Test 2 | Test 3 | Test 4 | Test 5 | Test 6 |
|-------------------------------------|--------|--------|--------|--------|--------|--------|
| login (non nul et non vide)         | F      | T      | T      | T      | T      | T      |
| mot de passe (non nul et non vide)  |        | F      | T      | T      | T      | T      |
| client existe                       |        |        | F      | T      | T      | T      |
| champs (non nuls et non vides)      |        |        |        | F      | T      | T      |
| équipement inexistant               |        |        |        |        | F      | T      |
| *Post condition*                    | *Test 1* | *Test 2* | *Test 3* | *Test 4* | *Test 5* | *Test 6* |
| ajout d’un équipement à CasaControl| F      | F      | F      | F      | F      | T      |
|-------------------------------------|--------|--------|--------|--------|--------|--------|
| Nombre de jeux de tests             | 2      | 2      | 1      | n*2    | 1      | 1      |

Description du cas d'utilisation : Activer un équipement électrique


Acteur principal : Utilisateur


Préconditions :


L'utilisateur est connecté au système CasaControl : login (non nul et non vide ) et mot de pass ( non nul et non vide )


Le client existe.


L’équipement est existant.


L'équipement est fonctionnel.


L’équipement est désactivé.


Login(¬ null ∧ ¬ vide)(Λ)Mot de passe(¬ null ∧ ¬ vide)(Λ) client existant(Λ) équipement existant (Λ) équipement fonctionnel (Λ) équipement désactivé


Post-conditions : Équipement activé


Si l'activation est réussie, un message de confirmation "Équipement activé" est affiché à l'utilisateur et l'état de l'équipement est mis à jour.
Si l'activation échoue, un message d'erreur indiquant la cause de l'échec est affiché à l'utilisateur.


Table de décision des tests de validation :
| Pré condition                     | Test 1 | Test 2 | Test 3 | Test 4 | Test 5 | Test 6 | Test 7 |
|----------------------------------|--------|--------|--------|--------|--------|--------|--------|
| login (non nul et non vide)      | F      | T      | T      | T      | T      | T      | T      |
| mot de passe (non nul et non vide) |        | F      | T      | T      | T      | T      | T      |
| client existe                    |       |        | F      | T      | T      | T      | T      |
| équipement existant              |        |        |        | F      | T      | T      | T      |
| équipement fonctionnel           |        |        |        |        | F      | T      | T      |
| équipement désactivé             |        |      |     |      |       |  F |     T |
|----------------------------------||        |        |        |        |      |      |
| *Post condition*                 |      |      |      |       |       |       |       |
|equipement activé                 | F      | F      | F      | F      | F      | F      | T      |
| Nombre de jeux de test           | 2      | 2      | 1      | 1      | 1      | 1      | 1      |



Description du cas d'utilisation : Consulter la liste des équipements électriques

Acteur principal : Utilisateur
Préconditions :

L'utilisateur est connecté au système CasaControl : login (non nul et non vide ) et mot de pass ( non nul et non vide )

Le client existe.

Des équipements existent. 

Login(¬ null ∧ ¬ vide)(Λ)Mot de passe(¬ null ∧ ¬ vide)(Λ) client existant(Λ) équipements existants

Post-conditions :

La liste des équipements électriques est affichée à l'utilisateur.

Table de décision des tests de validation :

| Pré condition                     | Test 1 | Test 2 | Test 3 | Test 4 | Test 5 |
|----------------------------------|--------|--------|--------|--------|--------|
| login (non nul et non vide)      | F      | T      | T      | T      | T      |
| mot de passe (non nul et non vide) |        | F      | T      | T      | T      |
| client existe                    |        |        | F      | T      | T      |
| équipement existant              |        |        |        | F      | T      |
|----------------------------------|        |        |        |        |        |
| *Post condition*                 |        |        |        |        |        |
| affichage de la liste des équipements à CasaControl | F | F | F | F | T |
| Nombre de jeux de test           | 2      | 2      | 1      | n      | 1      |


5). Scénarios d’utilisation des cas d’utilisation ( bonus ):


Scénario 1 : Configuration des paramètres d'un équipement existant


Acteur principal : Utilisateur


Préconditions : 


L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à la section de configuration des équipements électriques dans le système CasaControl.


L'utilisateur sélectionne l'équipement électrique qu'il souhaite configurer.


Le système affiche les détails de l'équipement sélectionné, y compris son nom, sa description et ses paramètres actuels.


L'utilisateur modifie les paramètres de l'équipement selon ses besoins, tels que son nom, sa description, ou d'autres paramètres spécifiques à cet équipement.


Après avoir effectué les modifications, l'utilisateur confirme ses changements.


Le système enregistre les nouvelles configurations de l'équipement électrique.


Postconditions : 


Les paramètres de l'équipement électrique sont mis à jour conformément aux modifications apportées par l'utilisateur.


Scénario 2 : Ajout d'un nouvel équipement électrique


Acteur principal : Utilisateur


Préconditions : 


L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à la section d’ajout des équipements électriques dans le système CasaControl.


Le système affiche un formulaire à remplir avec les informations nécessaires telles que le type, la marque, le modèle, etc.


L'utilisateur remplit le formulaire avec les détails de l'équipement à ajouter.


Après avoir saisi les informations requises, l'utilisateur confirme l'ajout de l'équipement.


Le système valide les informations et ajoute le nouvel équipement à la liste des équipements électriques.


Postconditions : 


Le nouvel équipement électrique est ajouté avec succès au système CasaControl et est prêt à être utilisé par l'utilisateur.


Scénario 3 : Suppression d'un équipement électrique existant


Acteur principal : Utilisateur




Préconditions :


 L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à la section de suppression des équipements électriques dans le système CasaControl.


L'utilisateur sélectionne l'équipement électrique qu'il souhaite supprimer de la liste.


Le système affiche une confirmation de suppression pour l'équipement sélectionné, demandant à l'utilisateur de confirmer son choix.


L'utilisateur confirme sa décision de supprimer l'équipement électrique.


Le système traite la demande de suppression et retire l'équipement électrique de la liste.


Postconditions :


 L'équipement électrique sélectionné est supprimé avec succès du système CasaControl, et ses données associées sont effacées de la base de données du système.




Scénario 4 : Activation d'un équipement électrique


Acteur principal : Utilisateur


Préconditions : 


L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à la liste de pilotage des équipements électriques disponibles dans le système CasaControl.


L'utilisateur recherche et sélectionne l'équipement électrique qu'il souhaite activer.


Le système affiche l'état actuel de l'équipement, qui est probablement désactivé.


L'utilisateur sélectionne l'option pour activer l'équipement et précise “Activer”.


Le système envoie la commande d'activation à l'équipement sélectionné.


L'équipement reçoit la commande et passe à l'état activé.


Postconditions : 


L'équipement électrique sélectionné est activé et prêt à être utilisé par l'utilisateur.


Scénario 5 : Désactivation d'un équipement électrique


Acteur principal : Utilisateur


Préconditions : 


L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à la liste de pilotage des équipements électriques disponibles dans le système CasaControl.


L'utilisateur recherche et sélectionne l'équipement électrique qu'il souhaite désactiver.


Le système affiche l'état actuel de l'équipement, qui est probablement activé.


L'utilisateur sélectionne l'option pour désactiver l'équipement et sélectionne “Désactiver”.


Le système envoie la commande de désactivation à l'équipement sélectionné.


L'équipement reçoit la commande et passe à l'état désactivé.


Postconditions :


 L'équipement électrique sélectionné est désactivé et arrête son fonctionnement.


Scénario 6 : Affichage de la liste des équipements


Acteur principal : Utilisateur


Préconditions : 


L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à la section d’affichage des équipements électriques dans le système CasaControl.


Le système affiche la liste complète de tous les équipements électriques connectés.


L'utilisateur examine la liste pour voir tous les équipements disponibles.


Postconditions : 


L'utilisateur a une vue globale de tous les équipements électriques connectés, ce qui facilite la gestion et le suivi.


Scénario 7 : Consultation de l'état d'un équipement électrique
Acteur principal : Utilisateur


Préconditions : 


L'utilisateur est connecté au système CasaControl.


L'utilisateur accède à consultation des états des équipements électriques disponibles dans le système CasaControl.


L'utilisateur sélectionne l'équipement électrique dont il souhaite consulter l'état.


Le système affiche l'état actuel de l'équipement, y compris des informations telles que l'alimentation, la température, etc.


L'utilisateur examine l'état de l'équipement pour surveiller ses performances ou diagnostiquer d'éventuels problèmes.


Postconditions :


 L'utilisateur a visualisé avec succès l'état actuel de l'équipement électrique sélectionné, ce qui lui


6.Suivi du projet avec Classroom et GitHub :

Les spécifications sont consultables sur le fichier Markdown « readme.md » à la racine de notre projet GithubAGL et le diagramme de cas d’utilisation « * .pu » dans un répertoire Diagrammes.


Aspect statique :

Description textuelle des classes principales :

Un utilisateur peut avoir une ou plusieurs maisons intelligentes.

Un utilisateur est associé à une box domotique.

Une maison est la propriété d’un utilisateur ou plus.

Chaque maison ne peut avoir qu’une box et une box ne peut avoir qu’une seule maison.

Une box contrôle plusieurs actionneurs et plusieurs capteurs.


Une box détecte une ou plusieurs alertes.

Une box domotique est associée à une liste de capteurs et d'actionneurs.

Une box domotique agrège les données des capteurs.

Une box domotique contrôle les actionneurs.  

Une alerte est détectée par un et une seule box.

Un capteur ou un actionneur n’est connecté qu’à une box. 
| Classe        | Attribut          | Type    | Visibilité |
|---------------|-------------------|---------|------------|
| Smart_home    | idsmarthome       | integer | privé      |
|               | nom               | string  | privé      |
| Box_domotique | idboxdomotique    | integer | privé      |
|               | nomboxdomotique   | string  | privé      |
| Actionneur    | id                | integer | privé      |
|               | nom               | string  | privé      |
|               | position          | string  | privé      |
|               | description       | string  | privé      |
| Equipement    | idEquipement      | integer | privé      |
|               | nomEquipement     | string  | privé      |
|               | typeEquipement    | string  | privé      |
| Pièce         | idPiece           | integer | privé      |
|               | nomPiece          | string  | privé      |
|               | étage             | string  | privé      |
| Capteur       | idCapteur         | integer | privé      |
|               | nomCapteur        | string  | privé      |
|               | positionCapteur   | string  | privé      |
|               | descriptionCapteur| string  | privé      |
| Utilisateur   | idUtilisateur     | integer | privé      |
|               | nom               | string  | privé      |
|               | prénom            | string  | privé      |
|               | login             | string  | privé      |
|               | motDePasse        | string  | privé      |
|               | email             | string  | privé      |
| Alerte        | idAlerte          | integer | privé      |
|               | nomAlerte         | string  | privé      |
|               | dateAlerte        | string  | privé      |
|               | typeAlerte        | string  | privé      |

Description textuelle :

        Le diagramme de classe présenté représente les relations entre les différentes classes d'un système domotique “ CasaControl “.. Il met en évidence les relations reliant les classes.

Utilisateur : Identifié par un ID unique, il possède des informations telles que le nom, le prénom, le login, le mot de passe et l'email. Il peut s'authentifier dans le système.

Actionneur : Il agit sur l'environnement en fonction des commandes. Chaque actionneur possède un ID, un nom, une position et une description.

Capteur : Classe abstraite représentant divers types de capteurs (consommation, éclairage, température, etc.). Les sous-classes spécifient les types de détection. Chaque capteur possède un ID, un nom, une position et une description, avec des méthodes pour envoyer un signal et démarrer/terminer une exécution.

Box Domotique : Elle coordonne les dispositifs de la maison intelligente, possédant un ID et un nom.

SMART HOME : Représente le patron de conception (façade), avec des références vers l'utilisateur, les actionneurs, les capteurs et la box domotique. Il offre des méthodes pour vérifier le contrôle du système.

Équipement : Classe abstraite représentant les équipements de la maison (lampe, climatisation, alarme, etc.), avec des sous-classes spécifiant les types d'équipements. Chaque équipement possède un ID, un nom, un type, une marque, un mode de fonctionnement et une référence vers la pièce où il est installé.

Pièce : Représente les différentes pièces de la maison, possédant un ID, un nom, un numéro d'étage et une superficie. Elle offre une méthode pour afficher les équipements présents.

Alerte : Générée par le système en cas de situation inhabituelle, chaque alerte possède un ID, un nom, une date et un type.

Actionneur: Représente un actionneur générique qui peut effectuer des actions sur les équipements.

Utilisateur: Représente un utilisateur du système domotique qui peut interagir avec la box et les équipements.               


![diag rendu 2](https://github.com/nouhabennasr/projectagl/assets/168307999/c311bf17-b57e-4a3c-b144-63be08ac7554)


![Capture d'écran 2024-04-29 192213](https://github.com/nouhabennasr/projectagl/assets/168307999/91644d19-c2e6-4b84-b0b0-2d553c0ad78a)
![Capture d'écran 2024-04-29 192325](https://github.com/nouhabennasr/projectagl/assets/168307999/02ca6c4d-2e8d-433a-a376-a8df3f8abce2)
![image](https://github.com/nouhabennasr/projectagl/assets/168307999/b3a2702e-fd63-442a-a10f-3bac24c1b701)

Figure 1 : Diagramme de classe préliminaire de notre système domotique

1. Diagramme de séquence :

     A.  Ajouter un équipement électrique :

Quand un utilisateur veut commander son réseau domotique, il peut accéder à l’interface de la plateforme dans son téléphone portable ou son PC et il saisit son login et son mot de passe. 
Les entrées seront vérifiées dans l’application. 
Si tout est bien, l’interface de pilotage des équipements électriques sera affichée.

Acteur principal : Utilisateur
Scénario nominal :

L'utilisateur se connecte au système CasaControl.
L'interface de commande envoie les identifiants (login et mot de passe) au serveur pour vérification.
Le serveur valide les identifiants.
L'interface de commande affiche l'interface d’ajout des équipements électriques à l'utilisateur.
L'utilisateur accède à la section d’ajout des équipements électriques dans le système CasaControl.
Le système affiche un formulaire à remplir avec les informations nécessaires telles que le type, la marque, le modèle, etc.
L'utilisateur remplit le formulaire avec les détails de l'équipement à ajouter.
Après avoir saisi les informations requises, l'utilisateur confirme l'ajout de l'équipement.
Le système valide les informations et ajoute le nouvel équipement à la liste des équipements électriques.


Scénario alternatif 1:

L'utilisateur demande l'affichage de l'interface de l’ajout des équipements.
L'interface de commande envoie les identifiants (login et mot de passe) au serveur pour vérification.
Le serveur détecte que les identifiants sont invalides.
L'interface de commande affiche un message d'erreur à l'utilisateur.

Scénario alternatif 2:

L'utilisateur demande l'affichage de l'interface de l’ajout des équipements.
L'interface de commande affiche l'interface d’ajout des équipements électriques à l'utilisateur.
L'utilisateur accède à la section d’ajout des équipements électriques dans le système CasaControl.
Le système affiche un formulaire à remplir avec les informations nécessaires telles que le type, la marque, le modèle, etc.
L'utilisateur remplit le formulaire avec les détails de l'équipement à ajouter.
Après avoir saisi les informations requises, l'utilisateur confirme l'ajout de l'équipement.
Le système ne valide pas les informations et affiche un message pour dire que l’équipement existe déjà.
[Capture d'écran 2024-04-29 192658](https://github.com/nouhabennasr/projectagl/assets/168307999/8c489b7b-717a-4b2b-9f69-6fd2d107d4f1)
Figure 2 : Diagramme de séquence :
 « Ajouter un équipement électrique »:
![Capture d'écran 2024-04-29 192809](https://github.com/nouhabennasr/projectagl/assets/168307999/0458ba6a-40a4-4e65-8ef8-8c6dd2c7ea19)
![Capture d'écran 2024-04-29 194503](https://github.com/nouhabennasr/projectagl/assets/168307999/d95f93c0-6017-4a08-a199-2e2c0b916ab7)


 B. Activer un équipement électrique :

Pour activer un équipement électrique, l’utilisateur clique sur “ Activer un équipement “. 
On lui affiche la liste des équipements électriques et il choisit l’équipement qu’il veut activer. 
Après que les actions associées à cet équipement soient affichées, il clique sur le bouton d’activation « ON ».
Enfin, le message « équipement activé » sera affiché.

 Scénario nominal : 

L'utilisateur se connecte au système CasaControl.
L'interface de commande envoie les identifiants (login et mot de passe) au serveur pour vérification.
Le serveur valide les identifiants.
L'interface de commande affiche l'interface d’ajout des équipements électriques à l'utilisateur.
L'utilisateur accède à la section d’activer des équipements électriques dans le système CasaControl.
Une liste d'équipements s'affiche à l'écran.
L'utilisateur choisit l'équipement qu'il souhaite activer.
Les actions associées à cet équipement sont affichées à l'utilisateur.
L'utilisateur clique sur le bouton d'activation "ON".
Un message de confirmation "Équipement activé" est affiché à l'utilisateur.



Scénario alternatif :

L'interface de commande affiche l'interface d’ajout des équipements électriques à l'utilisateur.
L'utilisateur souhaite activer un équipement électrique.
Il clique sur “ Activer un équipement “
Une liste d'équipements s'affiche à l'écran.
L'utilisateur choisit l'équipement qu'il souhaite activer.
Les actions associées à cet équipement sont affichées à l'utilisateur.
Cependant, le bouton d'activation "ON" est grisé ou indisponible.
Un message d'erreur s'affiche, indiquant que l'équipement ne peut pas être activé pour une raison quelconque (peut-être un dysfonctionnement, une maintenance en cours, etc.).
L'utilisateur est invité à contacter le service technique pour obtenir de l'aide ou des informations supplémentaires.
![Capture d'écran 2024-04-29 194655](https://github.com/nouhabennasr/projectagl/assets/168307999/9f16a601-8a91-4056-9a9b-bfb21a82ca17)
![Capture d'écran 2024-04-29 202152](https://github.com/nouhabennasr/projectagl/assets/168307999/02d79bda-b611-46a4-bc2c-426e450cf731)
![Capture d'écran 2024-04-29 202235](https://github.com/nouhabennasr/projectagl/assets/168307999/c8c12178-1c5a-47c0-9ba8-fe8baed2c900)
C.Affichage de la liste des équipements électriques  : 

L’utilisateur peut connaître la liste des équipements électriques sur le réseau domotique. 
Tout d’abord, il clique sur “ Consulter la liste des équipements électriques “. 


Scénario nominal :

L'utilisateur souhaite connaître la liste des équipements disponibles sur le réseau domotique.
Il clique  sur “ Consulter la liste des équipements “.
La liste des équipements est affichée


Scénario alternatif :

L'utilisateur souhaite connaître la liste des équipements disponibles sur le réseau domotique.
Il clique  sur “ Consulter la liste des équipements “.
La liste des équipements est affichée
Cependant, le système rencontre une erreur lors de la récupération des détails de l'équipement.
Le système affiche un message d'erreur indiquant qu'il n'est pas possible de récupérer tous les détails de l'équipement pour le moment.
L'utilisateur est invité à réessayer ultérieurement ou à contacter le support technique pour obtenir de l'aide.
![Capture d'écran 2024-04-29 202347](https://github.com/nouhabennasr/projectagl/assets/168307999/34427540-5570-4195-8e58-21d1fce3dc3c)
![Capture d'écran 2024-04-29 202523](https://github.com/nouhabennasr/projectagl/assets/168307999/b1a42892-a156-4ba3-bc03-52e4da585fb1)




La conception détaillée est un document essentiel qui, s’il est bien étayé, nous permettra de restituer une réalisation de qualité.
L’objectif de ce document est de fournir la feuille de route exhaustive et détaillée nécessaire à la réalisation technique de votre projet.
![Capture d'écran 2024-04-29 202721](https://github.com/nouhabennasr/projectagl/assets/168307999/615f6879-1884-4df8-a456-730cad97dda8)
1-Raffinement du diagramme de classe préliminaire : 

Identifier les classes et les relations : Vérifier et valider les classes déjà identifiées dans le diagramme de classe initial. Identifier de nouvelles classes si nécessaire en fonction des détails émergents.
Spécifier les attributs et les méthodes : Examiner les attributs et les méthodes de chaque classe pour vous assurer qu'ils sont complets et précis. Ajouter des détails supplémentaires si nécessaire.
Préciser les relations entre les classes : Affiner les relations entre les classes en définissant plus précisément le type de relation (agrégation, composition, association) et en spécifiant les cardinalités si elles ne sont pas claires.
Gérer l'héritage : Si des hiérarchies de classes sont présentes, il faut clarifier les rôles et les responsabilités de chaque classe héritée. Il faut assurer que l'héritage est justifié et que les relations de sous-classe/super classe sont correctement définies.

Documenter les contraintes et les règles métier : Ajouter toute contrainte ou règle métier importante qui doit être respectée dans le diagramme de classe.
Vérifier la cohérence et la complétude : Assurer que le diagramme de classe est cohérent avec les autres documents de conception et qu'il est complet, couvrant tous les aspects importants du système.
Finaliser la documentation : Une fois que le diagramme de classe a été raffiné et validé, assurer de documenter toutes les décisions prises et les détails ajoutés pour référence future.
![Capture d'écran 2024-04-29 202825](https://github.com/nouhabennasr/projectagl/assets/168307999/94f162e9-cbbd-481c-aa4b-ccc41403be81)
![Capture d'écran 2024-04-29 202904](https://github.com/nouhabennasr/projectagl/assets/168307999/261a178d-115c-4cf8-acd7-ce59585982c6)
![image](https://github.com/nouhabennasr/projectagl/assets/168307999/256215ec-a126-4f69-b8cc-8baee6297312)
![Capture d'écran 2024-04-29 203402](https://github.com/nouhabennasr/projectagl/assets/168307999/085cd18a-b0f4-4085-93d7-5387ed7edd31)


L'encapsulation consiste à regrouper les données et les méthodes qui les manipulent au sein d'une même entité, souvent appelée classe. 


Les attributs d'une classe sont généralement déclarés comme privés pour limiter leur accès direct depuis l'extérieur de la classe. Pour permettre l'accès à ces attributs, des méthodes publiques, appelées getters et setters, sont utilisées. 


Les getters permettent d'obtenir la valeur d'un attribut, tandis que les setters permettent de modifier sa valeur. Cette approche assure la sécurité et l'intégrité des données en contrôlant leur accès et leur modification. 


En résumé, l'encapsulation garantit une meilleure modularité, une gestion efficace des données et une sécurité accrue du code en regroupant les données et en contrôlant leur accès via des méthodes publiques.
![DiagrammeDeClasse1](https://github.com/nouhabennasr/projectagl/assets/168307999/3f1fce58-0562-4f8c-a71c-e3e1ab88f7f8)


2. Le diagramme de machines à état :
Ce diagramme d'état de transition représente le cycle de vie d'un système domotique, en montrant les différents états dans lesquels le système peut se trouver et les transitions entre ces états. Voici une explication détaillée du diagramme :
États :
Éteint (Rose) : C'est l'état initial du système, où le système est éteint et inactif.

Démarrage (Bleu Ciel) : Dans cet état, le système est en cours de démarrage, généralement initié par l'utilisateur ou un processus automatique extérieur.

En Marche (Bleu Ciel) : C'est l'état dans lequel le système est pleinement opérationnel et exécute ses fonctions.

Fin (Rose) : C'est l'état final du système, où le processus d'exécution est terminé.

Transitions :
De l'état initial éteint, le système peut passer à l'état Démarrage lorsqu'un utilisateur ou un processus démarre le système en appuyant sur le bouton Démarrer ou à travers une condition extérieure.
Depuis l'état Démarrage, le système peut revenir à l'état Éteint si le processus de démarrage est annulé, généralement en appuyant sur le bouton "Annuler" ou un problème technique de démarrage.
De l'état Démarrage, le système peut passer à l'état En Marche une fois que l'actionneur électrique est programmé pour démarrer le système.
Depuis l'état En Marche, le système peut passer à l'état Fin une fois que la mise à jour de l'état est effectuée, indiquant que le processus d'exécution est terminé.
De l'état Fin, le système revient à l'état initial éteint, prêt pour un nouveau cycle d'exécution.
—> Ce diagramme illustre le flux de contrôle dans le système domotique, montrant comment le système évolue d'un état à un autre en réponse aux actions de l'utilisateur ou aux événements internes.
—> Il fournit une vue globale du fonctionnement du système, mettant en évidence les différents scénarios possibles et les transitions entre les États.

![Capture d'écran 2024-04-29 203802](https://github.com/nouhabennasr/projectagl/assets/168307999/c7714b67-ad0d-4e17-9042-be9f18df6b52)
![Capture d'écran 2024-04-29 203843](https://github.com/nouhabennasr/projectagl/assets/168307999/d16a1c54-7850-4114-89a0-c3237d6793c2)

1. 2ème raffinement du 2ème diagramme de classe : 


A)Navigabilite
On a ajouté des flèches de navigabilité entre les classes pour représenter les relations entre elles. 
Par exemple, on a relié la classe Utilisateur à la classe SMART_HOME avec une multiplicité de 1 à plusieurs (1..*), ce qui signifie qu'un utilisateur peut posséder plusieurs maisons intelligentes : relation unidirectionnelle puisque de base toutes les bases sont bidirectionnelles.


A)Traduction des attributs dérivés:
On a également introduit des attributs dérivés pour les classes Lampe et Climatisation, ce qui permet de calculer certains attributs en fonction d'autres attributs de la classe. 


Par exemple, on a ajouté l'attribut consommationElectrique pour la classe Lampe, calculé en fonction de la puissance et de la luminosité de la lampe.

![diag rendu4](https://github.com/nouhabennasr/projectagl/assets/168307999/fe806144-6da3-459d-9456-85b8c1fa905d)

![Capture d'écran 2024-04-29 205057](https://github.com/nouhabennasr/projectagl/assets/168307999/e27776b2-a00a-4974-a732-84fa011ac86c)
![Capture d'écran 2024-04-29 205129](https://github.com/nouhabennasr/projectagl/assets/168307999/d80a6a66-2ef1-48c0-87c1-f49105217b1b)
![Capture d'écran 2024-04-29 205205](https://github.com/nouhabennasr/projectagl/assets/168307999/27e1fff6-5369-4efb-9db8-187288946b30)
![Capture d'écran 2024-04-29 205241](https://github.com/nouhabennasr/projectagl/assets/168307999/05d80e3e-0af9-4a2c-ab55-1091bc6c7cbe)

2. Invariants :


A‐ Invariants :


Construction de l'invariant d'au moins une classe importante :


Un invariant est une condition qui doit toujours être vraie pour une instance de classe donnée à tout moment de son cycle de vie. C'est une sorte de règle ou de contrainte que chaque instance d'une classe doit respecter pour garantir un comportement cohérent du système.


Pour illustrer la construction de l'invariant d'une classe importante, prenons l'exemple de la classe Capteur dans notre système domotique.
Voici un exemple d'invariant :


Invariant de la classe Capteur :


Chaque capteur doit avoir un identifiant unique.


Un capteur doit être associé à une pièce de la maison.


Un capteur doit être actif ou inactif. 


Il ne peut pas être dans un état indéterminé.


Les données collectées par un capteur doivent être valides et cohérentes par rapport à son type (par exemple, un capteur de température ne doit pas rapporter des données de luminosité).


Un capteur ne peut pas être associé à plusieurs équipements en même temps.
.


La position du capteur ne doit pas être nulle.


—> Ces invariants garantissent que les instances de la classe Capteur fonctionnent de manière fiable et cohérente dans le système domotique, ce qui contribue à la stabilité et à la sécurité globales du système. 






La formule en logique propositionnelle de l'invariant de la classe capteur :


Soient les propositions symboliques :


Ui : L'identifiant unique du capteur 
Pi : La pièce de la maison associée au capteur 
Ai : L'état d'activation du capteur  (actif ou inactif).
Di  : Les données collectées par le capteur 
POi  : La position du capteur




L'invariant peut être exprimé comme suit en logique propositionnelle :


∀Capteur,


(𝑈𝑖≠null)∧(𝑃𝑖≠null)∧(𝐴𝑖∈{actif,inactif})∧(𝐷𝑖≠null)∧(𝑇𝑖≠null)∧(𝑆𝑖≠null)∧(𝐹𝑖>0)∧(𝑅𝑖≠null)(Ui=null)∧(Pi=null)∧(Ai∈{actif,inactif})∧(Di=null)∧(POi≠nul)


B‐ Tables de décisions des tests unitaires :


Opération 1 : s’authentifier : la table de décision des tests unitaires.
| Cas de test | Conditions                            | Résultat attendu |
|-------------|--------------------------------------|------------------|
| Test 1      | Utilisateur existe                   | T                |
| Test 2      | Utilisateur inexistant               | F                |
| Test 3      | Utilisateur avec mauvais mot de passe| F                |
| Test 4      | Utilisateur avec login incorrect     | F                |

Figure 2 : table de décision des tests unitaires pour l'opération s’authentifier



Cette table de décision contient les différents cas de test pour l'opération s'authentifier() de la classe Utilisateur. 


Chaque cas de test est décrit avec les conditions qui doivent être remplies et le résultat attendu de l'opération.


Test 1: Vérifie si un utilisateur existe dans le système.


Test 2: Vérifie le comportement lorsque l'utilisateur n'existe pas dans le système.


Test 3: Vérifie le comportement lorsque l'utilisateur existe mais fournit un mot de passe incorrect.


Test 4: Vérifie le comportement lorsque le login associé à son compte est invalide.


Opération 2 : ajouter un équipement :  la table de décision des tests unitaires.

| Cas de test | Conditions                                                | Résultat attendu |
|-------------|----------------------------------------------------------|------------------|
| Test 1      | Équipement existant                                      | T                |
| Test 2      | Équipement inexistant                                    | F                |
| Test 3      | Champs du formulaire d’ajout non nuls et non vides      | F                |

Figure 3 : table de décision des tests unitaires pour l'opération ajouter un équipement


Cette table de décision contient les différents cas de test pour l'opération ajouter_équipement () de la classe équipement. Chaque cas de test est décrit avec les conditions qui doivent être remplies et le résultat attendu de l'opération

Test 1: Vérifie si un équipement existe.

Test 2: Vérifie si un équipement est inexistant.

Test 3: Vérifie le comportement concernant le formulaire d’ajout d’un équipement (champs non vides et non nuls).
 



































