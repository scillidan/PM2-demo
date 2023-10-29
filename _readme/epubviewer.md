## Localhost

```sh
serve -s . -p 4321
```

`localhost:4000#book.pdf` can also work.

If app take up `4321` port, open `chrome://serviceworker-internals/?devtools` and unregister it.

## PM2

```sh
pm2 serve . 4321 --name epubvidewer --watch
```