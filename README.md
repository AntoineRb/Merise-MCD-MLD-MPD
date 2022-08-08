# Merise-MCD-MLD-MPD

---

##### Contexte du projet

Les formations sont organisés en modules.

Chaque module est caractérisé par un numéro de module sous forme de Semantic Versionning, un intitulé, un objectif pédagogique, un contenu (textes, images et vidéos), une durée en heures, un ou plusieurs tags et un auteur.

Un module peut faire partie d'une ou plusieurs formations, comme par exemple un pire module "Commandes de base Git" pourrait faire partie d'une pire formation "Frontend Javascript" et "DevOps", voir  plus.

Un module peut contenir un texte et/ou une image et/ou une vidéo.

Les apprenants peuvent s'inscrire à une ou plusieurs formations, ils peuvent choisir de ne pas suivre certains des modules s'ils possèdent déjà, par exemple, les compétences. Autrement dit, ils peuvent arbitrairement valider les modules de leur choix en un clic.

Chaque apprenant est évalué pour chaque module et possède un état de fin de module (OK / KO).

Une formation est considérée comme terminée lorsque tous les modules ont été validés.

Chaque apprenant est caractérisé par un numéro d’inscription unique, un nom, un prénom, une adresse et une date de naissance.

Un formateurs est auteur d'un module pour une formation donnée, chaque formateur est caractérisé par un code, un nom, un prénom.

#### Modalités pédagogiques
* Travail en groupe
* Rendu individuel
* Livraison Mardi 09 Août 2022 17h

#### Critères de performance
* La nomenclature MERISE est respectée
* Le méthode MERISE est respectée dans sa structure en découpant la conception de cette base de données en 3 niveaux : le niveau conceptuel, le niveau logique ou organisationnel, le niveau physique

#### Modalités d'évaluation
Revue des diagrammes sur le dépôt Git.

#### Livrables
- Un dépôt Github recensant : 
    - Un README explicite et soigné
    - Une définition de l'acronyme MERISE dans le README.md
    - Un dictionnaire de données
    - Des règles de gestion
    - Un MCD
    - Un MLD
    - Un MPD
    - Un script SQL de la base de données
--- 
# Brief

## Règles de gestion

### Utilisateurs

- Un utilisateur doit renseigner un **prénom**, un **nom**, une **adresse** et **date de naissance**;

- Les utilisateurs ont soit un **rôle** d'enseignant ( **teacher** ) ou un rôle d'apprenant ( **student** );

- Les utilisateurs ont un ***rôle "user" par défaut*** tant qu'ils n'ont pas renseigner un rôle;

### Professeurs

- Chaque professeur à un **code d'enseignant** unique;

- Un professeur peut créer une nouvelle formation:

- Un professeur peut ajouter des modules de formation existents à la sienne ou en créer de nouveaux;

- Un module de formation doit contenir obligatoirement un **text**, la **vidéo** et l'**image** sont optionnelles;

- Les modules sont reliés à leurs auteurs ( professeurs ). Une formation peut donc contenir des modules postés par plusieurs professeurs;


- Les modules sont liés à un ou plusieurs **tags**, ils ont pour but d'indiquer les notions enseignées dans un module;

- Les chapitres d'une formation sont donc divisés en modules, ils sont donc caractérisé par un marquage sémantique;

### Etudiants

- Un étudiant possède un **code d'étudiant unique**;

- Un étudiant peut suivre une à plusieurs formations;

- Un étudiant peut compléter les modules de ces formations suivies, il peut le faire de manière arbitraire si il a déjà acquis la compétence enseignée dans un module;
