# BMG 2.1 — Centre de contrôle fonctionnel

- Remplacement du faux voyant « Virements OK » par un contrôle réel des transferts budgétaires.
- Tableau de bord : synthèse par onglet, détail des erreurs et bouton d’accès direct à l’onglet concerné.
- Contrôles : configuration, budget et avenants, transferts, ST et OM, RAD, facturation, cahier d’épicier, prorata, révision.
- Refus des nouveaux transferts négatifs, nuls, entre codes identiques, vers codes inconnus ou dépassant le budget source.
- Correction des coefficients de révision de prix : une part fixe/variable égale à zéro est désormais respectée.
- Détection du risque de double comptage entre dépenses engagées et RAD, sans changer silencieusement la méthode comptable.

## Limites importantes
Les contrôles identifient des anomalies de cohérence, mais ne certifient pas les comptes du chantier. Le modèle actuel additionne engagé + RAD : il faut confirmer que RAD est le reste à dépenser, sans dépenses déjà engagées. Le système ne connaît pas automatiquement les clauses contractuelles de révision et de prorata. Les données restent locales.
