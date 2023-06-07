# Vite, une nouvelle ère de tooling front ?

### Conférenciers: Christophe Jollivet & Yann-Thomas Le Moigne

## Time Line
- Début de Vite en Avril 2020 suite à un tweet
- V1 prête en Novembre 2020
- V2 en Février 2021
- Mars 2021 création de la première commu
  Aujourd'hui en V4

## Pourquoi Vite ?
Build de dev(ESBuild 2020) et de prod(Rollup --> Webpack) séparés.
Build séparé en node_modules et bundle.

## Demo
On peut créer un projet à partir d'un template (npm/yarn), on choisit le nom du projet, un framework (react, etc...) et une variante (TS, JS, etc...).
On installe les dépendances, on en a très peu, seulement ce qui est nécessaire.
Rechargement à chaud quand modification, seulement l'élément modifié (le h1 en loccurence) a été refresh. Le compteur n'a pas été reset lors de ce refresh.
Grâce à React, l'état n'est pas perdu lors d'un refresh contrairement à Vue.
Ajout d'un composant Header dans l'app mais l'état du compteur n'a toujours pas bougé.
Afin de passer du CSS au SCSS, il suffit de l'installer (cela est proposé automatiquement en console quand on change un import css vers scss)
Sur notre poste on peut aussi bien check l'env de prod que celui de dev.

## Avantages
- Documentation complète et bien faite
- Configuration accessible à  tous
- Système de plugins riche et puissant
- Confortable à l'usage pour le dev
- Safe pour la prod rollup

## Inconvénients
- Build de dev et prod différents (ESBuild/Rollup) attention aux différences de comportement potentielle
- Comportement différents selon les plugins et langages, peut être déroutant si on change de projet réguliérement

## Conclusion
Pas encore une nouvelle ère, même si pour les dépendances et le build tout est simplifié.
À tenter si déjà utilisateur de Vue ou React.

## Questions
Vite intégre une partie tests