# BMG 1.9 – Frais généraux et lisibilité RAD

- Dans Tableau de bord > Configuration, le taux de frais généraux (%) est modifiable de 0 à 100, avec deux décimales.
- Les indicateurs d’étude, réel et atterrissage, ainsi que les frais généraux et marges nettes mensuels du RAD, utilisent le taux du projet.
- La ligne « Facturation client totale HT (base + avenants + révision) » possède un fond vert foncé opaque et une écriture blanche contrastée, y compris dans les cellules mensuelles.
- Les valeurs sont conservées dans le JSON de chantier existant.

## Tests manuels conseillés

1. Passer le taux de 15 à 10 dans Configuration.
2. Vérifier le recalcul de la marge nette et des frais généraux dans Tableau de bord et RAD.
3. Exporter le JSON, le réimporter et vérifier la persistance du taux.
4. Vérifier la ligne de facturation totale en mode sombre et sur plusieurs mois.
