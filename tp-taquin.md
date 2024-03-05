# TP Taquin

# Setup

On s'assure d'avoir une version de node qui marche 

```bash
$ node -v
v20.11.0
```


Si on a pas cela, 

```bash
nvm use 20.11.0
```

Sinon on regarde le précédent TP.

## Création d'un projet avec SolidJS et Tailwind

Pour créer un projet utilisant SolidJS, nous utiliserons `npm`, le gestionnaire de paquets fourni avec Node.js.

### Initialisation du projet

Dans le répertoire de votre choix, exécutez la commande suivante pour créer votre projet :

```bash
npx degit solidjs/templates/js-tailwindcss tp-taquin
```

Cette commande crée un dossier `tp-taquin` contenant un squelette de projet SolidJS.

Pour ouvrir ce dossier :

- Utilisez la commande `cd tp-hello` dans le terminal,
- Puis ouvrez-le avec VSCode en utilisant `code .` (Si cela ne fonctionne pas, ouvrez manuellement VSCode et naviguez jusqu'au dossier `tp-taquin`).

### Installation des dépendances

Installez les dépendances du projet avec :

```bash
npm install
```

Lancez le projet avec :

```bash
npm run dev
```

Le projet sera accessible à l'adresse `http://localhost:3000`. Ouvrez cette adresse dans votre navigateur pour voir le projet.

### Modification du projet

Ouvrez le fichier `src/App.js` et remplacez le texte `Hello World` par `Hello les mines` (ou tout autre message de votre choix).

On supprime le fichier `pnpm.lock` qui peut géner.


Votre navigateur devrait se rafraîchir automatiquement et afficher le nouveau message.

On vérifie que tailwind fonctionne.

### (optionnel) Utilisation de Git et GitHub

Créez un dépôt sur GitHub et téléversez-y votre projet.

1. Allez sur https://github.com/new pour créer un nouveau dépôt public sans utiliser de template.
2. Nommez-le, par exemple, `hello-solid`.
3. Dans le répertoire du projet `tp-taquin`, exécutez les commandes suivantes :

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:<username>/tp-taquin.git
git push -u origin main
```

Remplacez `<username>` par votre nom d'utilisateur GitHub. Vérifiez ensuite que le projet a bien été poussé sur GitHub.


## On commence !

Exemple de taquin 4x4:
![taquin.png](taquin.png)

On implémente le visuel d'un taquin.
