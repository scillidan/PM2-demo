# PM2-demo

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

Some web applications and tools I collected. Mainly used on `localhost`. I plan to use [PM2](https://pm2.keymetrics.io/) to manage some local services that I using.  
And I used [fnm](https://github.com/Schniz/fnm), default Node.js version is `18.15.0`.  
See [table.md](table.md). 

## Start

See links on [Reference](README.md#reference) and `*.md` such as [reference.md](_readme/reference.md).

after `pm2 start ...`, if you want to save app:

```sh
gsudo pm2 save
```

Then, set `pm2` to run automatically at startup. On Windows10, you need:

```sh
scoop install gsudo
git clone https://github.com/jessety/pm2-installer
cd pm2-installer
gsudo npm run configure
gsudo npm run setup
```

Windows → Control Panel → Administrative Tools > Services → PM2 → Properties → Log On → local system account → Go back to first tab → Start

If you want to start multiple app with `ecosystem.config.js`, create `ecosystem.config.js` and edit. I didn't use this way:

```js
{
	"apps": [
		{
			"name": "regexr",
			"interpreter": "C:\\Users\\yourname\\AppData\\Roaming\\fnm\\node-versions\\v10.21.0\\installation\\node",
			"script": "C:\\Users\\yourname\\AppData\\Roaming\\pnpm\\global\\5\\.pnpm\\gulp-cli@2.3.0\\node_modules\\gulp-cli\\bin\\gulp.js"
		},
		{
			...
		},
		...
	]
}
```

Then `pm2 start`.

## Reference

- [Process management](https://pm2.keymetrics.io/docs/usage/process-management/)
- [PM2 as a static server](https://pm2.keymetrics.io/docs/usage/expose/)
- [Cli Reference](https://pm2.io/docs/runtime/reference/pm2-cli/)
- [Configuration file](https://pm2.keymetrics.io/docs/usage/application-declaration/)
- [快速开始](https://pm2.fenxianglu.cn/docs/start)
- [Persistent applications](https://pm2.keymetrics.io/docs/usage/startup/)
- [pm2-installer](https://github.com/jessety/pm2-installer)

## Troubleshooted

- [State is now: Stopped](https://github.com/jessety/pm2-installer/issues/69)
- [Spawning PM2 daemon with pm2_home=/home/tealou/.pm2](https://github.com/Unitech/pm2/issues/2799)