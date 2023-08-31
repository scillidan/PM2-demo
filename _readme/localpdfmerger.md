## Localhost

```sh
yarn
```

```sh
yarn build
```

Edit near line `4` of `package.json`:

```json title="package.json"
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start -p 4321"
}
```
```sh
yarn start
```
