## Localhost

```sh
fnm install 16.20.0
fnm use 16.20.0
```

```sh
npm i
```

Edit near line `6` of `package.json`:

``` title="package.json"
  "homepage": "",
```

```sh
npm run build
```

```sh
serve -s build -l 4321
```
