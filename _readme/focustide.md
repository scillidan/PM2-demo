## Localhost

```sh
yarn install
```

```sh
yarn generate
```

```sh
serve dist -p 4321
```

## PM2

```sh
pm2 serve dist 4321 --name focustide --spa
```

If app take up `4321` port, open `chrome://serviceworker-internals/?devtools` and unregister it.