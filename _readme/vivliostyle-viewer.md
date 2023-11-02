## Localhost

Download from [Vivliostyle Viewer](https://github.com/vivliostyle/vivliostyle.js/tree/master/packages/viewer)

Decompress the archive.

```sh
serve -s viewer -p 4321
```

## PM2

```sh
pm2 serve viewer 4321 --name vivliostyle-viewer --spa
```