# HackIA24 - Edge AI System for Smart Cities 
<br>18-19 mai 2024
<br>
<br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/b42a54a4-1f99-4fb1-ace2-ce26acee932c width="300">

## Groupe 2 (HackAI_2024_GRP_2)

**photo de groupe ici**

<br> *Data Expert* : Francesco Romeo :older_adult:
<br> *Operations Manager* : Loïc Reboursière :bearded_person:
<br> *Lead Developer* : Rabie Najem :bearded_person:
<br> *Designer* : Bérengère Fally :curly_haired_woman:

## Introduction

Ce projet met en œuvre et exploite les connaissances acquises en intelligence artificielle lors de la formation Hands on AI, pour développer des solutions concrètes adaptées aux villes intelligentes. 
Le projet se concentre sur le déploiement de modèles de Deep Learning pour des applications en temps réel sur des ressources Edge AI (Jetson Xavier de NVIDIA).
Pendant ces deux jours, nous avons travaillé en équipe pour développer, entraîner, et optimiser des réseaux de neurones profonds capables de traiter des séquences vidéo capturées en temps réel. Le but étant de créer des modules Edge AI efficaces pour la reconnaissance faciale et la détection d'objets, contribuant ainsi à la sécurité et à la gestion intelligente des infrastructures urbaines.
Ce document détaille les étapes du projet, allant de la conception initiale et l'entraînement des modèles, à leur portage sur des ressources Edge, jusqu'à l'optimisation et l'explicabilité des solutions développées. 

## Objectifs
- Développer des réseaux de neurones pour classifier des images, localiser des objets et reconnaître des visages.
- Intégrer les modèles dans un système Edge AI pour des vidéos capturées en temps réel.
- Optimiser la solution pour obtenir un bon compromis entre précision, temps de calcul et espace mémoire.

## Phases du Projet

### Phase 1 : Développement et entraînement des modèles

#### Objectifs
- Développer et entraîner des modèles de Deep Learning.
- Utiliser des ressources locales ou cloud (xxxxxx).

#### Base de données 
<br> Images BD1, BD2 + photos web (kaggle) => 1716 images

<br> fire : 572
<br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/8719ccff-25b9-4c4e-9011-ef67bf6fd899 width="300">

<br> no-fire : 572
<br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/c073b396-36a8-4960-a2f8-75bdd3bfa920 width="300">

<br> start-fire : 572
<br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/eba66914-97fd-4176-b102-ba76c7fe4fac width="300">

<br> Dataset final : https://drive.google.com/drive/folders/10FvmIW5iMZp31oEN0X9UfeA_-M2dyt7w?usp=sharing 
 
#### Face recognition
Modèle “Face”
<br> Authentification faciale grâce à la reconnaissance de visages.
<br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/d050359c-e63e-43a7-aee8-86329bdcf6bf width="300">
<br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/3b82591c-1b66-47d5-9f45-8b10a8453708 width="300">

#### Modèles développés
- **Modèle 1 : Classification de Feu**
  - **Architecture :** Description de l'architecture.
  - **Données utilisées :** Source et description des données.
  - **Résultats d'entraînement :** Précision, courbes de perte, etc.

- **Modèle 2 : Détection de feu et/ou objets (voitures, personnes, etc.)**
  - **Architecture :** Description de l'architecture.
  - **Données utilisées :** Source et description des données.
  - **Résultats d'entraînement :** Précision, courbes de perte, etc.

### Phase 2 : Portage sur ressource Edge
#### Configuration de l'environnement Edge
- **Ressources utilisées :** Jetson Xavier.
- **Installation des dépendances :** Liste des dépendances et instructions d'installation.

#### Déploiement des modèles
- **Procédure de déploiement :** Étapes suivies pour déployer les modèles.
- **Challenges rencontrés :** Description des problèmes et solutions trouvées.

### Phase 3 : Optimisation/compression et explicabilité des modèles
#### Optimisation des modèles
- **Pruning :** Description des techniques de pruning appliquées.
Réduire le poids pour rendre le modèle plus efficaces en termes de temps de calcul et d'utilisation de la mémoire, sans compromettre significativement leur précision. C'est déployer ces modèles sur des ressources limitées telles que les dispositifs Edge AI.
- **Quantization :** Description des techniques de quantization appliquées.
Diminuer la taille du modèle et accélérer les calculs sans sacrifier la précision du modèle. Cela permet d'améliorer les performances du modèle sur des appareils avec des capacités de calcul et de mémoire limitées, comme les Jetson Xavier, tout en maintenant une efficacité énergétique élevée.
- **Knowledge distillation :** Description des techniques de distillation des connaissances appliquées.
Transférer les connaissances d'un grand modèle complexe vers un modèle plus petit et plus simple. Permet de maintenir une haute précision tout en réduisant les besoins en calcul et en mémoire. Cela facilite le déploiement de solutions intelligentes sur le dispositif Edge AI, contribuant ainsi à l'optimisation et à l'efficacité des systèmes intelligents dans divers contextes.

<br> !!! tableaux comparaison
métriques des meilleures versions de modèles compressés

#### Explicabilité des modèles
- **Framework utilisé :** PyTorch.
- **Méthodes d'explicabilité :** Description des méthodes et résultats obtenus.

## Résultats et performance
### Évaluation de la performance
- **Précision :** Résultats de précision avant et après optimisation.
- **Temps d'inference :** Comparaison du temps d'inference avant et après optimisation.
- **Espace mémoire :** Comparaison de l'utilisation de la mémoire avant et après optimisation.

### Analyse des résultats
- **Compromis entre précision et performance :** Description des compromis.
- **Suggestions d'amélioration :** Idées pour améliorer le système.

## Conclusion
### Synthèse du projet
Synthèse des travaux réalisés, des défis relevés et des résultats obtenus.

## Environnements, outils utilisés, méthodologie et références utiles
- **Environnements :** Google Colab, Google Colab Pro.
  
- **Frameworks :** TensorFlow, PyTorch, Keras.
  
- **Outils de collaboration :** 
<br> Drive : https://drive.google.com/drive/folders/1pZg4WNNQ67gFMcpX1OwIWz55K1kt07ip?usp=sharing 
<br> Git : https://github.com/loicreboursiere/HackAI_2024_GRP_2 
<br> Slack : https://hackia-2024.slack.com/
<br> Telegram : https://t.me/HackIA24_bot

- **Méthodologie :**
 <br><img src=https://github.com/loicreboursiere/HackAI_2024_GRP_2/assets/170175731/68603fee-0ffe-43bf-abcb-dacb90adc44b width="300">


- **Références :** Liste des références


