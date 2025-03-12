# cvwonder-theme-zatsit

cvwonder-theme-zatsit regroupe l'ensemble des thèmes Zatsit destinés à la génération de CV aux formats HTML ou PDF via [cvwonder](https://github.com/germainlefebvre4/cvwonder).

## Comment lancer en local cvwonder avec le theme zatsit?

1. **Télécharger cvwonder** : Télécharger le fichier éxécutable correspondant à votre systeme d'exploitation [ici](https://github.com/germainlefebvre4/cvwonder/releases).

2. **Créer un repertoire et déplacer l'éxécutable dans ce repertoire**.
   Si vous etes sur linux lancer la commande suivante pour rendre le binaire executabe.

   ```sh
   chmod +x cvwonder_linux_amd64
   ```

3. **Installer le theme zatsit**: pour ajouter le theme zatsit, lancer la commande suivant.

   ```sh
   ./cvwonder_linux_amd64 theme install https://github.com/zatsit-oss/cvwonder-theme-zatsit
   ```

4. **Préparer le fichier YAML** : Créer à la racine un fichier `cv.yaml` avec vos informations personnelles, expériences, projets, etc.
   Vous pouvez trouver plusieurs exemple [ici](https://github.com/zatsit-oss/zats-cv-generator)

5. **Générer le CV** : Utilisez l'outil `cvwonder_linux_amd64` pour générer le CV en HTML/PDF.

   ```sh
   ./cvwonder_linux_amd64 generate --input=cv.yml --output=generated/ --theme=default --format=pdf
   ```

6. **Visualiser le CV** : Pour visualiser en live le rendu de votre CV, taper la ligne de commande suivante à la racine du projet.

   ```bash
   ./cvwonder_linux_amd64 serve --input=cv.yaml --theme=default --watch
   ```

## Developpement

1. **Télécharger cvwonder** : Télécharger le fichier éxécutable correspondant à votre systeme d'exploitation [ici](https://github.com/germainlefebvre4/cvwonder/releases).

2. **Créer un repertoire et déplacer l'éxécutable dans ce repertoire**.
   Si vous etes sur linux lancer la commande suivante pour rendre le binaire executabe.

   ```sh
   chmod +x cvwonder_linux_amd64
   ```

3. **Cloner le theme zatsit**:

   ```sh
   git clone git@github.com:zatsit-oss/cvwonder-theme-zatsit.git
   ```

4. **Préparer le fichier YAML** : Créer à la racine un fichier `cv.yaml` avec vos informations personnelles, expériences, projets, etc.
   Vous pouvez trouver plusieurs exemple [ici](https://github.com/zatsit-oss/zats-cv-generator)

5. **Générer le CV** : Utilisez l'outil `cvwonder_linux_amd64` pour générer le CV en HTML/PDF.

   ```sh
   ./cvwonder_linux_amd64 generate --input=cv.yml --output=generated/ --theme=default --format=pdf
   ```

6. **Visualiser le CV** : Pour visualiser en live le rendu de votre CV, taper la ligne de commande suivante à la racine du projet.

   ```bash
   ./cvwonder_linux_amd64 serve --input=cv.yaml --theme=default --watch
   ```
