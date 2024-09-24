<div style="text-align: center;">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRDRZIZCeWekkLEQ0GzKtXMoNZs0MY_d4QqcQ&s" alt="Logo CKAN" title="Logo CKAN">
</div>

# Étude de solution de catalogage : CKAN

Création d'un projet Github par groupe de travail (**CKAN** ~et~ ~uData~) pour diffuser le contenu de la recherche.

[`Github : https://github.com/az-si/CKAN_IDGEO`](https://github.com/az-si/CKAN_IDGEO)

<u>Projet composé de</u> : [Maureen](https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSe7sOOlS0_9h6qkNnryU_hBRZozsBajLLP1z-kjZDDzC7CSBaB), [Antonin](https://www.linkedin.com/in/antonin-brun-52a4bb203/), [Matéo](https://fr.linkedin.com/in/mat%C3%A9o-tartas-12bab2252?original_referer=https%3A%2F%2Fwww.google.com%2F), [Adama](https://www.linkedin.com/in/adama-w-486829211/), [La zizanie](https://www.linkedin.com/in/abdelaziz-souissi/), [Elia](https://www.linkedin.com/in/elia-marie-350em/) et [Théodose](https://www.linkedin.com/in/th%C3%A9odose-tchedji-39a04521a/)


## Description de la solution

D'après leur GitHub, CKAN est le leader mondial de platforme de portail open data.

Logiciel Libre (open source data management system).
La fonctionnalité de moissonage utilise l’API de CKAN pour récupérer les métadonnées.
Ce moissonneur attend l’URL racine de l’instance CKAN et non du portail (dans le cas où CKAN est couplé à Drupal par exemple).

CKAN possède une extention de base de données. C'est une solution "à la carte" grace à l'ajout ou au retrait d'extentions.
Il gère les données géospatiales, les métadonnées, la gestion de données, la recherche par mots clés, la visualisation de données, la sécurité et on peut refaire la déco pour que ça corresponde à notre chartre graphique.

Possibilité de déployer un portail data ou de gérer et publier de la donnée en interne.

Utilisé par le gouvernement du Canada.
Met en place des Webinaires.


## Procédure d'installation

:::info
:information_source: Monsieur MICHEL, notre professeur bien-aimé, nous a proposé des critères de recherche rigoureux qui reflètent sa quête constante d'excellence et de précision. Il nous encourage à approfondir : Documentation + privilégier docker
:::

[`Image docker : 
https://hub.docker.com/r/ckan/ckan`](https://hub.docker.com/r/ckan/ckan)

[`Instructions pour installer ckan via docker :
https://github.com/ckan/ckan-docker`](https://github.com/ckan/ckan-docker)

[`Guy theub :
https://github.com/ckan/ckan`](https://github.com/ckan/ckan)

[`Documentation :
https://docs.ckan.org/en/2.9/maintaining/installing/install-from-docker-compose.html`](https://docs.ckan.org/en/2.9/maintaining/installing/install-from-docker-compose.html)

Cette partie a pour but de proposer un déploiement à la fois simple et entièrement modulable, plus facile à mettre en place qu'une installation depuis les sources, tout en offrant plus de personnalisation qu'une installation via un package.

### Quelques prérequis

- **Docker**:Une plateforme permettant de lancer certaines applications dans des conteneurs

- **Python**
Si vous utilisez un système d'exploitation basé sur Debian, il faut commencer par installer les packages requi avec cette commande : 
sudo apt-get install python3-dev libpq-dev python3-pip python3-venv git-core redis-server libmagic1

- **PostgreSQL** : Le système de base de données PostgreSQL, v12 ou plus récent.

- **Java** Development Kit (JDK) et OpenJDK
- **Redis** : Un magasin de structures de données en mémoire

## Présentation des interfaces
:::info
:information_source: Monsieur Michel, notre enseignant tant apprécié, nous a présenté des critères de recherche exigeants qui témoignent de son engagement permanent pour l’excellence et la rigueur. Il nous incite à approfondir : back et frontend
:::
#### Visualisation de l'interface utilisateur

L'utilisateur peut visualiser la donnée de différentes manières : c b onsultation de l'information sous forme de statistiques, de cartes, d'images, de tableurs, ...

<img style="display:block;border:1px #eee;width:100%;" src="https://docs.ckan.org/en/2.9/_images/manage_views.png" />

#### Visualisation de l'interface administrateur

Voici l'interface administrateur dans laquelle vous trouverez le nom de notre groupe **<span style="color:green">EMMAAA</span>**.
![image](https://hackmd.io/_uploads/r1zqTWl00.png)

L'administrateur a la possibilité de créer des comptes collaborateurs grâce au formulaire d'enregistrement de compte.
![image](https://hackmd.io/_uploads/Sk8ob4eAR.png)

Ensuite, chaque membre de l'équipe se connecte et accède au compte de l'organisation **<span style="color:green">EMMAAA</span>**.
Pour ce faire, nous utilisons le lien suivant : https://192.168.40.12:8443/user et ouvrons l'onglet **Log in**.

#### Ajout de dataset

Pour implémenter le catalogue, il suffit de remplir le formulaire suivant : 
![image](https://hackmd.io/_uploads/S1h9oQxRC.png)

#### Visualisation de la donnée

Pour visualiser la donnée, il faut consulter l'onglet **Dataset** de l'organisation.
![image](https://hackmd.io/_uploads/ryLUhQx0R.png)


:::success


:lock: **Accès aux comptes**

Identifiants et mots de passe créés par l'administrateur La zizanie


|User|Mot de passe|
|:---------:|:-------------:|
|   maureen    |maureen1234 |
|    antona  |   antona1234   | 
| mateo  |    mateo1234    |
| elia  |    elia1234    |
| adama |     adama1234     |
:::

## Avantages et inconvénients


|<span style="color: #26B260">Avantages</span>|<span style="color: #e10c0c">Inconvénients</span>|
|:---------:|:-------------:|
|    Facile de publier    |      Configuration complexe      |
|    Facile à partager    |   Connexion et collaboration   | 
| Présence d'une API  |        |
| Système de managment de la data  |        |
| Personnalisation de l'interface|          |





⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⣠⣤⣶⣶⣦⣄⡀  ⠀⢀⣤⣴⣶⣶⣤
⣼⣿⣿⣿⣿⣿⣿⣷⣤⣾⣿⣿⣿⣿⣿⣿⣧
⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿
⠹⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠏
⠀⠙⢿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠋⠀
⠀⠀⠀⠙⢿⣿⣿⣿⣿⣿⣿⣿⡿⠛⠁⠀⠀
⠀⠀⠀⠀⠀⠉⢿⣿⣿⣿⠟⠋⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠙⠻⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
    
    
   ## About
```
https://hackmd.io/@EzhzaLoNTpuc8eGVX0TZtA/SkJsmzgAC
```


## Users 
![image](https://hackmd.io/_uploads/HyrpxVxAC.png)


# Présentation

Nous sommes **une équipe de géomaticiens expérimentés**, spécialisés dans la gestion de projets complexes et innovants. Avec une passion pour la précision et l’efficacité, nous utilisons notre expertise en systèmes d’information géographique (SIG) pour transformer les données géospatiales en solutions concrètes. Notre approche est résolument tournée vers l'action, guidée par la rigueur scientifique et une compréhension approfondie des enjeux technologiques.

 # Nos Atouts

- **Engagement total** : Chaque membre de notre équipe est profondément investi dans chaque projet. Nous faisons preuve de dévouement et d'une éthique de travail sans faille, assurant la réussite à chaque étape du processus.
  
- **Résolution de problèmes complexes** : Nous ne reculons devant aucun défi. Qu'il s'agisse de concevoir des infrastructures de données géospatiales ou de répondre aux exigences spécifiques des projets, nous avons les compétences techniques et managériales pour délivrer des résultats d'exception.

- **Innovation continue** : En combinant nos connaissances en géomatique avec les dernières avancées technologiques, nous apportons des solutions créatives et personnalisées, adaptées à l'évolution des besoins de nos clients.

 # Notre Mission

Nous sommes plus qu'un simple groupe de **géomaticiens**. Nous sommes des leaders de projets, prêts à relever les défis du terrain avec une approche proactive et une vision stratégique. Toujours en quête d’excellence, nous plaçons la réussite de vos projets au cœur de notre mission.

# Notre équipe
<div style="text-align: center;">

![Capture](https://hackmd.io/_uploads/H1N2QfgCC.jpg)![maur](https://hackmd.io/_uploads/S1tP4fgA0.jpg)![ent](https://hackmd.io/_uploads/rJSc4fgR0.jpg)![ab](https://hackmd.io/_uploads/Skw6EzgRR.jpg)![ma](https://hackmd.io/_uploads/HyReBMeA0.jpg)![ad](https://hackmd.io/_uploads/rylmSzgCC.jpg)
![doseddd](https://hackmd.io/_uploads/HJPmUMgRR.jpg)
##### [`IdGeo : site web`](https://idgeo.fr/)
