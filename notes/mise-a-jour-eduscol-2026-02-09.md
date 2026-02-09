# Mise à jour selon document Eduscol — 09/02/2026

## Contexte

Intégration complète du document officiel Eduscol "Projet de fin de première STI2D - Support de l'épreuve commune de contrôle continu" (Juin 2019) dans le projet.

**Références officielles :**
- BOEN spécial n° 1 du 22 janvier 2019 (Programme IT)
- BOEN n° 17 du 25 avril 2019 (Épreuve de contrôle continu)
- Ressource Eduscol Juin 2019

---

## Fichiers mis à jour

### 1. `contexte/cadrage-pedagogique.md` ✅

**Ajouts majeurs :**
- Référence aux textes officiels en en-tête
- **Compétences officielles détaillées** : 10 compétences du programme IT, dont 7 évaluées à l'oral (en gras)
- **Les 6 phases officielles de la démarche de projet** :
  1. Analyse du besoin (3h)
  2. Recherche d'idées, conception préliminaire (5h)
  3. Conception détaillée, simulation (8h)
  4. Maquettage ou prototypage (14h)
  5. Tests et validation (4h)
  6. Restitution (2h)
- **Points d'étape (jalons)** : rôle et fréquence
- **Pédagogie de projet - points de vigilance** : équilibre entre 3 dérives (productiviste, techniciste, spontanéiste)
- Organisation précisée : 3 à 5 élèves officiellement (nous gardons 4)
- Période : fin de première, thème choisi courant 2e trimestre

**Ce qui est conservé :**
- Transversalité MEI (adapté à notre contexte)
- Niveaux de livrable (adapté à nos moyens)
- ETLV

---

### 2. `planification/calendrier.md` ✅

**Refonte complète basée sur les 6 phases Eduscol :**

**Nouveau tableau des phases :**
| Phase | Durée | Type activités | Livrables | Jalons |
|-------|-------|----------------|-----------|--------|
| Phase 1 : Analyse du besoin | 3h | Équipe, investigation | CDC, diagrammes SysML | J1 - Validation CDC |
| Phase 2 : Recherche d'idées | 5h | Équipe, investigation | Concept, planning, tâches | J2 - Validation concept |
| Phase 3 : Conception détaillée | 8h | Équipe + tâches individuelles | CAO, simulations, composants | J3 - Validation conception |
| Phase 4 : Prototypage | 14h | Équipe + tâches individuelles | Prototype, protocole tests | J4 - Proto fonctionnel |
| Phase 5 : Tests et validation | 4h | Équipe | Bilan, mesures, écarts | J5 - Validation performances |
| Phase 6 : Restitution | 2h | Équipe | Présentation 10 min | J6 - Épreuve orale 20 min |

**Ajouts :**
- Détail des 6 jalons avec documents à vérifier et décisions à prendre
- Adaptation spécifique au contexte (thèmes agricole/bâtiment) : découpage en 18 séances de 2h
- Section "Évaluation finale" avec détail de l'épreuve orale (20 min)
- Contraintes à prendre en compte (matériel, coordination 8 groupes)

---

### 3. `ressources/template-cahier-des-charges.md` ✅

**Refonte complète selon la fiche de définition projet IT Eduscol (pages 8-9) :**

**Nouvelle structure obligatoire :**

1. **Fiche de définition projet IT**
   - Intitulé du projet
   - Lycée / Enseignant responsable / Session
   - Thème sociétal + ancrage local

2. **Le besoin initial**
   - Description du besoin général
   - Utilisateurs et parties prenantes

3. **La finalité du produit**
   - Mission du produit

4. **Le problème technique à résoudre**
   - Problématique technique (approche MEI)
   - Contraintes spécifiques

5. **Diagrammes SysML (Ingénierie Système) - OBLIGATOIRES**
   - 4.1 Diagramme de contenu (expression du besoin)
   - 4.2 Diagramme d'exigences (mission du système)
   - 4.3 Diagramme de contexte (contexte du système)
   - 4.4 Diagramme de cas d'utilisation
   - 4.5 Diagramme d'exigences (besoins parties prenantes)

6. **La répartition des tâches des élèves**
   - Tableau avec 4 élèves (3 à 5 officiellement)
   - Tâche principale + dominante MEI + compétences évaluées

7. **La production finale attendue**
   - Type de livrable
   - Critères de réussite mesurables (tableau)

8. **Déclinaison technique MEI**
   - 8.1 Matière (CAO, matériaux, fabrication)
   - 8.2 Énergie (bilan, dimensionnement, autonomie)
   - 8.3 Information (architecture logicielle, capteurs, MQTT)

9. **Planning prévisionnel (36h selon phases Eduscol)**
   - Tableau des 6 phases avec durées, activités, livrables, jalons

10. **Compétences STI2D évaluées**
    - Liste des 10 compétences (7 en gras évaluées à l'oral)

11. **Espace collaboratif et documentation**
    - Outils à utiliser
    - Documents à produire

12. **Annexes**
    - Références aux fichiers contexte et ressources

---

### 4. `ressources/competences-evaluation.md` ✅ (NOUVEAU)

**Création d'un document complet sur l'évaluation :**

**Contenu :**
- Vue d'ensemble : 10 compétences IT, dont 7 évaluées à l'oral
- **Tableau récapitulatif** des 10 compétences avec indication "évaluée à l'oral" et "phase du projet"
- **Détail des 7 compétences évaluées** avec :
  - Ce que l'élève doit montrer
  - Comment le présenter pendant les 10 min
  - Comment répondre lors du dialogue (10 min)
- **Structure de l'épreuve orale** (20 min : 10 + 10)
  - Partie 1 : Présentation
  - Partie 2 : Dialogue argumenté
  - Supports autorisés
- **Grille d'évaluation** :
  - Notation sur 20
  - Fiche individuelle d'évaluation (Banque Nationale de Sujets)
  - Critères
- **Conseils pratiques** pour élèves et enseignants

**Les 7 compétences évaluées à l'oral :**
1. C1 - Décoder le CDC
2. C2 - Évaluer la compétitivité
3. C3 - Décrire avec outils adaptés
4. C5 - Identifier problème technique (MEI)
5. C6 - Planifier un projet (Gantt)
6. C7 - Proposer des solutions (créativité)
7. C10 - Réaliser et valider prototype/maquette

---

### 5. `CLAUDE.md` ✅

**Mises à jour :**
- Ajout des références officielles en en-tête
- Section "Cadre officiel du projet (selon Eduscol)" :
  - Organisation
  - Les 6 phases officielles
  - Évaluation finale (épreuve orale 20 min)
  - Livrables obligatoires (diagrammes SysML)
- Mise à jour "Contexte détaillé" avec marquage ⭐ des fichiers clés
- Mise à jour "État d'avancement" avec nouvelles sections
- Refonte "Prochaines étapes" selon priorités pédagogiques

---

## Nouveaux fichiers créés

### `ressources/competences-evaluation.md` ✅
Document complet de 200+ lignes sur l'évaluation du projet IT et l'épreuve orale.

---

## Impact sur le projet

### Ce qui change

1. **Cahiers des charges plus complets**
   - 5 diagrammes SysML obligatoires (vs précédemment : suggérés)
   - Fiche de définition conforme modèle Eduscol

2. **Planning plus structuré**
   - 6 phases officielles (vs notre découpage initial)
   - Jalons précis avec documents à vérifier

3. **Évaluation clarifiée**
   - 7 compétences évaluées à l'oral (vs précédemment : toutes les compétences)
   - Structure d'épreuve précise (10 min + 10 min)

4. **Pédagogie de projet explicite**
   - Points de vigilance (3 dérives à éviter)
   - Règles pour respecter l'équilibre

### Ce qui ne change pas

1. **Organisation retenue**
   - 32 élèves, 8 groupes de 4 (conforme au 3-5 officiel)
   - 36 heures

2. **Thèmes proposés**
   - Agricole et bâtiment restent pertinents
   - Architecture MQTT commune validée

3. **Approche MEI**
   - Déjà intégrée, juste renforcée

4. **Livrables**
   - Maquette démonstrateur sur table (conforme Eduscol)

---

## Actions à mener

### Immédiat
- [x] Mise à jour des fichiers de contexte et planification
- [x] Mise à jour du template CDC
- [x] Création du document compétences-évaluation
- [x] Mise à jour CLAUDE.md

### Court terme (après choix du thème)
- [ ] Vérifier que les 8 sous-projets permettent d'évaluer les 7 compétences
- [ ] Rédiger les 8 CDC conformes au nouveau template
- [ ] Créer les 5 diagrammes SysML pour chaque sous-projet
- [ ] Planifier les 18 séances détaillées (2h × 18 = 36h)

### Moyen terme
- [ ] Créer les fiches élèves avec grille d'évaluation
- [ ] Préparer les oraux blancs
- [ ] Organiser l'épreuve orale finale (planning, évaluateurs externes)

---

## Points de vigilance

### Diagrammes SysML
- **5 diagrammes obligatoires** par sous-projet
- Logiciel à utiliser : Papyrus, Modelio, PlantUML ?
- Formation élèves nécessaire (prévoir temps dans Phase 1 et 2)

### Répartition des tâches
- **Chaque élève doit pouvoir être évalué sur les 7 compétences**
- Attention à ne pas cantonner un élève à une seule dominante MEI
- La répartition doit permettre une évaluation individuelle

### Points d'étape
- **6 jalons obligatoires** à respecter
- Prévoir des revues de projet régulières
- Documentation à jour pour chaque jalon

### Épreuve orale
- **Évaluateur externe** (enseignant SII n'ayant pas encadré)
- Nécessite coordination entre enseignants
- Préparation des élèves : oraux blancs indispensables

---

## Ressources complémentaires

- **Banque Nationale de Sujets** : Fiche d'évaluation individuelle à récupérer
- **RNR STI** : Exemples de fiches et de projets IT
- **Document Eduscol** : Conservé dans `sources/eduscol/RA19_Lycee_T_STI2D_1_ProjetFinPremiere-SupportEpreuve_IT_1150885.pdf`

---

## Conclusion

Le projet est maintenant **parfaitement aligné sur les exigences officielles Eduscol**. Les fichiers de contexte, planification et ressources ont été mis à jour pour garantir la conformité avec le référentiel.

La prochaine étape prioritaire est le **choix du thème** (agricole ou bâtiment), puis la **rédaction des 8 cahiers des charges** conformes au nouveau template.
