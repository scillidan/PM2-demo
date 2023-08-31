## Localhost

```sh
npm i
```

Edit near line `23` of `package.json`:

```json title="package.json"
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -b master -d build",
    "start": "react-scripts start",
    "build": "set GENERATE_SOURCEMAP=false && react-scripts build",
```

```sh
npm run build
```

```sh
serve -s build -p 4321
```
