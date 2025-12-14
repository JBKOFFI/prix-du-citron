# Analyse comparative des dynamiques du prix du citron : Abidjan vs Bouaké

**Auteurs :** Jean-Baptiste KOFFI et Prosper KOUASSI  
**Date :** 25 juillet 2025  

## Contexte
Le citron est un produit agricole clé en Côte d’Ivoire. Les prix varient selon les régions : Abidjan, marché économique central, et Bouaké, plus dépendante des productions locales. Cette étude compare les dynamiques de prix entre ces deux villes sur la période 2020-2022 et identifie des modèles de prévision fiables.

## Méthodologie
- **Analyse descriptive :** visualisation des tendances, dispersion et anomalies.  
- **Modélisation :** décompositions des séries (additive, multiplicative, STL), modèles ARIMA et SARIMA.  
- **Sélection des modèles :** basée sur RMSE, MAE et AIC.  

## Résultats
- **Tendances :**  
  - Abidjan : forte volatilité, effondrement des prix en 2020, rebond fin 2021.  
  - Bouaké : plus stable, prix élevés en 2020, chute modérée en 2021.  
- **Saisonnalité :** non significative.  
- **Décomposition multiplicative :** meilleure ajustement des données.  
- **Modèles ARIMA :**  
  - Abidjan : ARIMA(1,1,1) performant.  
  - Bouaké : Auto ARIMA(0,1,0) supérieur pour les prévisions.  
- **SARIMA :** non adapté en raison de l’absence de saisonnalité forte.  
- **Performance :** Bouaké → prévisions fiables (RMSE = 64, MAE = 27,3), Abidjan → prévisions moins précises (RMSE ≈ 488, MAE ≈ 425–450).  

## Conclusion
Les dynamiques de prix diffèrent fortement entre Abidjan et Bouaké. Les modèles multiplicatifs et ARIMA/Auto ARIMA sont les plus adaptés, mais la volatilité élevée d’Abidjan limite la précision des prévisions. La gestion des prix doit donc être contextualisée pour chaque marché.

## Source de données
[Data Côte d’Ivoire - Écho du marché](https://data.gouv.ci/datasets/echo-du-marche)
