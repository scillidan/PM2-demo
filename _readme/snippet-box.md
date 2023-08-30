## Localhost

```sh
fnm install 16.20.0
fnm use 16.20.0
```

```sh
cd client
npm i
cd ..
```

Edit near line `30` of `package.json`:

``` title="package.json"
  "dependencies": {
    "babel-jest": "^26.6.0",
    "babel-loader": "8.1.0",
    "eslint": "^7.11.0",
    "jest": "26.6.0",
    "webpack": "4.44.2",
    "webpack-dev-server": "3.11.1",
```

```sh
npm i
```

```sh
npm run build
```

```sh
cd build
node server.js
```

Open `localhost:5000`