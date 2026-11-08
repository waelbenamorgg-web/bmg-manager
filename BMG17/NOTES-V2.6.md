# BMG 2.6 — RAD ST net, moins-values et avoirs

- Le RAD restant d'un sous-traitant est rapproché du **marché actualisé net de prorata**, moins les factures et avoirs ST enregistrés dans le Cahier d'épicier. Le montant saisi en facture ST doit être le montant HT net de retenue prorata pour que les bases soient comparables.
- Le marché actualisé comprend marché initial + OM (positifs ou négatifs) + régularisations (positives ou négatives). Les provisions sont présentées à part.
- Les factures négatives (avoirs) sont acceptées, ainsi que les corrections mensuelles négatives justifiées. Les virements budgétaires restent des montants positifs dirigés d'un code vers un autre.
- Le contrôle de rapprochement ST s'effectue en centimes entiers. Aucun rééquilibrage automatique du RAD mensuel.
- Les indicateurs et messages du tableau de bord présentent désormais la base **nette de prorata**.
- Les données de versions antérieures sont conservées. **Les RAD ST existants auparavant saisis en brut devront être revus manuellement** : l'application signale les écarts.
- Le contrôle n'est pas un rapprochement bancaire ni un calcul de TVA. Pour les situations cumulatives, ne saisir que la période réellement facturée (éviter de compter plusieurs fois un cumul).

## Vérification
`npm test` : 12 vérifications financières, 9 contrôles fonctionnels et scénarios supplémentaires ST (avoir négatif, OM négatif, 1 centime) exécutés avec succès. Compilation Vite et tests navigateurs non exécutés dans cet environnement.
