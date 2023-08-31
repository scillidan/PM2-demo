# PM2-demo

[![](https://img.shields.io/static/v1?style=for-the-badge&message=atom&color=222222&logo=RSS&logoColor=FFA500&label=)](https://github.com/scillidan/PM2-demo/commits/main.atom)
[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

Some web applications and tools I collected. Mainly used on `localhost`. I plan to use [PM2](https://pm2.keymetrics.io/) to manage some local services that I using.  
See [table.md](table.md).

## Notes

Start multiple app with `ecosystem.config.js`:

```js title="ecosystem.config.js"
{
	"apps": [
		{
			"name": "regexr",
			"interpreter": "C:\\Users\\scillidan\\AppData\\Roaming\\fnm\\node-versions\\v10.21.0\\installation\\node",
			"script": "C:\\Users\\scillidan\\AppData\\Roaming\\pnpm\\global\\5\\.pnpm\\gulp-cli@2.3.0\\node_modules\\gulp-cli\\bin\\gulp.js"
		},
		{
			...
		},
		...
	]
}
```

```sh
pm2 start
```

Set `pm2` as service on Windows10:

```sh
git clone https://github.com/jessety/pm2-installer
npm run configure
scoop install gsudo
gsudo npm run setup
gsudo pm2 save
```sh

After reboot:

```sh
gsudo pm2 list
```

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