# Journal des décisions — Projet IT 36h

Ce fichier documente les décisions importantes prises au fil du projet, avec leur justification.

## Format

Chaque décision suit ce format :
- **Date** : JJ/MM/AAAA
- **Décision** : Description concise
- **Justification** : Pourquoi cette décision
- **Impact** : Sur quoi cela influe

---

## Décisions prises

### 09/02/2026 — Structure de dossiers étendue

- **Décision** : Ajout de `planification/`, `notes/`, et `supports-eleves/` dans chaque thème
- **Justification** :
  - Meilleure organisation du suivi de projet
  - Séparation claire entre conception (sous-projets/) et supports pédagogiques
  - Facilite l'utilisation de Claude CLI avec contexte ciblé
- **Impact** : Structure de fichiers plus complète, besoin de créer davantage de documents

### [Date antérieure] — Un seul thème retenu

- **Décision** : Choix entre thème agricole et bâtiment (décision à prendre)
- **Justification** :
  - 32 élèves = 8 groupes, un thème cohérent facilite les interconnexions MQTT
  - Évite la dispersion pédagogique
- **Impact** : Les 8 sous-projets doivent s'intégrer dans un scénario commun

### [Date antérieure] — 8 sous-projets distincts

- **Décision** : 8 sous-projets, un par groupe de 4
- **Justification** :
  - 32 élèves / 4 = 8 groupes
  - Permet diversité technique tout en gardant cohérence d'ensemble
- **Impact** : Nécessite architecture commune (broker MQTT + dashboard)

### [Date antérieure] — Architecture mix noyau commun + modules indépendants

- **Décision** : Broker MQTT central + dashboard partagé + modules indépendants
- **Justification** :
  - Travail collaboratif entre groupes
  - Chaque groupe reste autonome sur son sous-projet
  - Réaliste par rapport au temps disponible (36h)
- **Impact** : Définition collective des conventions MQTT obligatoire en début de projet

### [Date antérieure] — Couverture MEI obligatoire

- **Décision** : Chaque sous-projet doit traiter Matière, Énergie, Information
- **Justification** :
  - Programme STI2D exige transversalité MEI
  - Chaque élève doit avoir une tâche spécifique identifiable
- **Impact** : Répartition MEI variable selon les sous-projets (dominante + secondaires)

### [Date antérieure] — Domaines techniques retenus

- **Décision** : IoT/objets connectés + énergies renouvelables + robotique/automatismes (pas d'IA)
- **Justification** :
  - Matériel labo disponible adapté
  - Cohérence avec le contexte Martinique
  - Évite complexité excessive pour un projet 36h
- **Impact** : Les sous-projets doivent s'inscrire dans ces domaines

### [Date antérieure] — Livrable minimum vs idéal

- **Décision** :
  - Minimum = simulation/modélisation + quelques éléments physiques
  - Idéal = maquette démonstrateur sur table
  - Pas de prototype en conditions réelles
- **Justification** :
  - Réaliste avec 36h et budget limité
  - Évite frustration des groupes
  - Focus sur la conception + validation principe
- **Impact** : Critères d'évaluation adaptés, acceptation de maquettes simplifiées

### [Date antérieure] — Conception en deux phases

- **Décision** :
  1. Phase théorique (matériel idéal)
  2. Phase prototypage (matériel disponible)
- **Justification** :
  - Permet de ne pas brider la créativité en phase conception
  - Réalisme en phase prototypage
  - Apprentissage de l'adaptation
- **Impact** : Besoin de bien distinguer ces deux phases dans le planning 36h

### [Date antérieure] — Budget 20-50€ par équipe

- **Décision** : Budget maxi 50€ par groupe pour composants spécifiques
- **Justification** :
  - Matériel labo couvre l'essentiel (Arduino, capteurs, ESP32...)
  - Budget pour éléments spécifiques (matériaux, connecteurs, petits moteurs...)
  - Total 8 × 50€ = 400€ max gérable
- **Impact** : Besoin d'identifier précisément les achats dans chaque CDC

---

## Décisions en attente

- [ ] **Choix du thème** : agricole ou bâtiment ?
- [ ] **Organisation ETLV** : intégration dans le projet ou module séparé ?
- [ ] **Modalités d'évaluation** : grille par compétence CO1-CO4 ou note globale ?
- [ ] **Planning détaillé** : répartition des 36h par phase ?

## Notes

- Mettre à jour ce fichier à chaque décision structurante
- Référencer ce fichier dans les discussions avec collègues
- Utile pour justifier les choix pédagogiques auprès de la hiérarchie
