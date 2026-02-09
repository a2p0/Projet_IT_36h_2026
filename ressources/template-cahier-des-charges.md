# Template — Cahier des Charges (CDC)

**Référence :** Conforme à la fiche de définition projet IT Eduscol (Juin 2019)

> Ce template sera utilisé pour rédiger le cahier des charges de chaque sous-projet.
> Le CDC est fourni par l'enseignant via un espace collaboratif de travail.

---

## Fiche de définition projet IT

### Intitulé du projet

[Nom complet du sous-projet]

### Lycée concerné | Enseignant responsable

- **Lycée** : [Nom du lycée]
- **Enseignant responsable du suivi du projet** : [Nom]
- **Session** : [Année scolaire]

### Thème sociétal

[Décrire le thème sociétal : développement durable, agriculture connectée, smart building, aide à la personne, santé, diminution des consommations énergétiques, etc.]

**Ancrage local Martinique** : [Contextualiser par rapport au climat tropical, agriculture locale, énergie insulaire, etc.]

---

## 1. Le besoin initial

**Description du besoin général associé à un enjeu global authentique :**

[Décrire le besoin auquel répond le projet. Quel problème cherche-t-on à résoudre ?]

**Utilisateurs et parties prenantes :**
- [Utilisateur principal]
- [Partie prenante 1]
- [Partie prenante 2]

---

## 2. La finalité du produit

**Mission du produit :**

[Quelle est la mission du système ? Que doit-il faire concrètement ?]

---

## 3. Le problème technique à résoudre

**Problématique technique identifiée :**

[Décrire le problème technique spécifique que ce sous-projet doit résoudre. Approche MEI (Matière, Énergie, Information)]

**Contraintes spécifiques :**
- Matériaux et composants disponibles (voir `contexte/materiel-labo.md`)
- Budget : 20-50€ par équipe pour composants spécifiques (hors matériel labo)
- Dimensions : Maquette démonstrateur sur table
- Environnement : Climat tropical martiniquais
- Communication : Protocole MQTT (voir `ressources/conventions-mqtt.md`)

---

## 4. Diagrammes SysML (Ingénierie Système)

**Éléments obligatoires du cahier des charges selon Eduscol :**

### 4.1 Diagramme de contenu (expression du besoin)

[Insérer image ou description du diagramme de contenu]

**Bête à cornes :**
- À qui rend-il service ?
- Sur quoi agit-il ?
- Dans quel but ?

### 4.2 Diagramme d'exigences (mission du système)

[Insérer image ou description du diagramme d'exigences - mission]

**Exigences principales :**
- EX1 : [Exigence 1]
- EX2 : [Exigence 2]
- EX3 : [Exigence 3]

### 4.3 Diagramme de contexte (contexte du système)

[Insérer image ou description du diagramme de contexte]

**Environnement du système :**
- [Élément extérieur 1]
- [Élément extérieur 2]
- [Élément extérieur 3]

### 4.4 Diagramme de cas d'utilisation (utilisation du système)

[Insérer image ou description du diagramme de cas d'utilisation]

**Cas d'utilisation identifiés :**
- UC1 : [Cas d'utilisation 1]
- UC2 : [Cas d'utilisation 2]
- UC3 : [Cas d'utilisation 3]

### 4.5 Diagramme d'exigences (besoins des parties prenantes)

[Insérer image ou description du diagramme d'exigences - parties prenantes]

**Besoins par partie prenante :**
- Utilisateur principal : [Besoins]
- Mainteneur : [Besoins]
- Environnement : [Besoins]

---

## 5. La répartition des tâches des élèves

**Effectif du groupe :** 4 élèves (officiellement 3 à 5 maximum)

**Principe :** Chaque élève doit avoir une tâche spécifique identifiable. La répartition doit permettre d'évaluer chaque élève sur l'ensemble des compétences visées par l'épreuve commune de contrôle continu.

| Élève | Nom | Tâche principale | Dominante MEI | Compétences évaluées |
|-------|-----|------------------|---------------|----------------------|
| **Élève 1** | [Nom] | [Description de la tâche spécifique] | **M**atière | Conception CAO, fabrication, choix matériaux |
| **Élève 2** | [Nom] | [Description de la tâche spécifique] | **E**nergie | Dimensionnement énergétique, bilan puissance |
| **Élève 3** | [Nom] | [Description de la tâche spécifique] | **I**nformation | Programmation, capteurs, communication MQTT |
| **Élève 4** | [Nom] | [Description de la tâche spécifique] | Transverse | Planification, tests, intégration, documentation |

**Note :** Bien que chaque élève ait une tâche principale et une dominante MEI, tous contribuent collectivement à l'ensemble du projet et participent aux choix communs.

---

## 6. La production finale attendue

**Type de livrable :**
- [x] Prototype/Maquette démonstrateur sur table
- [x] Documentation technique (dossier de conception)
- [x] Support de présentation numérique (diaporama, poster, CAO, vidéo)
- [x] Intégration au système global (communication MQTT avec dashboard central)

**Critères de réussite mesurables :**

| Critère | Niveau attendu | Moyen de vérification |
|---------|----------------|-----------------------|
| Critère 1 : [Ex: Autonomie énergétique] | [Ex: 48h min] | Mesure avec multimètre, calcul |
| Critère 2 : [Ex: Précision capteur] | [Ex: ±2°C] | Test comparatif, étalonnage |
| Critère 3 : [Ex: Communication MQTT] | [Ex: 100% messages reçus] | Test intégration dashboard |
| Critère 4 : [Ex: Temps de réponse] | [Ex: < 5 secondes] | Chronométrage, test utilisateur |

---

## 7. Déclinaison technique MEI (Matière, Énergie, Information)

### 7.1 Matière
**Composants à concevoir/fabriquer :**
- [Liste des pièces à concevoir]
- [Matériaux retenus et justification]
- [Procédés de fabrication : impression 3D, découpe laser, assemblage]

**Diagrammes associés :** BDD (Block Definition Diagram), IBD (Internal Block Diagram)

### 7.2 Énergie
**Bilan énergétique :**
- Source d'alimentation : [Batterie, solaire, secteur, etc.]
- Puissance consommée : [Estimation en W]
- Autonomie visée : [Durée]
- Dimensionnement : [Calculs de validation]

**Lien avec le sous-projet SP5/SP7 (centrale solaire) si pertinent**

### 7.3 Information
**Architecture logicielle :**
- Microcontrôleur : [Arduino, ESP32, Raspberry Pi, etc.]
- Langage : [C++, Python, etc.]
- Bibliothèques : [MQTT, capteurs, etc.]

**Capteurs et actionneurs :**
- [Liste des capteurs avec références]
- [Liste des actionneurs avec références]

**Communication MQTT :**
- Topics publiés : `ferme/{module}/{donnee}` ou `campus/{module}/{donnee}`
- Format JSON : voir `ressources/conventions-mqtt.md`
- Fréquence de publication : [ex: toutes les 5 min]

**Interface utilisateur :**
- Dashboard Node-RED (intégration au dashboard central)
- [Autre interface si pertinent]

---

## 8. Planning prévisionnel (36h selon phases Eduscol)

| Phase | Durée | Activités | Livrables | Jalon |
|-------|-------|-----------|-----------|-------|
| **Phase 1 : Analyse du besoin** | 3h | Décodage CDC, convention MQTT collective | CDC complété, diagrammes SysML | J1 - Validation CDC |
| **Phase 2 : Recherche d'idées** | 5h | Créativité, benchmark, choix solution | Concept validé, planning Gantt, répartition tâches | J2 - Validation concept |
| **Phase 3 : Conception détaillée** | 8h | CAO, schémas, simulations, dimensionnement | Dossier conception, maquettes numériques, liste composants | J3 - Validation conception |
| **Phase 4 : Prototypage** | 14h | Fabrication, assemblage, programmation, câblage | Prototype fonctionnel, protocole de tests | J4 - Proto fonctionnel |
| **Phase 5 : Tests et validation** | 4h | Mesures, tests intégration MQTT, analyse écarts | Bilan technique, performances mesurées, propositions amélioration | J5 - Validation performances |
| **Phase 6 : Restitution** | 2h | Préparation présentation orale, support numérique | Présentation (10 min) pour épreuve IT | J6 - Épreuve orale 20 min |

**Total** : 36 heures

---

## 9. Compétences STI2D évaluées (Référence programme IT)

**Les compétences en gras sont évaluées lors de l'épreuve orale de contrôle continu :**

- ✓ **Décoder le cahier des charges d'un produit, participer, si besoin, à sa modification**
- ✓ **Évaluer la compétitivité d'un produit d'un point de vue technique et économique**
- ✓ **Décrire une idée, un principe, une solution, un projet en utilisant des outils de représentation adaptés**
- ✓ S'impliquer dans une démarche de projet, menée en groupe
- ✓ **Identifier et justifier un problème technique à partir de l'analyse globale d'un produit (approche MEI)**
- ✓ **Planifier un projet (Gantt, chemin critique) en utilisant les outils adaptés et en prenant en compte les données technico-économiques**
- ✓ **Proposer des solutions à un problème technique identifié en participant à des démarches de créativité, choisir et justifier la solution retenue**
- ✓ Participer à une étude de design d'un produit dans une démarche de développement durable
- ✓ Définir la structure matérielle, la constitution d'un produit en fonction des caractéristiques technico-économiques et environnementales attendues
- ✓ **Réaliser et valider un prototype ou une maquette obtenus en réponse à tout ou partie du cahier des charges initial**

---

## 10. Espace collaboratif et documentation

**Outils collaboratifs à utiliser :**
- [ENT, Drive, Git, etc.]
- Dashboard MQTT : Node-RED sur Raspberry Pi central
- Logiciels de conception : [Fusion 360, SolidWorks, Papyrus SysML, etc.]

**Documents à produire et partager :**
- Dossier de conception (CAO, schémas, code)
- Protocole de tests et résultats
- Support de présentation pour l'épreuve orale
- Documentation technique (pour maintenance et évolution)

---

## Annexes

- Référence matériel labo : `contexte/materiel-labo.md`
- Conventions MQTT : `ressources/conventions-mqtt.md`
- Contexte Martinique : `contexte/martinique.md`
- Fiche de définition projet IT Eduscol (page 8-9 du document ressource)
