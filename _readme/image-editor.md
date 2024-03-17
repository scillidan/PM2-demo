## Localhost

```sh
fnm install 16.20.0
fnm use 16.20.0
```

```sh
npm i
```

```sh
npm run build
```

```sh
serve -s build -l 4321
```

## PM2

```sh
pm2 serve build 4321 --name image-editor --watch --spa
```