# Projet WP-BTS-E-Learning

Ce projet utilise Git pour la gestion de versions. Si vous rencontrez des problèmes lors de l'ajout et de la mise à jour de fichiers, veuillez suivre ces étapes pour résoudre les conflits.

## Résolution des conflits

Si vous rencontrez des problèmes lors de la mise à jour du dépôt distant, suivez ces étapes :

1. Assurez-vous d'être sur la branche `main` avec la commande :
   ```bash
   git branch
   ```
   Si vous n'êtes pas sur la branche `main`, basculez avec :
   ```bash
   git checkout main
   ```

2. Récupérez les dernières modifications du dépôt distant :
   ```bash
   git pull origin main
   ```
   Si vous obtenez une erreur "fatal: refusing to merge unrelated histories", essayez cette commande :
   ```bash
   git pull origin main --allow-unrelated-histories
   ```

3. Si des conflits surviennent, résolvez-les dans vos fichiers locaux.

4. Ajoutez et commitez les changements :
   ```bash
   git add .
   git commit -m "message"
   ```

5. Poussez les modifications vers le dépôt distant :
   ```bash
   git push origin main
   ```

Si ces étapes ne fonctionnent pas, envisagez de cloner à nouveau le dépôt et de déplacer vos fichiers modifiés.
