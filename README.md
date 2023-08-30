# PM2-demo

[![](https://img.shields.io/static/v1?style=for-the-badge&message=atom&color=222222&logo=RSS&logoColor=FFA500&label=)](https://github.com/scillidan/PM2-demo/commits/main.atom)
[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

Some web applications and tools I collected. Mainly used on `localhost`. I plan to use [PM2](https://pm2.keymetrics.io/) to manage some local services that I using.  
See [table.md](table.md).

## Tools

- [PM2](https://pm2.keymetrics.io/)
- [pm2-installer](https://github.com/jessety/pm2-installer)
- [Watchexec](https://github.com/watchexec/watchexec)

## Notes

Set `pm2` as service on Windows10:

```
git clone https://github.com/jessety/pm2-installer
npm run configure
scoop install gsudo
gsudo npm run setup
pm2 save
```

After reboot:

```
gsudo pm2 list
```

In addition, I use this command to run `hexo g` automatically after `reference\source\_posts\*.md` are modified.

```
cd reference
watchexec -w source\_posts -- hexo g
```

I use `.vbs` to set it to run in the background after booting.


## Reference

- [Process management](https://pm2.keymetrics.io/docs/usage/process-management/)
- [Persistent applications](https://pm2.keymetrics.io/docs/usage/startup/)
- [Configuration file](https://pm2.keymetrics.io/docs/usage/application-declaration/)
- [PM2 as a static server](https://pm2.keymetrics.io/docs/usage/expose/)
- [State is now: Stopped](https://github.com/jessety/pm2-installer/issues/69)
- [Spawning PM2 daemon with pm2_home=/home/tealou/.pm2](https://github.com/Unitech/pm2/issues/2799)