---
title: API Scolarite de élève
tagline: Interrogez les statuts scolarité et boursier des élèves du primaire, collège et lycée
is_open: 1 # 1 means API is fully open
producer: MENJ
keywords:
  - élèves
  - scolarité
  - statut scolaire
  - bourse
  - établissement
themes:
  - Education
content_intro: |
  L' **API Scolarité élève** permet de vérifier si un élève est bien scolarisé dans un établissement donné, et s'il est boursier ou non.

  ### A quoi sert l'API Scolarité élève ?

  En intégrant l'API dans votre système d'information, vous pouvez notamment :

  - vérifier qu'un élève est bien scolarisé dans l'établissement où il prétend être
  - vérifier si un élève est boursier ou non
  - récupérer son échelon de bourse
contact_link: api-sco-eleve_contacts@education.gouv.fr
doc_tech_link: https://geo.api.gouv.fr/definition.yml
doc_tech_external: https://geo.api.gouv.fr/decoupage-administratif
last_update: 25/08/2023
---

### Périmètre
#### Particuliers concernés : 
Cette API concerne les élèves du primaire, du collège et du lycée.
Une large majorité d’établissements sont concernés :

    - établissements publics ;
    - établissements privés sous contrat ;
    - lycées militaires et lycées maritimes ;
    - une partie des formations à distance du CNED.

Concernant le statut boursier des élèves : seules les bourses sur critères sociaux à l’échelle nationale sont couvertes par l’API. Par ailleurs, les bourses ne concernent que les collégiens et lycéens.
Les établissements suivants ne sont pas couverts par l’API :

    - établissements privés hors contrat ;
    - lycées agricoles ;
    - instruction dans la famille.
    
#### Périmètre géographique : 
  - France métropolitaine
  - DROM-COM

#### Actualisation de la donnée : 

Cette API délivre les informations de l’année scolaire en cours et bientôt de l’année scolaire à venir (N+1).
Les données du premier degré (primaire) sont mises à jour en temps réel. Les données du second degré (collèges et lycées) sont mises à jour quotidiennement toutes les nuits.
Les informations, même si elles évoluent principalement lors de la rentrée scolaire en septembre, peuvent changer en cours d’année (déménagements, etc.).
Attention, si un élève est indiqué “non-boursier” avant mi-octobre, il ne faut pas prendre en compte cette information. Le statut non-boursier est véritablement fiable à partir de mi-octobre.

### Données disponibles

| Nom         | Description                                                                                                              |
| ----------- | ------------------------------------------------------------------------------------------------------------------------ |
| Commune     | Le nom, la population, le code INSEE, le code postal, la géolocalisation (latitude, longitude) et le contour (GeoJSON), localisation de la mairie |
| Département | Le nom, le code INSEE du département, et la région de rattachement                                                       |
| Région      | La liste des régions et leur code INSEE                                                                                  |
| EPCI        | Le nom, le département et la région de rattachement, le contour des Etablissements publics de coopération intercommunale |

### Couverture du territoire

France métropolitaine, [DROM](https://fr.wikipedia.org/wiki/D%C3%A9partement_et_r%C3%A9gion_d%27outre-mer) et [COM](https://fr.wikipedia.org/wiki/Collectivit%C3%A9_d%27outre-mer).

### Coordonnées géographiques

Cette API utilise exclusivement des coordonnées géographiques [WGS-84](https://fr.wikipedia.org/wiki/WGS_84).
Elle peut renvoyer des données au format JSON ou [GeoJSON](http://geojson.org).

### Données source

[Toutes les données utilisées](https://github.com/etalab/api-communes#données-sources) sont sous licences Open Data.
