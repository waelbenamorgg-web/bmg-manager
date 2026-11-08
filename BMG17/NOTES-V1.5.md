# BMG 1.5 – Corrections

- Budget évolution : choix de l'unité par code (forfait, u, m, m², m³, kg, t, h, jour, mois, ml).
- Passage en forfait : la quantité passe à 1 et le montant total antérieur est conservé dans le champ « PU / Montant HT ».
- Pour un code en forfait, la quantité est bloquée à 1 et le champ « PU / Montant HT » sert à saisir directement le montant global.
- Accès : bouton Afficher/Masquer sur le mot de passe à la connexion et dans l'administration.
- Administration : bouton de changement du mot de passe utilisateur rendu plus visible après connexion avec le compte administrateur.

## Limite de sécurité majeure
L'authentification actuelle est uniquement une interface locale. Les secrets restent dans le code client et le changement de mot de passe est enregistré uniquement dans localStorage sur le navigateur utilisé. **Cela ne sécurise pas un déploiement public et ne modifie pas le mot de passe sur les autres appareils.** Pour un accès réel, utiliser un service d'authentification côté serveur.

## Vérifications à effectuer sur Windows

```powershell
npm.cmd install
npm.cmd run build
npm.cmd run dev
```

Vérifier le code MXFE, le passage kg → forfait, le maintien du total, la modification du montant, le retour vers une unité, l'ouverture de l'administration et l'affichage/masquage des mots de passe.
