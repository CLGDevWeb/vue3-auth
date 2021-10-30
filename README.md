# :star2: VueJS 3 Auth avec Vuex & Vue Router

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
    ├── repositories                    # librairie (endpoint) fonctionnelle d'appels API
    ├── router                          # Vue-router: routes, historique, meta, etc ...
    ├── services
    │   └── authenticationService.js    # service d'authentification (réutilisable dans les composants)
    ├── store                           # Vuex: global state management
    │   ├── modules
    │   │    ├── posts.js
    │   │    └── ...
    │   └── index.js
    ├── App.vue
    ├── container.js
    ├── main.js
    └── .env
```
