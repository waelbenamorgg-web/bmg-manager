# BMG 1.7 – Corrections RAD / avenants / PRORATA

- Facturation prévisionnelle mensuelle du marché de base : modifiable dans le RAD, même lorsque les paramètres du chantier sont verrouillés.
- Création d'un avenant dans Budget évolution : numéro, date, montant et affectations par codes, sans obligation d'affecter la totalité.
- Part non affectée = montant avenant - montants affectés. Il s'agit d'une enveloppe non affectée / marge brute potentielle, **pas** d'un bénéfice net acquis.
- Ventilation de la facturation de chaque avenant exclusivement dans le RAD, par mois. Le total prévisionnel du RAD additionne base, avenants et révision de prix du marché de base.
- Migration des avenants précédents : le mois de facturation existant est repris dans la ventilation mensuelle.
- Alertes si facturation mensuelle de base ou d'un avenant ne correspond pas au montant du marché correspondant.
- Suppression du code PRORATA possible dans Budget évolution, même s'il était verrouillé, après confirmation. Refus si des écritures externes (dépenses, avenants, transferts) y font référence. Supprime aussi la ventilation détaillée. Le code peut être recréé avec le bouton Rétablir le code PRORATA.
- L'export JSON reste indispensable à la sauvegarde portable.

## Validation
- 12 tests financiers existants exécutés avec succès.
- Vérifications structurelles des nouveaux chemins de code réalisées.
- Compilation Vite et tests navigateur non exécutés dans cet environnement, faute de dépendances npm disponibles hors ligne.

## Tester sur Windows
```powershell
npm.cmd install
npm.cmd run build
npm.cmd run dev
```
Tester sur une **copie** des données JSON : un avenant de 1000 € dont 500 € affectés à MXBE, puis 400 € facturés un mois et 600 € un autre ; vérifier le total, la marge, la suppression du prorata et la restauration après import/export.
