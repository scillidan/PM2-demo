## Localhost

```
npm install --legacy-peer-deps
npm run build
```

```sh
serve -s build -p 4321
```

## PM2

```sh
pm2 serve build 4321 --name recoded --spa
```