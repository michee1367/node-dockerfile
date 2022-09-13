# Documentation
- step 1
```bash
    docker-compose up -d --build
```

- step 2 
```bash
    docker-compose exec front /bin/bash

```

- step 3
```bash
    git clone -b main --single-branch  https://github.com/PNDA-CD/sigi-webui.git .
```

- step 4
```bash

    yarn install

```

- step 5

```bash
    yarn nuxt
```

- step 6

```bash

    exit

```

- step 7

```
    Dans le dossier `app_front` créer un un fichier `.env`. Puis inserer les contenu suivant :

    `
        APP_ENV=dev
        END_POINT="http://localhost"
        #ROUTER_BASE=web
        KEYCLOAK_API_URL=https://keycloak.surintrants.com/
        KEYCLOAK_CLIENT_ID=webui-localhost

    `
```

- step 8

```
    docker-compose exec front yarn nuxt

```

- step 9

```
    Acceder à http://localhost:3000
```