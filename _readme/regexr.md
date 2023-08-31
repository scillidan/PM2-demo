## Localhost

```sh
fnm install 10.21.0
fnm use 10.21.0
```

```sh
npm i
```

Edit near line `62` of `./gulpfile.babel.js`:

```js title="gulpfile.babel.js"
gulp.task("serve", () => {
	browser({
		server: { baseDir: "./deploy/" },
		port: 3001,
	});
});
```

```sh
gulp
```

## PM2 (PC)

...

```sh
pm2 start "C:/Users/yourname/AppData/Roaming/pnpm/global/5/.pnpm/gulp-cli@2.3.0/node_modules/gulp-cli/bin/gulp.js" --interpreter "C:/Users/yourname/AppData/Roaming/fnm/node-versions/v10.21.0/installation/node.exe" -n regexr
```	

Open `localhost:3001`