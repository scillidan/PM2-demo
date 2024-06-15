## Localhost

```sh
fnm install 16.20.0
fnm use 16.20.0
```

Edit near line `5` of `nuxt.config.js`:

```json title="nuxt.config.js"
  server: {
    host: "localhost",
    port: 3003
  },
```

```sh
npm install
npm run generate
```

```sh
npm run start
```

## PM2 (Ubuntu 22.04.4 ARM)

```sh
pm2 start npm --name "qr-designer" -- run start
```