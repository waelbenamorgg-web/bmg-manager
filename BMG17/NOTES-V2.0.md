# BMG 2.0 — Prorata sous-traitants

- Colonne **Prorata ST** avec taux modifiable par sous-traitant, initialisé à 2 %.
- Retenue HT = (marché ST initial + ordres modificatifs + travaux à régulariser) × taux / 100.
- Les provisions sont exclues de la base tant qu’elles ne sont pas transformées en OM ou travaux à régulariser.
- Colonne **Net après prorata** = base contractuelle - retenue.
- Le marché brut et son RAD ne sont pas diminués automatiquement : la retenue correspond à un mouvement de règlement et non à une réduction du coût de travaux ; éviter tout double comptage avec le compte prorata de chantier.
- Import JSON ancien : 2 % par défaut pour les sous-traitants sans taux enregistré.
- Taux propre à chaque sous-traitant, sauvegardé avec le projet.
- Contrôler les conditions contractuelles avant d’appliquer effectivement une retenue.
