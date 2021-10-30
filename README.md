# :star2: VueJS 3 Auth avec Vuex & Vue Router

## :loudspeaker: Description
Ce dépôt Github est un synthèse d'une de mes expériences professionnelles de projet Front-End avec :
```
- VueJS 3.2.2
- Vue-router 4.0.12
- Vuex 4.0
```
Cette synthèse s'addresse aux personnes souhaitant mettre en place une authentification, sur une application VueJS, un peu plus poussée que celle des tutoriels habituels. Sans prétention aucune, les critiques constructives sont encouragées :pray:

## :floppy_disk: Installation

Télécharger l'application & installation des dépendances

```
  git clone #####
  cd vue-auth
  npm install
```

Créer & configurer le fichier `.env` à la racine du projet

### Compiler le Javascript & le CSS
```
npm run serve
```

### Compiler pour la mise en production
```
npm run build
```

## :file_folder: Structure
```bash
├── public
└── src
    ├── assets                          # css, images, etc..
    ├── clients                         # préparation de nos appels axios (headers, token, baseURL, etc..)
    │   └── api.js
    ├── components
    │   ├── MyComponent.vue
    │   └── ...
    ├── interceptors/response           # capte les erreurs API (ex: erreur 401 => supprime le token)
    │   ├── failure.js                  
    │   └── success.js
    ├── layouts                         # layouts de l'appli (configuration dans le router & main.js)
    ├── repositories                    # fonctions pour les appels API
    ├── router                          # Vue-router: routes, historique, meta, etc ...
    │   ├── posts
    │   ├── ...
    │   └── index.js
    ├── services
    │   └── authenticationService.js    # service d'authentification (réutilisable dans les composants)
    ├── store                           # Vuex: global state management
    │   ├── modules
    │   │    ├── posts.js
    │   │    └── ...
    │   └── index.js
    ├── App.vue
    ├── container.js                    # librairie d'appels des repositories
    ├── main.js                         # racine de l'application
    └── .env                            # variables d'environnement
```

