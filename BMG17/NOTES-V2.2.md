# BMG 2.2 — Rapprochement réel / RAD des sous-traitants

- Les factures du Cahier d’épicier sont comptabilisées en réel, sans modifier automatiquement les RAD.
- Lors de la saisie d’une facture imputée à un code ST, sélection obligatoire du marché ST exact.
- Pour chaque ST : marché actualisé = initial + OM signés (+/-) + travaux à régulariser (+/-) + provision prévisionnelle ; facturé réel = factures imputées au ST ; reste à facturer prévisionnel = marché actualisé - facturé réel.
- Somme des RAD mensuels restants = reste à facturer prévisionnel, contrôle strict en centimes. Écart de 0,01 € = anomalie.
- Les mois du RAD ST restent modifiables uniquement manuellement dans ST.
- Centre de contrôle et alertes du Tableau de bord indiquent le sous-traitant, les sommes et l'écart.
- Les anciens fichiers JSON sont acceptés ; les factures ST historiques sans stId sont rapprochées par code seulement si ce code correspond à un unique sous-traitant. Sinon, une alerte demande d'affecter le marché exact.
- Prorata ST conservé à part : aucune déduction automatique du prorata dans les factures ni dans le RAD.

Attention : la provision reste incluse dans le total de marché prévisionnel, conformément à la logique historique de BMG. Elle n'est pas une facture validée.

Tests : npm test. Compilation : npm install puis npm run build.
