# learn-math

## Project setup

```
yarn install
```

### Compiles and hot-reloads for development
```
yarn run serve
```

### Compiles and minifies for production
```
yarn run build
```

### Run your tests
```
yarn run test
```

### Lints and fixes files
```
yarn run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/)

### How this app was created

Vue CLI v3.1.1:

```
vue create learn-math
```

Added [eslint standard](https://github.com/standard/eslint-config-standard):

```
yarn add eslint-config-standard eslint-plugin-standard eslint-plugin-promise eslint-plugin-import eslint-plugin-node --dev
```

Replaced "eslint:recommended" with "standard" in package.json under eslintConfig.extends.

### How this app was Prepared for Heroku Deployment

```
yarn add express
```

Added minimal `server.js` and scripts in package.json:

```
"start": "node server.js",
"heroku-postbuild": "yarn build",
```

Set NODE_ENV:

```
heroku config:set NODE_ENV=production
```
