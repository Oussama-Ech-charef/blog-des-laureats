# Définir la vision produit et exprimer les besoins en User Stories

## 1. Les notions fondamentales

### 1.1. Vision Produit

#### Définition

La Vision Produit décrit l'objectif principal d'une application. Elle présente le problème à résoudre, les utilisateurs ciblés et la valeur apportée par le produit.

Elle permet à toute l'équipe de partager le même objectif et de guider les décisions du projet.

#### Exemple – Billetterie d'événements

Notre vision est de créer une plateforme web qui permet aux organisateurs de publier et gérer leurs événements, et aux visiteurs de découvrir facilement les événements disponibles.

### 1.2. Personas

#### Définition

Un Persona est un profil fictif qui représente un type d'utilisateur de l'application.

Il décrit ses objectifs, ses besoins, ses motivations et ses contraintes.

Les Personas permettent de mieux comprendre les utilisateurs et de créer une application adaptée à leurs attentes.

#### Exemple – Billetterie d'événements

- **Organisateur :** une personne qui souhaite publier et gérer ses événements.
- **Visiteur :** une personne qui souhaite découvrir les événements et consulter leurs informations.

### 1.3. User Stories

#### Définition

Une User Story est une description simple d'une fonctionnalité du point de vue de l'utilisateur.

Elle explique ce que l'utilisateur veut faire et pourquoi il a besoin de cette fonctionnalité.

#### Structure standard

Une User Story respecte le modèle suivant :

> En tant que [Utilisateur],  
> Je veux [Fonctionnalité],  
> Afin de [Objectif].

#### Exemple – Billetterie d'événements

En tant qu'organisateur, je veux ajouter un événement afin de le présenter aux visiteurs.

### 1.4. Critères d'acceptation

#### Définition

Les critères d'acceptation sont des conditions qui permettent de vérifier si une User Story fonctionne correctement.

Ils doivent être clairs, précis, mesurables et testables.

#### Exemple – Ajouter un événement

- Le formulaire contient un titre, une description, une date, une heure, un lieu, un prix, un nombre de places et une catégorie.
- Les champs obligatoires doivent être remplis.
- L'événement est enregistré dans la base de données si les informations sont valides.

### 1.5. MVP – Minimum Viable Product

#### Définition

Le MVP est la première version simple d'un produit. Il contient uniquement les fonctionnalités essentielles pour apporter une première valeur aux utilisateurs.

Il permet de tester le produit avec les utilisateurs avant d'ajouter des fonctionnalités plus avancées.

#### Exemple – Billetterie d'événements

**Fonctionnalités essentielles du MVP :**

- Ajouter un événement.
- Consulter ses événements.
- Modifier un événement.
- Supprimer un événement.
- Afficher la liste des événements publiés.
- Consulter les détails d'un événement.

**Fonctionnalités futures :**

- Inscription et connexion.
- Réserver des billets.
- Effectuer un paiement en ligne.
- Générer des QR Codes.
- Envoyer des notifications.

---

## 2. Application pratique au Projet Technique

### 2.1. Présentation du projet

Le projet Billetterie d'événements est une plateforme web qui permet aux organisateurs de publier et gérer leurs événements.

Les visiteurs peuvent consulter les événements disponibles et découvrir leurs informations comme le titre, la description, la date, le lieu et le prix.

L'objectif est de faciliter la gestion et la découverte des événements depuis une seule plateforme.

### 2.2. Vision Produit

Créer une plateforme web simple et accessible qui permet aux organisateurs de publier et gérer leurs événements, et aux visiteurs de découvrir facilement les événements disponibles et leurs informations.

**Valeur apportée :**

- Pour les organisateurs : faciliter la publication et la gestion des événements.
- Pour les visiteurs : faciliter la découverte et la consultation des événements.

### 2.3. Personas cibles

Les deux Personas suivants représentent les principaux utilisateurs de notre plateforme.

#### Persona 1 – Yassine, Organisateur

| Élément | Description |
|---|---|
| Nom | Yassine |
| Âge | 29 ans |
| Profil | Organisateur d'événements |
| Objectif | Publier et gérer ses événements. |
| Besoins | Ajouter, modifier et supprimer des événements. |
| Motivations | Présenter ses événements à un grand nombre de visiteurs. |
| Contraintes | Il souhaite utiliser une plateforme simple et rapide. |

**Scénario d'utilisation :**

Yassine organise des événements et souhaite utiliser la plateforme pour publier les informations de ses événements et les gérer facilement.

#### Persona 2 – Salma, Visiteur

| Élément | Description |
|---|---|
| Nom | Salma |
| Âge | 22 ans |
| Profil | Étudiante et visiteuse |
| Objectif | Découvrir les événements disponibles. |
| Besoins | Consulter les événements et leurs détails. |
| Motivations | Trouver des événements intéressants. |
| Contraintes | Elle souhaite accéder rapidement aux informations depuis son téléphone. |

**Scénario d'utilisation :**

Salma souhaite découvrir les événements disponibles. Elle utilise la plateforme pour consulter les dates, les lieux et les prix avant de choisir un événement.

### 2.4. User Stories et critères d'acceptation

Les User Stories décrivent les principales fonctionnalités attendues par les utilisateurs.

#### US-01 : Ajouter un événement

**User Story :**

En tant qu'organisateur, je veux ajouter un événement afin de le présenter aux visiteurs.

**Critères d'acceptation :**

- Le formulaire contient les informations nécessaires : titre, description, date, heure, lieu, prix, nombre de places et catégorie.
- Les champs obligatoires doivent être remplis.
- Le prix doit être positif ou égal à zéro et le nombre de places doit être supérieur à zéro.
- L'événement est enregistré dans la base de données avec les informations de son organisateur.

#### US-02 : Gérer ses événements

**User Story :**

En tant qu'organisateur, je veux consulter, modifier et supprimer mes événements afin de garder mes informations à jour.

**Critères d'acceptation :**

- L'organisateur peut consulter la liste de ses événements dans son espace de gestion.
- Il peut modifier les informations d'un événement.
- Les modifications sont enregistrées dans la base de données.
- Avant la suppression, le système demande une confirmation.

#### US-03 : Afficher les événements

**User Story :**

En tant que visiteur, je veux afficher la liste des événements publiés afin de découvrir les événements disponibles.

**Critères d'acceptation :**

- La plateforme affiche uniquement les événements ayant le statut « publish ».
- Chaque événement affiche son titre, sa date, son lieu et son prix.
- Si aucun événement n'est disponible, un message informatif est affiché.

#### US-04 : Consulter les détails d'un événement

**User Story :**

En tant que visiteur, je veux consulter les détails d'un événement afin d'obtenir toutes les informations avant de participer.

**Critères d'acceptation :**

- Le visiteur peut sélectionner un événement depuis la liste.
- La page de détails affiche le titre, la description, la date, l'heure, le lieu et le prix.
- Les informations affichées correspondent à l'événement sélectionné.

### 2.5. Définition du MVP

Le MVP (Minimum Viable Product) de notre projet contient les fonctionnalités essentielles pour proposer une première version utilisable de la plateforme.

#### Fonctionnalités incluses dans le MVP

| Fonctionnalité | Utilisateur |
|---|---|
| Ajouter un événement | Organisateur |
| Consulter ses événements | Organisateur |
| Modifier un événement | Organisateur |
| Supprimer un événement | Organisateur |
| Afficher les événements publiés | Visiteur |
| Consulter les détails d'un événement | Visiteur |

**Remarque :**

Dans le prototype MVP, un organisateur prédéfini utilise l'espace de gestion. L'inscription et la connexion seront ajoutées dans une version future.

#### Fonctionnalités reportées aux versions futures

| Fonctionnalité | Description |
|---|---|
| Inscription et connexion | Permettre aux utilisateurs de créer un compte et de se connecter. |
| Réservation des billets | Permettre aux visiteurs de réserver une place pour un événement. |
| Paiement en ligne | Permettre de payer les billets directement sur la plateforme. |
| QR Code | Générer un code pour chaque billet réservé. |
| Notifications | Informer les utilisateurs des nouveaux événements. |

#### Conclusion sur le MVP

Le MVP se concentre sur la publication, la gestion et la consultation des événements.

Les fonctionnalités avancées, comme la réservation et le paiement en ligne, seront développées dans les versions futures.

---

## 3. Conclusion générale

Cette analyse permet de définir clairement les objectifs du projet Billetterie d'événements et de comprendre les besoins des utilisateurs.

La Vision Produit donne une direction au projet, les Personas représentent les utilisateurs cibles et les User Stories décrivent leurs besoins.

Les critères d'acceptation permettent de vérifier le bon fonctionnement des fonctionnalités, tandis que le MVP aide à sélectionner les fonctionnalités prioritaires pour la première version de l'application.