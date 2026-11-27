# Comprendre l'approche Agile et le cadre Scrum

## 1. Objectif de l'atelier

L'objectif est de comprendre la différence entre Cascade et Agile.

Nous allons aussi découvrir Scrum et son organisation du travail.

Nous utilisons notre projet : **Billetterie d'événements**.

La plateforme permet d'ajouter et d'afficher des événements.

Le projet utilise trois tables principales :

- **Organisateur**
- **Event**
- **Category**

La table principale est **Event**.

## 2. Approche Cascade et approche Agile

### 2.1. Approche Cascade (Cycle en V)

La méthode Cascade organise le projet en étapes.

Chaque étape se termine avant de commencer la suivante.

Les étapes sont :

1. Analyse des besoins.
2. Conception.
3. Développement.
4. Tests.
5. Livraison.

**Avantages :**
- Le travail est planifié au début.
- Les étapes sont claires.
- La méthode est adaptée aux besoins stables.

**Limites :**
- Les changements sont difficiles et coûteux.
- Le client voit le résultat tard.
- Une erreur au début peut créer des problèmes après.

### 2.2. Approche Agile

Agile permet de travailler par petits cycles.

L'équipe développe une partie du produit, la teste et la présente au client.

Ensuite, elle reçoit des avis (*Feedback*) et améliore le produit.

**Avantages :**
- Le produit avance progressivement.
- Le client donne son avis régulièrement.
- L'équipe peut changer les priorités.

### 2.3. Différence entre Cascade et Agile

| Cascade | Agile |
|---|---|
| Plan au début | Plan adapté régulièrement |
| Étapes successives | Cycles courts |
| Résultat à la fin | Résultat régulièrement |
| Changements difficiles | Changements possibles |

**À retenir :** Agile utilise un plan, mais l'équipe peut l'adapter selon les besoins.

## 3. Les quatre valeurs du Manifeste Agile

Les quatre valeurs expliquent comment une équipe Agile travaille.

1. **Les individus et les interactions**
   - Communiquer et travailler ensemble.

2. **Un logiciel opérationnel**
   - Donner la priorité à un produit qui fonctionne.

3. **La collaboration avec le client**
   - Échanger avec le client pendant le projet.

4. **L'adaptation au changement**
   - Changer les priorités si les besoins changent.

**Exemple :**

Dans notre Billetterie, les utilisateurs demandent une meilleure recherche des événements.

L'équipe peut ajouter cette amélioration dans un prochain Sprint.

## 4. Les trois piliers de Scrum

Scrum utilise trois piliers :

| Pilier | Explication simple | Exemple |
|---|---|---|
| **Transparence** | Le travail est visible pour tous. | L'équipe voit le Product Backlog et les tâches. |
| **Inspection** | Vérifier le travail régulièrement. | Présenter la liste des événements pendant la Sprint Review. |
| **Adaptation** | Améliorer le travail après une vérification. | Modifier l'affichage des événements après les avis. |

## 5. Les trois rôles Scrum

Scrum définit trois responsabilités principales.

### 5.1. Product Owner (PO)

- Définit les besoins du produit.
- Organise les priorités du Product Backlog.
- Cherche à donner plus de valeur au produit.

**Exemple :** donner la priorité à l'ajout et à l'affichage des événements.

### 5.2. Scrum Master (SM)

- Aide l'équipe à utiliser Scrum.
- Facilite les réunions.
- Aide à résoudre les problèmes.

**Exemple :** aider l'équipe lorsqu'un problème bloque le développement.

### 5.3. Développeurs

- Développent les fonctionnalités.
- Organisent leur travail.
- Choisissent comment réaliser les tâches.

**Exemple :** créer le formulaire d'ajout et la page d'affichage des événements.

**Important :** les trois rôles travaillent ensemble. Il n'y a pas de chef entre eux.

## 6. Les cinq événements Scrum

Le **Sprint** est une période de travail fixe. Il contient les quatre autres événements.

| Événement | Objectif |
|---|---|
| **1. Sprint** | Créer une partie fonctionnelle du produit. |
| **2. Sprint Planning** | Choisir et planifier le travail. |
| **3. Daily Scrum** | Vérifier le travail chaque jour (15 minutes maximum). |
| **4. Sprint Review** | Présenter le résultat et recevoir les avis. |
| **5. Sprint Retrospective** | Améliorer le travail de l'équipe. |

**À retenir :**

Le Daily Scrum aide les Développeurs à organiser leur travail. Ce n'est pas une réunion pour faire un rapport au Scrum Master.

## 7. Increment et Definition of Done (DoD)

### 7.1. Increment

Un **Increment** est une partie du produit qui fonctionne et qui respecte la Definition of Done.

Il s'ajoute aux parties déjà terminées.

**Exemple :**

À la fin du premier Sprint, un organisateur peut ajouter un événement et voir les événements enregistrés.

### 7.2. Definition of Done (DoD)

La **DoD** définit les conditions pour dire qu'une fonctionnalité est terminée.

Pour notre Billetterie :

- Le formulaire d'ajout fonctionne.
- Les champs sont validés.
- Les événements sont enregistrés dans MySQL.
- Les événements s'affichent correctement.
- Les tests sont réussis.
- Le code est intégré et vérifié.

**À retenir :** toute l'équipe utilise les mêmes règles de qualité.

## 8. Application de Scrum à la Billetterie d'événements

### 8.1. Vision du produit

Créer une plateforme pour ajouter et afficher des événements.

Chaque événement contient des informations comme le titre, la date, le lieu et le prix.

### 8.2. Les trois tables principales

| Table | Rôle |
|---|---|
| **Event** | Contient les informations des événements. |
| **Organisateur** | Contient les informations des organisateurs. |
| **Category** | Classe les événements par catégorie. |

Les relations suivent le modèle de données du projet.

### 8.3. Exemple de Product Backlog

Le **Product Backlog** est une liste de besoins du produit.

Voici quelques exemples :

1. En tant qu'organisateur, je veux ajouter un événement.
2. En tant que visiteur, je veux voir la liste des événements.
3. En tant que visiteur, je veux voir les détails d'un événement.
4. En tant qu'organisateur, je veux choisir une catégorie pour mon événement.

Le Product Owner confirme et organise ces besoins.

### 8.4. Exemple du premier Sprint

**Durée proposée :** une semaine.

**Objectif du Sprint :**

Permettre à l'organisateur d'ajouter un événement et de voir la liste des événements.

| Étape | Travail |
|---|---|
| Sprint Planning | Choisir l'ajout et l'affichage des événements. |
| Daily Scrum | Vérifier le travail chaque jour. |
| Développement | Créer le formulaire et la page d'affichage. |
| Sprint Review | Présenter les fonctionnalités et recevoir les avis. |
| Sprint Retrospective | Trouver des améliorations pour le prochain Sprint. |

**Increment attendu :**

Une première version fonctionnelle qui permet d'ajouter et d'afficher les événements avec MySQL.

**Limite du Sprint 1 :**

Ce Sprint concerne seulement l'ajout et l'affichage des événements. Il ne comprend pas toutes les fonctionnalités de la Billetterie.

## 9. Préparation de la présentation (5 à 10 minutes)

| Partie | Temps | Sujet |
|---|---:|---|
| Introduction | 30 secondes | Présenter Agile, Scrum et le projet. |
| Cascade et Agile | 1 minute | Expliquer la différence. |
| Valeurs et piliers | 1 min 30 | Présenter les valeurs et les piliers. |
| Rôles Scrum | 1 minute | Présenter les trois rôles. |
| Événements Scrum | 1 min 30 | Présenter les cinq événements. |
| Premier Sprint | 2 minutes | Expliquer l'objectif et le résultat. |
| Conclusion | 30 secondes | Résumer l'intérêt de Scrum. |

### Exemple de conclusion orale

« Dans notre projet Billetterie d'événements, Scrum nous aide à travailler étape par étape.

Au premier Sprint, nous créons une première version pour ajouter et afficher les événements.

Nous présentons le résultat et nous recevons des avis.

Ensuite, nous améliorons le produit dans le prochain Sprint. »

## 10. Sources

- [Manifeste Agile](https://agilemanifesto.org/iso/fr/manifesto.html)
- [Guide Scrum officiel en français](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-French.pdf)