# TP Hello Web

## Configuration de Node.js

Pour exécuter du code JavaScript, un environnement d'exécution est nécessaire. Node.js est l'un des environnements d'exécution les plus populaires pour le JavaScript.

### Installation de Node.js

Installez la version 20 (LTS - Long Term Support) de Node.js.

**Installation simplifiée**

Consultez la documentation en ligne sur https://nodejs.org/en/download/ et suivez les instructions d'installation.

**Installation avancée pour Mac/Windows avec WSL**

Consultez https://github.com/nvm-sh/nvm#install--update-script pour obtenir des instructions sur l'utilisation de NVM (Node Version Manager) pour installer Node.js.

### Vérification de l'installation de Node.js

Ouvrez un terminal et saisissez la commande `node -v` pour vérifier que Node.js est correctement installé.

Créez un fichier nommé `hello.js` contenant le code suivant :

```javascript
console.log("Hello les mines");
```

Exécutez ce fichier avec la commande `node hello.js`. Assurez-vous que le message "Hello les mines" s'affiche, confirmant ainsi que Node.js est correctement installé.

## Création d'un projet avec SolidJS

Pour créer un projet utilisant SolidJS, nous utiliserons `npm`, le gestionnaire de paquets fourni avec Node.js.

### Initialisation du projet

Dans le répertoire de votre choix, exécutez la commande suivante pour créer votre projet :

```bash
npx degit solidjs/templates/js-tailwindcss tp-hello
```

Cette commande crée un dossier `tp-hello` contenant un squelette de projet SolidJS.

Pour ouvrir ce dossier :

- Utilisez la commande `cd tp-hello` dans le terminal,
- Puis ouvrez-le avec VSCode en utilisant `code .` (Si cela ne fonctionne pas, ouvrez manuellement VSCode et naviguez jusqu'au dossier `tp-hello`).

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

Votre navigateur devrait se rafraîchir automatiquement et afficher le nouveau message.

### Utilisation de Git et GitHub

Créez un dépôt sur GitHub et téléversez-y votre projet.

1. Allez sur https://github.com/new pour créer un nouveau dépôt public sans utiliser de template.
2. Nommez-le, par exemple, `hello-solid`.
3. Dans le répertoire du projet `tp-hello`, exécutez les commandes suivantes :

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:<username>/hello-solid.git
git push -u origin main
```

Remplacez `<username>` par votre nom d'utilisateur GitHub. Vérifiez ensuite que le projet a bien été poussé sur GitHub.

## Publication sur le Web avec Vercel

Utilisez le service Vercel pour publier votre projet en ligne.

Créez un compte sur https://vercel.com en utilisant vos identifiants GitHub, puis suivez les instructions pour déployer votre projet.

### Pour continuer

- Partagez le lien de votre projet Vercel sur Slack.
- Modifiez le texte du projet pour le rendre plus original, puis faites un commit et poussez les modifications sur GitHub. Vérifiez que le projet se met à jour automatiquement sur Vercel.
