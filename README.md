---
description: Réalisé par HOSTIN Christopher et MONDESIR Malik
---

# Alumnus LPRS

## Présentation du projet

L'objectif est de développer un site internet pour les anciens étudiants pour un établissement supérieur, Lycée et UFA Robert Schuman \(Dugny, 93\). Ce site doit respecter les standards sur le Web ainsi que le cahier des charges qui nous a été transmis.

### Cahier des charges

* Maquette : se trouve dans "alumnus/src/static"
* Page _Index_ de présentation
* Page _Connexion_ \(sécurisée et mot de passe encrypté\)
  * Réinitialisation de mot de passe par envoi de mail
* Page _Événements_
  * Admin : Ajout, modification et suppression d'événements
  * Tous :  Ajout, modification et suppression de posts
* Page _Gallerie_
  * Admin : Ajout, modification et suppression d'images
  * Membre : consultation simple
* Footer
  * Informations et liens vers le lycée Robert Schuman
  * Localisation du site : API OpenStreetMap
  * Souscription à la newsletter d'Alumnus LPRS \(mail à chaque nouvel événement et post\)
* Accessibilité
  * Portage du site afin de le rendre accessible par les appareils mobiles
* Page _Dashboard_ et Vue administrateur
  * Accès aux données des tables des bases de données

#### Additionnels 

* Header
  * Sélection de la langue entre le français et l'anglais \(entraînement avec le JSON\)
  * Sélection du thème entre "lumineux" et "sombre" \(le dernier donne un meilleur rendu visuel\)
* Page _Chat_
  * Tous : connexion au chat et discussion \(en local en raison de nos capacités\)

{% hint style="warning" %}
Notre site est accessible sur les appareils portables avec quelques fonctionnalités manquantes : la sélection de la langue \(Français par défaut\) et du thème \(Lumineux par défaut\).
{% endhint %}

## Ressources

Langages : HTML, CSS, JS, PHP, SQL

API : [OpenStreetMap](https://www.openstreetmap.org/)

Librairies : [Bootstrap](https://getbootstrap.com/), [SBAdmin](https://startbootstrap.com/templates/sb-admin/), [jQuery](https://jquery.com/), [FancyBox](https://fancyapps.com/fancybox/), BxSlider, CalendarJS

Serveur : dernière version de [WAMP](http://www.wampserver.com/)

Répertoire Github : ~~**coming soon**~~

#### Tables de la base de données _`alumnus`_

* _`events`_ : contient les événements apparaissant sur la page _Événements_
* _`gallery`_ : contient les images et vidéos apparaissant sur la page _Galerie_
* _`users`_  : contient les identifiants des utilisateurs du site Alumnus

#### Tables de la base de données _`chat`_

* _`events`_ : contient les événements apparaissant sur la page _Événements_
* _`gallery`_ : contient les images et vidéos apparaissant sur la page _Galerie_
* _`users`_  : contient les identifiants des utilisateurs du site Alumnus

## Page d'accueil

Les pages accessibles par les utilisateurs de tout niveau d'accès sont :

* **Chat** \(dirige vers la page de connexion\)
* **Événements**
* **La page d'accueil**
* **Galerie**

{% hint style="info" %}
Le carousel, créé avec BxSlider \(une dérivée et composante de FancyBox\), présente brièvement les locaux et l'établissement du Lycée et UFA Robert Schuman. Le changement d'images est automatisé et s'interromps uniquement si l'utilisateur le fait manuellement.
{% endhint %}

## Page de connexion

Maintenant, accédez à la page de connexion avec le bouton en haut à droite de la page d'accueil.

#### Utilisez une de ces paires d'identifiants afin de vous connectez \(pour le moment\) :

| Nom | Mot de passe | Rôle |
| :---: | :---: | :---: |
| admin | root | Administrateur |
| user | test | Utilisateur |

#### Identifiants du chat

| Nom | Mot de passe | Rôle |
| :---: | :---: | :---: |
| root | admin | Administrateur |
| sudo | guest | Utilisateur |

{% hint style="danger" %}
Veuillez les changer avant tout déploiement sur un serveur.
{% endhint %}

Voir plus sur la [documentation utilisateur en pièce jointe](https://drive.google.com/file/d/1xNt2Y-n-bcGkEsDAKVf4qh_BMUWtSP3A/view?usp=sharing).

