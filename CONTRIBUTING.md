# Comment contribuer

## Les branches

- `main` : version stable, protégée. On n'y travaille jamais directement.
- `dev` : branche d'intégration, protégée. Tout passe par une pull request.
- `feature/<code tâche>-<nom>` : une branche par tâche du tableau de suivi, par exemple `feature/T14-base-de-donnees`.

## Marche à suivre pour une tâche

1. Récupérer la dernière version de dev :

       git checkout dev
       git pull

2. Créer sa branche à partir de dev :

       git checkout -b feature/T14-base-de-donnees

3. Travailler, puis enregistrer régulièrement :

       git add .
       git commit -m "T14 : création des tables utilisateur et contenu"
       git push -u origin feature/T14-base-de-donnees

4. Sur GitHub, ouvrir une pull request vers `dev` et demander une relecture à une autre membre.
5. Une fois la PR approuvée, la fusionner puis supprimer la branche.

## Règles

- Chaque message de commit commence par le code de la tâche (T14, T07...).
- Une PR doit être relue et approuvée par une autre membre avant fusion.
- Penser à mettre à jour le tableau de suivi et la feuille de temps.
