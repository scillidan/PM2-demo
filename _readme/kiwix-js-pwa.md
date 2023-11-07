## PWA

```sh
npm i
npm run build
npm run serve
```

Open `localhost:5173` → Install PWA.

Setting → Use Private File System → Add file(s) → Add to OPFS → Select your `.zim` → Wait for it to complete.

## PM2

```sh
pm2 serve dist 5173 --name kiwix-js-pwa --spa --env production
```