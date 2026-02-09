# Calendrier — Projet IT 36h

**Référence :** Planning basé sur les 6 phases officielles Eduscol (Ressource Juin 2019)

## Vue d'ensemble

- **Durée totale** : 36 heures encadrées de conception-réalisation
- **Effectif** : 32 élèves, 8 groupes de 4
- **Période** : Fin de classe de première (thème choisi courant 2e trimestre)
- **Modalités** : Projet pluritechnologique collaboratif

## Les 6 phases officielles du projet (selon Eduscol)

| Phase | Durée estimée | Type d'activités | Livrables attendus | Jalons |
|-------|--------------|------------------|-------------------|--------|
| **Phase 1 : Analyse du besoin** | 3h | Équipe, investigation | Cahier des charges, performances initiales, phasage | J1 - Validation CDC |
| **Phase 2 : Recherche d'idées, conception préliminaire** | 5h | Équipe, investigation | Description fonctionnelle, concept, planning et répartition des tâches, créativité | J2 - Validation concept |
| **Phase 3 : Conception détaillée, simulation** | 8h | Équipe + tâches individuelles | Dossier de conception, maquette numérique, performances simulées | J3 - Validation conception |
| **Phase 4 : Maquettage ou prototypage** | 14h | Équipe + tâches individuelles | Sous-ensemble fonctionnel (prototype) réalisé et intégré, protocole de tests | J4 - Proto fonctionnel |
| **Phase 5 : Tests et validation** | 4h | Équipe | Bilan technique, performances mesurées, écarts, causes, propositions d'amélioration | J5 - Validation performances |
| **Phase 6 : Restitution** | 2h | Équipe | Présentation du projet (support numérique) pour épreuve IT | J6 - Épreuve orale |

**Total** : 36h

## Détail des jalons et points d'étape

Les points d'étape permettent de (selon Eduscol) :
- Rendre compte des activités de chacun et faire le point sur l'avancement
- Vérifier les documents produits attestant des résultats obtenus
- Confronter les solutions et détecter les risques
- Valider les jalons pour passer à l'étape suivante
- Partager les informations au sein de l'équipe
- Prendre des décisions pour la suite du projet

| Jalon | Fin de phase | Documents à vérifier | Décisions à prendre |
|-------|--------------|----------------------|---------------------|
| **J1** | Phase 1 | Cahier des charges complété, diagrammes SysML (besoin, contexte, cas d'utilisation, exigences), répartition des tâches | Validation CDC, autorisation de passer en conception |
| **J2** | Phase 2 | Description fonctionnelle, concepts proposés (créativité), planning individuel (Gantt), répartition MEI | Choix de la solution retenue, validation du planning |
| **J3** | Phase 3 | Dossier de conception détaillée, maquettes numériques (CAO, schémas), simulations, liste composants/matériel | Validation conception, commande matériel si nécessaire |
| **J4** | Phase 4 | Prototype/maquette fonctionnel, protocole de tests défini, documentation technique | Vérification fonctionnement, autorisation tests |
| **J5** | Phase 5 | Bilan technique, mesures de performances, analyse des écarts, propositions d'amélioration | Validation finale, préparation restitution |
| **J6** | Phase 6 | Support de présentation (diaporama, poster, CAO, vidéo démo), documentation complète | Évaluation lors de l'épreuve orale de 20 min |

## Planning détaillé (à compléter après choix du thème)

### Semaine 1

*À détailler une fois le thème choisi et les CDC rédigés*

### Semaine 2

*À détailler*

## Adaptation spécifique au contexte (thèmes agricole/bâtiment)

### Phase 1 : Analyse du besoin (3h)
- **Séance 1 (2h)** : Présentation du scénario fédérateur, constitution des groupes, attribution des sous-projets
- **Séance 2 (1h)** : Définition collective des conventions MQTT (topics, format JSON, QoS), décodage du CDC fourni

### Phase 2 : Recherche d'idées (5h)
- **Séance 3 (3h)** : Brainstorming créativité, recherche de solutions existantes, benchmark
- **Séance 4 (2h)** : Choix de la solution, planification détaillée (Gantt), répartition des tâches MEI entre les 4 élèves

### Phase 3 : Conception détaillée (8h)
- **Séances 5-6 (4h)** : Modélisation SysML complète (BDD, IBD), schémas, CAO
- **Séances 7-8 (4h)** : Simulations, dimensionnement énergétique, calculs, choix composants définitifs

### Phase 4 : Prototypage (14h)
- **Séances 9-12 (8h)** : Fabrication (impression 3D, découpe, assemblage, câblage)
- **Séances 13-15 (6h)** : Programmation (Arduino/ESP32), configuration MQTT, intégration

### Phase 5 : Tests et validation (4h)
- **Séance 16 (2h)** : Tests unitaires, mesures, relevés de performances
- **Séance 17 (2h)** : Intégration au dashboard central, tests d'intégration, analyse des écarts, améliorations

### Phase 6 : Restitution (2h)
- **Séance 18 (2h)** : Préparation du support de présentation, répétition présentation orale (10 min + 10 min questions)

## Contraintes à prendre en compte

- Disponibilité du matériel labo (un seul Raspberry Pi pour le broker MQTT central ?)
- Salles informatiques pour la partie simulation/SysML/CAO
- Temps de fabrication (impression 3D, découpe laser) à anticiper et planifier
- Période de commande des composants spécifiques (délai livraison, validation budget)
- Coordination entre les 8 groupes pour l'intégration MQTT

## Évaluation finale

**Épreuve commune de contrôle continu** (BOEN n° 17 du 25 avril 2019)
- **Nature** : Épreuve orale
- **Durée** : 20 minutes (10 min présentation + 10 min dialogue argumenté)
- **Évaluateur** : Enseignant SII n'ayant pas encadré le candidat
- **Support** : Présentation numérique préparée par l'élève (diaporama, poster, CAO, vidéo, etc.)
- **Notation** : Sur 20 points avec fiche individuelle d'évaluation des compétences (Banque Nationale de sujets)
- **Contenu** : L'élève présente son travail personnel (issu de la répartition des tâches), peut s'appuyer sur les choix collectifs

## Notes

- Ce planning sera affiné après rédaction des cahiers des charges
- Prévoir du temps tampon pour les imprévus (1-2h de marge sur les phases 3 et 4)
- Adapter selon progression réelle des groupes
- Points d'étape réguliers pour suivre l'avancement et détecter les risques
