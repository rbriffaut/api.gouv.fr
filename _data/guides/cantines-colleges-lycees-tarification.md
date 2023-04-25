---
title: Tarification cantine des collèges et lycées
tagline: Départements et régions, simplifiez les démarches des familles en calculant automatiquement le tarif de restauration scolaire des collégiens et lycéens.
tags: cas usage, api particulier, quotient familial dématérialisé, tarification restauration scolaire, cantine collège, cantine lycée
image: cantines_colleges_lycees_tarification.jpg
noindex: false # this page will appear on Google
publish: true # this page will appear on /guides page
api:
  - API Particulier
---

<details>
   <summary>Comment fonctionne la tarification des cantines dans les collèges et lycées ?</summary>

Les départements sont en charge des cantines des collèges, et les régions, des cantines des lycées. Dans ce cadre, ce sont ces collectivités qui fixent les tarifs de la restauration scolaire et qui peuvent décider d'appliquer une tarification sociale sur la base des revenus de la famille.

Pour en savoir plus, consulter cette page de [Service-Public.fr](https://www.service-public.fr/particuliers/vosdroits/F24569)

</details>


## Table des matières

- [Simplifier la tarification des cantines au collège et lycée grâce aux API](#simplifier-la-tarification-des-cantines-au-collège-et-lycée-grâce-aux-api)
- [Les API et données utiles](#les-api-et-données-utiles)
- [Améliorer votre tarification cantine avec l'API Particulier](#améliorer-votre-tarification-cantine-avec-lapi-particulier)
  - [Exemple d'utilisation](#exemple-dutilisation)
- [Demander un accès aux API](#demander-un-accès-aux-api)


## Simplifier la tarification des cantines au collège et lycée grâce aux API

Départements et régions, en intégrant l'API Particulier dans votre système d'information :
- 😃 Pour instruire les dossiers, **il n'est plus nécessaire de demander aux familles de renseigner** : 
   - leur quotient familial CAF ;
   - leur revenu fiscal de référence ;
- ⏰ Vous accélérez le traitement des dossiers car vos agents n’ont **pas à vérifier les données saisies et les pièces justificatives fournies**, les informations obtenues par l'API sont certifiées 🔎 ;
- 🎯 Enfin, vous **participez à la simplification des démarches pour les citoyens** en mettant en oeuvre le [« Dites-le-nous une fois »](https://www.numerique.gouv.fr/services/guichet-dites-le-nous-une-fois/), en application de l’[article L113-12 du Code des relations entre le public et l’administration](https://www.legifrance.gouv.fr/codes/article_lc/LEGIARTI000037313155).

## Les API et données utiles

| API utiles | Données disponibles |  Peut s'utiliser avec FranceConnect |
| --- | --- | --- |
| Bouquet [API Particulier](https://particulier.api.gouv.fr/catalogue) - opéré par la DINUM | Quotient familial CAF, composition familiale| ⚙️ Certaines API sont disponibles avec FranceConnect |
| [API Impôt particulier](/les-api/impot-particulier) - DGFIP | Revenu fiscal de référence, nombre de parts fiscales | ✅ |


## Améliorer votre tarification cantine avec l'API Particulier

L'API Particulier est un bouquet d'API délivrant des informations administratives des particuliers issues de différents fournisseurs de données.

Avec l'API Particulier, vous avez notamment accès au quotient familial CAF, au statut élève scolarisé et boursier, au statut étudiant et étudiant boursier, au statut demandeur d'emploi...

<Button href="https://particulier.api.gouv.fr/catalogue">Découvrir l'API Particulier</Button>

### Exemple d'utilisation

**Un parent souhaite inscrire son enfant à la cantine du lycée depuis le site de sa région connecté à l'API Particulier** :

**Étape 1 :** Le parent se connecte à son espace personnel sur le site de la région, il clique sur la démarche dédiée à l'inscription cantine scolaire et **renseigne son numéro d'allocataire et son code postal**.

> ⚙️ **En arrière plan** : Un appel à l'API quotient familial CAF du bouquet API Particulier est effectué et permet de récupérer le quotient familial du mois en cours.

**Étape 2 :** La tarification de la cantine scolaire est automatiquement calculée en fonction du quotient familial. Le parent n'a plus qu'à terminer l'inscription.


## Demander un accès aux API

### Justifier votre cadre juridique

L'utilisation des données est encadrée légalement. Vous devez formuler une demande auprès de l'API Particulier en justifiant du cadre légal de l'utilisation des données :
- Cadre légal général : l'[Article L114-8 du Code des relations entre le public et l'administration](https://www.legifrance.gouv.fr/codes/article_lc/LEGIARTI000045213315) fixe le cadre général qui oblige l’administration à échanger des données lors d’une démarche d’un usager ;
- Cadre légal spécifique aux téléservices : En tant que collectivités territoriales vous avez donc un droit d'accès à certaines données dans le cadre de demandes, services pro-actifs et déclarations usagers. 
L'[Arrêté du 04/07/13 sur les téléservices](https://www.legifrance.gouv.fr/loda/id/JORFTEXT000027697207/#:~:text=Dans%20les%20r%C3%A9sum%C3%A9s-,Arr%C3%AAt%C3%A9%20du%204%20juillet%202013%20autorisant%20la%20mise%20en%20%C5%93uvre,publiques%20locales%20dont%20ils%20sont) détaille à l'article 1 la liste des démarches par secteur. Aidez-vous de cet arrêté pour justifier de votre cadre légal.
- Fournir **l'acte/la délibération** qui fixe les critères de la tarification.

### Formulaires de demande d'accès

Vous souhaitez demander un accès à l'[API Particulier](https://particulier.api.gouv.fr/catalogue) ? Déposez votre demande d'habilitation :

<Button href="https://datapass.api.gouv.fr/api-particulier?demarche=ccas">Remplir une demande API Particulier</Button>

Vous avez besoin des données fiscales ? Il vous faudra faire une [demande d'habilitation dédiée auprès de la DGFIP](/les-api/impot-particulier).

⚠️ Lors de votre demande d’habilitation, vous vous engagez à ne demander que les données strictement nécessaires à la réalisation de la démarche administrative.

🛠 🧰 Avant de faire votre demande d'habilitation, **assurez-vous que votre service informatique ou votre éditeur de logiciel est en mesure d'intégrer des API**. L'API Particulier détaille [ici une liste de prérequis techniques](https://particulier.api.gouv.fr/developpeurs#prerequis-techniques). 