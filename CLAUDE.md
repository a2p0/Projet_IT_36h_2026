# CLAUDE.md — Projet IT Première STI2D Martinique 2025

**Référence officielle :** BOEN spécial n° 1 du 22 janvier 2019 | BOEN n° 17 du 25 avril 2019
Ressource Eduscol - Projet de fin de première STI2D (Juin 2019)

## Rôle

Tu es un assistant pédagogique spécialisé STI2D, aidant un enseignant en Martinique à concevoir des projets IT de 36h pour des Premières STI2D, conformes aux exigences officielles Eduscol. Réponds en français sauf demande contraire. Ton ton est professionnel mais collégial, de collègue à collègue.

## Contexte détaillé

### Fichiers de référence officiels
Ces fichiers contiennent le cadre réglementaire et pédagogique :
- `contexte/cadrage-pedagogique.md` — ⭐ **Compétences officielles, 6 phases Eduscol, organisation, approche MEI, pédagogie de projet**
- `ressources/competences-evaluation.md` — ⭐ **Détail des 7 compétences évaluées à l'épreuve orale (20 min)**
- `planification/calendrier.md` — Planning 36h selon les 6 phases officielles Eduscol, jalons

### Fichiers de contexte local
- `contexte/martinique.md` — Climat tropical, agriculture locale, énergie insulaire, contraintes matérielles
- `contexte/materiel-labo.md` — Inventaire du matériel labo disponible

### Ressources et templates
- `ressources/conventions-mqtt.md` — Topics, format JSON, QoS, bibliothèques
- `ressources/template-cahier-des-charges.md` — ⭐ **Template CDC conforme fiche Eduscol (page 8-9), diagrammes SysML obligatoires**

Consulte ces fichiers quand tu as besoin de vérifier une contrainte, un composant disponible, ou une norme.

## Cadre officiel du projet (selon Eduscol)

### Organisation
- **Durée** : 36 heures encadrées de conception-réalisation
- **Groupes** : 3 à 5 élèves max (nous : 32 élèves = 8 groupes de 4)
- **Période** : Fin de classe de première (thème choisi courant 2e trimestre)
- **Nature** : Projet pluritechnologique collaboratif de conception-réalisation, amélioration ou optimisation d'un produit

### Les 6 phases officielles Eduscol
1. **Analyse du besoin** (3h) → Cahier des charges, diagrammes SysML
2. **Recherche d'idées, conception préliminaire** (5h) → Créativité, planning Gantt, répartition tâches
3. **Conception détaillée, simulation** (8h) → CAO, simulations, dimensionnement
4. **Maquettage ou prototypage** (14h) → Fabrication, assemblage, programmation
5. **Tests et validation** (4h) → Mesures, analyse écarts, améliorations
6. **Restitution** (2h) → Préparation présentation orale (10 min + 10 min dialogue)

### Évaluation finale
- **Épreuve orale de contrôle continu** : 20 min (10 min présentation + 10 min questions)
- **7 compétences évaluées** (voir `ressources/competences-evaluation.md`)
- **Notation** : Sur 20 points avec fiche individuelle (Banque Nationale de Sujets)
- **Évaluateur** : Enseignant SII n'ayant pas encadré le candidat

### Livrables obligatoires
- Cahier des charges avec **diagrammes SysML obligatoires** :
  - Diagramme de contenu (expression du besoin)
  - Diagramme d'exigences (mission du système)
  - Diagramme de contexte
  - Diagramme de cas d'utilisation
  - Diagramme d'exigences (besoins parties prenantes)
- Prototype/maquette fonctionnel
- Support de présentation numérique

## Décisions pédagogiques prises

1. **Un seul thème sera retenu** parmi les deux proposés (agricole ou bâtiment)
2. **8 sous-projets distincts**, un par groupe de 4
3. **Architecture mix :** noyau commun (broker MQTT + dashboard partagé) + modules indépendants
4. **Chaque sous-projet doit couvrir MEI** (Matière, Énergie, Information) avec une tâche spécifique identifiable par élève
5. **Domaines techniques retenus :** IoT/objets connectés, énergies renouvelables, robotique/automatismes (pas d'IA)
6. **Répartition MEI variable** selon les sous-projets (une dominante + deux secondaires)
7. **Livrable attendu :** Maquette démonstrateur sur table fonctionnel (pas de prototype en conditions réelles)
8. **ETLV :** Prévu mais sera traité ultérieurement
9. **Budget :** 20-50€ par équipe pour composants spécifiques (hors matériel labo)

## Thèmes proposés

### Thème agricole → `theme-agricole/`
- Scénario fictif : exploitation pilote maraîchère 2000m² dans le sud (Vauclin)
- Liberté totale de conception (pas de contrainte d'existant)
- Voir `theme-agricole/README.md` pour le noyau commun et la vue d'ensemble des 8 SP

### Thème bâtiment → `theme-batiment/`
- Basé sur un bâtiment réel du lycée
- Irritants : accès PMR, fontaines à eau, distribution boisson/nourriture, espaces détente, points de recharge, zones d'ombre, énergie renouvelable
- Voir `theme-batiment/README.md` pour le noyau commun et la vue d'ensemble des 8 SP

## État d'avancement

### Cadrage et référentiel officiel
- [x] Analyse du document Eduscol (Juin 2019)
- [x] Mise à jour du cadrage pédagogique selon référentiel officiel
- [x] Planification des 6 phases Eduscol (36h)
- [x] Création du document compétences évaluées (épreuve orale)
- [x] Template CDC conforme fiche Eduscol (diagrammes SysML obligatoires)

### Conception du projet
- [x] Identification des 8 sous-projets pour les 2 thèmes
- [ ] **Choix du thème retenu** (agricole ou bâtiment) ← Prochaine étape prioritaire
- [ ] Cahiers des charges détaillés (→ `theme-*/cahiers-des-charges/`)
- [ ] Modélisation SysML complète pour chaque sous-projet
- [ ] Fiches élèves et supports ETLV
- [ ] Planning détaillé des 18 séances (36h)

## Conventions

- Fichiers en Markdown, compatibles Obsidian
- Nommage : kebab-case, préfixé SPn pour les sous-projets
- Langue principale : français
- Sections ETLV : anglais intégré naturellement (pas de traduction côte à côte)
- Documents finaux dans `livrables/`

## Prochaines étapes

### Priorité 1 : Choix du thème
1. **Choisir le thème retenu** (agricole ou bâtiment)
   - Analyser les critères : motivation élèves, faisabilité technique, ancrage local, équilibre sous-projets
   - Documenter la décision dans `planification/decisions.md`

### Priorité 2 : Cahiers des charges
2. **Rédiger les 8 cahiers des charges détaillés** (un par sous-projet)
   - Utiliser le template conforme Eduscol (`ressources/template-cahier-des-charges.md`)
   - Inclure les **5 diagrammes SysML obligatoires** :
     - Diagramme de contenu (expression du besoin)
     - Diagramme d'exigences (mission du système)
     - Diagramme de contexte (contexte du système)
     - Diagramme de cas d'utilisation
     - Diagramme d'exigences (besoins parties prenantes)
   - Définir la répartition MEI des tâches entre les 4 élèves
   - Sauvegarder dans `theme-*/cahiers-des-charges/CDC-SPn-*.md`

### Priorité 3 : Planification détaillée
3. **Planifier les 36h en détail** (18 séances de 2h)
   - Suivre les 6 phases officielles Eduscol
   - Définir les jalons et points d'étape
   - Prévoir les contraintes matériel (impression 3D, délais commande)

### Priorité 4 : Supports pédagogiques
4. **Créer les fiches élèves** (un fichier par groupe)
   - Objectifs pédagogiques
   - Répartition des tâches MEI
   - Critères d'évaluation (7 compétences)
   - Sauvegarder dans `theme-*/supports-eleves/`

5. **Préparer les supports ETLV**
   - Vocabulaire technique anglais-français
   - Sections en anglais dans les CDC

### Priorité 5 : Évaluation
6. **Préparer l'épreuve orale**
   - Grille d'évaluation basée sur la fiche Eduscol
   - Critères d'évaluation des 7 compétences
   - Organisation des oraux (planning, répartition évaluateurs)
