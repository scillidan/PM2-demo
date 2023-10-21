## Localhost

Add your books by editing `epub_content/`

```sh
serve -s . -p 4321
```

## PM2

```sh
pm2 serve . 4321 --name sreadium --spa
```

When you use `pm2`, if you want to read audiobook, use Firefox. There are some problems on Chrome.