## Localhost

```sh
npm i
```

```sh
npm run build
```

## PM2

```sh
hexo g
```

```sh
pm2 serve public 4321 --name reference --watch --spa
```

After editing `source/_posts/*.md`, run `hexo g` automatically:

```sh
watchexec -w source\_posts -- hexo g
```

I use `.vbs` to set this to run in the background after booting.