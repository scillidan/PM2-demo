## Localhost

Add your books by editing `epub_content/`

```sh
serve -s . -p 4321
```

If app take up `4321` port, open `chrome://serviceworker-internals/?devtools` and unregister it.

## PM2

```sh
pm2 serve . 4321 --name sreadium --spa
```

When you use `pm2`, if you want to read audiobook, use Firefox. There are some problems on Chrome.