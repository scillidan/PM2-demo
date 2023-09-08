## Vercel

1. Fork [excalith/excalith-start-page](https://github.com/excalith/excalith-start-page)
2. Import your fork to [Vercel](https://vercel.com/goblin-market)

## PM2

```sh
yarn
```

```sh
pm2 start yarn --watch --name "excalith-start-page" -- dev
```

Open the site, then:

```sh
config import https://gist.githubusercontent.com/scillidan/0d37c44fc21ddb8eee0615c35a289d16/raw/d3fffcaa2db7c39d870b9f9cacdd10c5d1f5f095/excalith-start-page.json
```