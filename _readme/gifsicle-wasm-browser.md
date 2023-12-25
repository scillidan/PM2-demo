## Localhost

```sh
npm i
```

```sh
serve -s docs -p 4321
```

## PM2

```sh
pm2 serve docs 4321 --name gifsicle-wasm-browser --spa
```

If app take up `4321` port, open `chrome://serviceworker-internals/?devtools` and unregister it.