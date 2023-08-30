## Localhost

```sh
fnm install 10.21.0
fnm use 10.21.0
```

```sh
npm i
```

Edit near line `62` of `./gulpfile.babel.js`:

```
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

```sh
fnm install 10.21.0
fnm use 10.21.0
```

```sh
touch pm2.json
```

``` title="pm2.json"
{
	"apps": [
		{
			"name": "regexr",
			"interpreter": "C:\\Users\\yourname\\AppData\\Roaming\\fnm\\node-versions\\v10.21.0\\installation\\node",
			"script": "C:\\Users\\yourname\\AppData\\Roaming\\pnpm\\global\\5\\.pnpm\\gulp-cli\\node_modules\\gulp-cli\\bin\\gulp.js"
		}
	]
}
```

```sh
pm2 start pm2.json
```

Open `localhost:3001`