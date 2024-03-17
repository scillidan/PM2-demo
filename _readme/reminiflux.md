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

1. Open Miniflux, liked `localhost:8070`.
2. Settings → API Keys → Create a new API key → `reminiflux` → Copy the Token
3. Open `localhost:4321`:

```sh
Host `http://127.0.0.1:8070`
API key `The Token`
```

## PM2

```sh
pm2 serve build 4321 --name reminiflux --spa
```