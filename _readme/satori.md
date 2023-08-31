## Localhost

```sh
fnm install 16.20.0
fnm use 16.20.0
```

```sh
pnpm i
```

```sh
pnpm dev:playground -- -p 4321
```

## PM2

...

```sh
set PORT=4005
pm2 start -n "satori" --cwd "./" "./node_modules/turbo/bin/turbo" -- dev --filter=satori-playground...
```

