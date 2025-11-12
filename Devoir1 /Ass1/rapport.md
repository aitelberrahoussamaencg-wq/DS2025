# AIT ELBERRAH OUSSAMA
<img width="320" height="426" alt="image" src="https://github.com/user-attachments/assets/b1b3ae71-7234-498b-a040-e4635c84c2c1" />
<img width="1276" height="1178" alt="image" src="https://github.com/user-attachments/assets/920a308c-00af-4864-9e4a-4f22a4a5275e" />
<img width="1590" height="1506" alt="image" src="https://github.com/user-attachments/assets/1a146809-664d-4d04-9f37-4707a9a792f0" />




## Vue d'ensemble du Dataset

**Source :** UCI Machine Learning Repository  
**Identifiant :** Dataset #360  
**Date de donation :** 22 mars 2016  
**Créateur :** Saverio Vito  
**Licence :** Creative Commons Attribution 4.0 International (CC BY 4.0)  
**DOI :** https://doi.org/10.24432/C59K5F

---

## Thème et Objectif

Ce jeu de données concerne la **surveillance de la qualité de l'air** dans un environnement urbain fortement pollué. Il contient les réponses d'un dispositif multicapteur chimique déployé sur le terrain dans une ville italienne, au niveau de la route, dans une zone significativement polluée.

Le dataset a été conçu pour permettre l'étude et la **calibration de capteurs chimiques électroniques** (nez électronique) pour l'estimation des concentrations de polluants atmosphériques en conditions réelles d'utilisation.

---

## Description

### Contexte et Collecte des Données

Le dispositif de mesure a été déployé **sur le terrain** pendant une période d'un an complet, de **mars 2004 à février 2005**, représentant ainsi le plus long enregistrement librement disponible de réponses de capteurs chimiques de qualité de l'air déployés en conditions réelles.

Le système était composé d'une **matrice de 5 capteurs chimiques à oxydes métalliques** intégrés dans un dispositif multicapteur chimique pour la qualité de l'air. Ces capteurs étaient positionnés à proximité immédiate d'un analyseur certifié de référence qui fournissait les concentrations réelles (ground truth) des différents polluants.

### Caractéristiques Techniques du Dataset

**Type de données :**
- Multivarié
- Séries temporelles

**Domaine d'application :**
- Informatique / Computer Science
- Science environnementale
- Chimie analytique

**Tâche associée :**
- Régression (prédiction de concentrations de polluants)

**Dimensions :**
- **Nombre d'instances :** 9 358 enregistrements horaires
- **Nombre de variables :** 15 caractéristiques
- **Type de variables :** Réelles, entières, catégorielles, temporelles
- **Valeurs manquantes :** Oui (identifiées par la valeur -200)

### Variables du Dataset

Le dataset comprend 15 variables divisées en plusieurs catégories :

#### 1. Variables Temporelles
- **Date** (DD/MM/YYYY) : Date de l'enregistrement
- **Time** (HH.MM.SS) : Heure de l'enregistrement

#### 2. Concentrations Réelles (Ground Truth)
Mesurées par un analyseur certifié de référence :
- **CO(GT)** : Concentration horaire moyenne de monoxyde de carbone (mg/m³)
- **NMHC(GT)** : Concentration horaire moyenne d'hydrocarbures non méthaniques totaux (µg/m³)
- **C6H6(GT)** : Concentration horaire moyenne de benzène (µg/m³)
- **NOx(GT)** : Concentration horaire moyenne d'oxydes d'azote (ppb)
- **NO2(GT)** : Concentration horaire moyenne de dioxyde d'azote (µg/m³)

#### 3. Réponses des Capteurs
Réponses horaires moyennes des 5 capteurs à oxydes métalliques :
- **PT08.S1(CO)** : Capteur à oxyde d'étain, ciblant nominalement le CO
- **PT08.S2(NMHC)** : Capteur au dioxyde de titane, ciblant nominalement les NMHC
- **PT08.S3(NOx)** : Capteur à oxyde de tungstène, ciblant nominalement les NOx
- **PT08.S4(NO2)** : Capteur à oxyde de tungstène, ciblant nominalement le NO2
- **PT08.S5(O3)** : Capteur à oxyde d'indium, ciblant nominalement l'ozone O3

#### 4. Variables Environnementales
- **Temperature** : Température en degrés Celsius (°C)
- **Relative Humidity** : Humidité relative (%)
- **Absolute Humidity** : Humidité absolue

### Défis et Particularités

Le dataset présente plusieurs caractéristiques importantes pour la recherche :

1. **Sensibilités croisées** : Les capteurs présentent des réponses croisées, c'est-à-dire qu'un capteur ciblant un polluant spécifique peut également réagir à d'autres composés chimiques présents dans l'air.

2. **Dérives des capteurs** : Le dataset présente des évidences de deux types de dérives :
   - **Dérive conceptuelle** : Changement des relations entre les entrées et les sorties au fil du temps
   - **Dérive des capteurs** : Dégradation progressive des performances des capteurs physiques

3. **Valeurs manquantes** : Les données manquantes sont identifiées par la valeur conventionnelle **-200**, facilitant ainsi leur détection et leur traitement.

Ces caractéristiques reflètent les conditions réelles d'utilisation et constituent des défis authentiques pour le développement d'algorithmes robustes de calibration et d'estimation.

---

## 🔬 Applications et Utilisations

### Applications Principales

1. **Calibration de capteurs chimiques** : Développement de modèles de calibration pour améliorer la précision des estimations de concentrations à partir des réponses des capteurs.

2. **Estimation de polluants** : Prédiction des concentrations de différents polluants atmosphériques (CO, benzène, NOx, NO2, NMHC).

3. **Détection d'anomalies** : Identification de conditions atmosphériques inhabituelles ou de dysfonctionnements des capteurs.

4. **Analyse de séries temporelles** : Étude des patterns temporels de pollution urbaine et de leurs corrélations avec des variables environnementales.

5. **Gestion des dérives** : Développement de techniques pour compenser les dérives conceptuelles et instrumentales dans les systèmes de capteurs à long terme.

### Domaines de Recherche

- Machine Learning et régression
- Traitement du signal
- Chimie analytique
- Sciences environnementales
- Internet des Objets (IoT) pour la surveillance environnementale
- Systèmes de capteurs intelligents

---

## Références Scientifiques

### Publication Introductive

**Titre :** "On field calibration of an electronic nose for benzene estimation in an urban pollution monitoring scenario"

**Auteurs :** S. De Vito, E. Massera, M. Piga, L. Martinotto, G. Di Francia

**Journal :** Sensors and Actuators B: Chemical, Vol. 129, Issue 2, 2008

**Lien :** [Article sur Semantic Scholar](https://www.semanticscholar.org/paper/a90a54a39ff934772df57771a0012981f355949d)

Cette publication décrit en détail la méthodologie de calibration sur le terrain du nez électronique et les défis associés aux sensibilités croisées et aux dérives des capteurs.

### Autres Publications Utilisant ce Dataset

1. **"Boosting for Dynamical Systems"**  
   Agarwal et al., 2019, ArXiv

2. **"Zoom-SVD: Fast and Memory Efficient Method for Extracting Key Patterns in an Arbitrary Time Range"**  
   Jang et al., 2018, CIKM '18

3. **"Combined modeling of sparse and dense noise for improvement of Relevance Vector Machine"**  
   Sundin et al., 2015

---

## Accès et Téléchargement

### Fichiers Disponibles

- **AirQualityUCI.csv** : 766.7 KB (format CSV standard)
- **AirQualityUCI.xlsx** : 1.2 MB (format Excel)
- **Archive complète** : 1.5 MB (format ZIP)

### Installation via Python

```python
# Installation du package
pip install ucimlrepo

# Chargement du dataset
from ucimlrepo import fetch_ucirepo

# Récupération du dataset
air_quality = fetch_ucirepo(id=360)

# Extraction des données (pandas DataFrames)
X = air_quality.data.features  # Variables explicatives
y = air_quality.data.targets   # Variables cibles

# Affichage des métadonnées
print(air_quality.metadata)

# Affichage des informations sur les variables
print(air_quality.variables)
```

### Documentation Complète

[Guide d'utilisation du package ucimlrepo](https://github.com/uci-ml-repo/ucimlrepo)

---

## ⚖️ Conditions d'Utilisation

### Licence

Ce dataset est distribué sous licence **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

Cette licence permet :
- ✅ Le partage et la redistribution du dataset
- ✅ L'adaptation et la transformation des données
- ✅ L'utilisation à des fins commerciales ou non commerciales

**Conditions :**
- Attribution appropriée des créateurs originaux
- Indication des modifications apportées
- Pas de restrictions supplémentaires

### Restrictions

⚠️ **Usage exclusivement à des fins de recherche**. Les utilisations commerciales directes du dataset sont explicitement exclues selon les termes originaux de donation.

### Citation Recommandée

```
Vito, S. (2008). Air Quality [Dataset]. 
UCI Machine Learning Repository. 
https://doi.org/10.24432/C59K5F
```

---

## 🎓 Intérêt Pédagogique et Scientifique

Ce dataset présente un intérêt majeur pour :

### Étudiants et Chercheurs
- Apprentissage des techniques de traitement de séries temporelles
- Étude de cas réel de régression multivariée
- Gestion de données manquantes et de valeurs aberrantes
- Analyse de la qualité des données issues de capteurs physiques

### Développeurs et Ingénieurs
- Développement d'algorithmes de calibration de capteurs
- Création de systèmes de surveillance environnementale
- Mise en œuvre de techniques de compensation de dérive
- Validation de modèles prédictifs en conditions réelles

### Scientifiques Environnementaux
- Analyse de patterns de pollution urbaine
- Étude des corrélations entre différents polluants
- Compréhension de l'impact des conditions météorologiques sur la qualité de l'air

---

## Conclusion

Le dataset **Air Quality UCI** constitue une ressource précieuse et unique pour la communauté scientifique, offrant un an complet de données réelles de qualité de l'air collectées en environnement urbain pollué. Sa richesse provient non seulement de sa taille et de sa durée, mais aussi de la présence simultanée de mesures de référence certifiées et de réponses de capteurs chimiques, permettant ainsi le développement et la validation de modèles de calibration robustes.

Les défis inhérents à ce dataset (sensibilités croisées, dérives, valeurs manquantes) en font un excellent terrain d'expérimentation pour des algorithmes avancés de machine learning et de traitement du signal, reflétant fidèlement les contraintes réelles des systèmes de surveillance environnementale déployés sur le terrain.

---

*Document créé le 12 novembre 2025*  
*Source : UCI Machine Learning Repository*
