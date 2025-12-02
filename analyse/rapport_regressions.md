# 📊 Compte rendu d'analyse : Régression linéaire & Régression logistique
## École Nationale de Commerce et de Gestion (ENCG) - 4ème Année
<img src="Screenshot_2024306-2024_WhatsApp (1).jpeg" style="height:464px;margin-right:432px"/>







# Nabila ABLAD

## 1️⃣ Introduction

L'objectif de cette analyse est d'étudier l'effet de la variable
**Hours_Studied (heures d'étude)** sur deux résultats différents :

1.  **Score obtenu** → Analyse via **régression linéaire**
2.  **Probabilité de compléter le cours (Completed)** → Analyse via
    **régression logistique**

Les deux visualisations examinées permettent d'évaluer la force et la
direction des relations entre ces variables.

------------------------------------------------------------------------

# 2️⃣ Régression linéaire : *Score \~ Hours_Studied*

## 🔍 Observation du graphique

Le nuage de points montre une forte dispersion des scores,
indépendamment du nombre d'heures étudiées. La droite de régression
présente :

-   **Une pente légèrement négative**
-   **Une relation très faible entre les deux variables**
-   Une répartition aléatoire des points autour de la droite

## 🧠 Interprétation

-   Il n'existe **pas de relation linéaire significative** entre le
    nombre d'heures d'étude et le score obtenu.
-   La pente négative indique un effet inverse **mais probablement non
    significatif**, suggérant qu'un modèle linéaire n'est pas adapté
    pour prédire le score dans ce cas.
-   La variance élevée du score suggère l'influence d'autres facteurs
    (compétence préalable, difficulté du cours, motivation, etc.).

------------------------------------------------------------------------

# 3️⃣ Régression logistique : *Completed \~ Hours_Studied + Age*

## 🔍 Observation du graphique

Le second graphique présente :

-   Les **labels réels** (0 = non complété, 1 = complété)
-   Les **probabilités prédites** par le modèle (croix orange)
-   La **courbe logistique** en fonction des heures d'étude\
    (l'âge est fixé à sa médiane pour simplifier la visualisation)

La courbe a une **légère pente négative**, ce qui signifie que, dans ce
modèle :

-   L'augmentation des heures d'étude **ne semble pas augmenter la
    probabilité de compléter le cours**
-   Le lien entre les deux variables est faible

## 🧠 Interprétation

-   Le modèle logistique montre que **Hours_Studied seul n'est pas un
    bon prédicteur** du statut "Completed".
-   Les points réels (0 ou 1) sont largement dispersés → signe d'un lien
    faible entre heures d'étude et achèvement du cours.
-   Les probabilités estimées sont proches les unes des autres (≈
    0.4--0.55), montrant une **faible confiance du modèle** dans sa
    capacité prédictive.

------------------------------------------------------------------------

# 4️⃣ Conclusion générale

-   Les deux modèles (linéaire et logistique) montrent une **relation
    très faible** entre le temps d'étude et les résultats.

-   Le fait que la pente soit légèrement négative dans les deux analyses
    suggère une absence de corrélation plutôt qu'un véritable effet
    inverse.

-   Ces résultats indiquent que **les performances et la completion du
    cours dépendent probablement d'autres facteurs**, tels que :

    -   motivation,
    -   qualité du contenu,
    -   emploi du temps,
    -   compétence préalable,
    -   méthode d'apprentissage.

## ✔️ Recommandation

Pour obtenir des modèles prédictifs plus fiables, il serait utile
d'inclure davantage de variables explicatives et de réaliser un
**feature engineering plus approfondi**.
