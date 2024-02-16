# Le TP Hello Web

## Setup Node

Pour executer du code javascript nous avons besoin d'un environnement d'execution. Node.js est un des environnement d'execution de code javascript.

### Installer Node.js

Installer la version 20 (LTS = long term support)

**version simple**

Voir documentation en ligne : https://nodejs.org/en/download/ et suivre les instructions

**version avancée, mac/windows wsl**

https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating


### Vérifier que Node.js est bien installé

Ouvrir un terminal et taper la commande `node -v` pour vérifier que Node.js est bien installé.

Créer un fichier `hello.js` avec le code suivant :

```javascript
console.log("Hello les mines")
```

Exécuter le fichier avec la commande `node hello.js` et s'assurer qu'on voit bien le text "Hello les mines", pour vérifier que Node.js est bien installé.

## Créer un projet avec SolidJS

Pour créer un projet avec SolidJS, nous allons utiliser le gestionnaire de paquet `npm` qui est installé avec Node.js.

### Créer un projet

Placer vous dans le dossier ou vous voulez créer votre projet et taper la commande suivante :

```bash
npx degit solidjs/templates/js-tailwindcss tp-hello
```

Ceci a alors créé un dossier `tp-hello` avec un projet SolidJS.

On peut alors ouvrir le dossier

Avec shell :

```bash
cd tp-hello
```

Puis avec VSCode (si cela ne marche pas chez vous vous pouvez ouvrir VSCode et ouvrir le dossier `tp-hello`):

```bash
code .
```

### On install les dépendances

Pour installer les dépendances du projet, taper la commande suivante :

```bash
npm install
```

On peut alors lancer le projet avec la commande suivante :

```bash
npm run dev
```

Le projet est alors accessible à l'adresse `http://localhost:3000` (normalement)
On peut alors ouvrir un navigateur à cette adresse pour voir le projet.

### Modifier le projet

Ouvrir le fichier `src/App.js` et modifier le texte `Hello World` par `Hello les mines` (ou autre chose de plus original).

Le navigateur devrait alors se mettre à jour automatiquement pour afficher le nouveau texte.

![Magic](https://i.gifer.com/2Gb.gif)

### Git & github

On crée un repository sur github et on push le projet dessus.

1. https://github.com/new pour créer un nouveau repository public sans template.
2. On peut le nommer par exemple `hello-solid`
3. Ensuite, dans le projet `tp-hello` on fait les commandes suivantes :

```bash
git init
git add .
git commit -m "Initial commit"

# rempalcer <username> par votre nom d'utilisateur github
git remote add origin git@github.com:<username>/hello-solid.git
git push -u origin main
```

On vérifie que le projet est bien sur github.

## Il est temps de publier sur le web

On utilisera pour cela le service Vercel.

Créer un compte sur vercel.com en utilisant votre compte github.

Suivre les instructions pour publier le projet sur vercel.

Suite

* Partager le lien du projet publié sur vercel sur slack !
* Changer le texte du projet pour quelque chose de plus original / commit / push / vérifier que le projet est bien mis à jour sur vercel.
