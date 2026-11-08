# BMG 2.9 — Suppression des provisions ST

- Suppression de la colonne Provision HT et des montants de provision dans les détails ST.
- Les provisions historiques sont ignorées et retirées à la normalisation des sauvegardes JSON.
- Marché ST = marché engagé + OM + travaux à régulariser ; prorata et RAD net restent calculés sur cette base, sans provisions.
- Contrôles financiers et rapprochement ST testés via `npm test`.
