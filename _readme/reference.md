## Localhost

Optional command:

```sh
pnpm add pug -g
pnpm add katex -g
scoop install mongosh
```

```sh
npm i
```

```sh
npm run build
```

```sh
npm run dev
```

## PM2

Edit near line `16` of `_config.yml`:

```yml title="_config.yml"
url: http://localhost
```

```sh
hexo g
```

```sh
pm2 serve public 4321 --name reference --watch --spa
```

Create a `watchexec_reference.cmd`:

```sh title="watchexec_reference.cmd"
cd yourpath/reference && watchexec -w source\_posts -- hexo g
```

It say: After editing `source/_posts/*.md`, run `hexo g` automatically.

Create a `watchexec_reference.vbs` to hide the running interface:

``` title="watchexec_reference.vbs"
Set WshShell = CreateObject("WScript.Shell")
  WshShell.Run chr(34) & "yourpath\watchexec_reference.cmd" & Chr(34), 0
Set WshShell = Nothing
```

Open `Task Scheduler`, create a task. Set it *start after each boot* and *if the scheduled start time is past, start the task immediately*.