# arene-des-algos-JasonDAHMOUN

## Choix de preprocessing

- Les trous cachés de `TotalCharges` sont remplacés par la médiane pour
  conserver les clients et limiter l'effet des valeurs extrêmes.
- `customerID` est supprimée : c'est un identifiant unique, pas une information
  utile pour prédire le churn. Son One-Hot créerait 7043 colonnes.
- `Contract` est encodée en One-Hot. Même si les contrats évoquent une durée,
  les coder 0, 1 et 2 imposerait une distance artificielle entre les catégories.
