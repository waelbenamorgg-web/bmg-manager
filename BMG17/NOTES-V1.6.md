# BMG 1.6 — accès et sauvegarde locale

- Choix explicite Utilisateur / Administrateur à la connexion. Le mode Administrateur ouvre directement le formulaire de changement du mot de passe utilisateur.
- Mot de passe utilisateur enregistré dans le localStorage du navigateur concerné.
- Export JSON via Blob, date dans le nom du fichier, bouton de sauvegarde visible et indicateur de modifications depuis le dernier export.
- Alerte native du navigateur avant fermeture/rechargement quand une sauvegarde JSON est à effectuer. Le texte de cette alerte dépend du navigateur et peut ne pas apparaître dans certaines circonstances.
- Import JSON pour restaurer une sauvegarde sur l'ordinateur d'un conducteur de travaux.
- Attention : un mot de passe côté navigateur n'est pas une protection contre un utilisateur technique ayant accès au code. Ne pas publier de données sensibles sur un site public.
