# Modèle de configuration de Webpack pour WordPress

## Réutilisation
1. Cloner le repo `git clone git@github.com:Claire-Lavigne/Webpack-Pattern-Claire.git`
2. Renommer le dossier cloné `mv Webpack-Pattern-Claire <nomduprojet>`
3. Se rendre dans le dossier `cd <nomduprojet>` et l'ouvrir dans vscode `code .`
4. Supprimer le dossier `.git` afin de repartir d'un repo tout neuf `sudo rm -R .git`
5. Initialisation d'un git tout beau tout neuf `git init`
6. Premier versionning de notre repo:
  - `git add .`
  - `git commit -m "First Commit"`
  - `git remote add origin git@github.com:Claire-Lavigne/Webpack-Pattern-Claire.git`
  - `git push -u origin master`

## Installation

1. Exécuter dans le répertoire la commande `npm install` qui va installer toute les dépendances Node.js nécessaire au bon fonctionnement de l'application.
2. Exécuter une des commandes ci-dessous.

## Commandes disponibles

- `npm run start` : Démarre le serveur de développement en utilisant [Browsersync](https://www.browsersync.io/). Ne s'ouvre plus automatiquement, il faut cliquer sur le lien local dans le terminal
- `npm run build:dev` : Génère les ressources front sans compression en vue d'une utilisation dans un environnement de développement
- `npm run build:prod` : Génère les ressources front avec compression (minify, uglify) en vue d'une utilisation dans un environnement de production
- `npm run clean` : Supprime les fichiers générés par Webpack
- `npm run clean:all` : Supprime les fichiers générés par Webpack ainsi que le répertoire des dépendances installées avec NPM (`node_modules`)
- `sudo npm install -g npm` : Actualiser Npm

## Options
- dépendances (npmjs) : reset-css/normalize, bootstrap, jQuery Scrollex
  - `npm i reset-css normalize bootstrap jquery.scrollex`
- main.scss : importer bootstrap, reset/normalize et fichiers
- base.scss : importer google fonts et variables
  - * --> box-sizing: border-box; (si pas dans reset)
  - body --> font-family: $font-family, $font-family-fallback;
