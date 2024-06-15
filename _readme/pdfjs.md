## Localhost

Download `pdfjs-xxx-dist.zip` from [Releases](https://github.com/mozilla/pdf.js/releases) and decompress it.

```sh
cd pdfjs-dist/
scoop install dufs
dufs
```

Open `localhost:5000/web/viewer.html`, or open `localhost:4007/web/viewer.html?file=book.pdf`.

Or:

Install [GTK 2](https://github.com/Automattic/node-canvas/wiki/Installation:-Windows#2-installing-gtk-2), then:

```sh
pnpm install node-pre-gyp
```

```sh
git clone https://github.com/mozilla/pdf.js
cd pdf.js
npm i
npm i -g gulp-cli
gulp generic
dufs build/generic
```

See [Error on npm install](https://github.com/mozilla/pdf.js/issues/15112) and other issues for troubleshooting.

## PM2

```sh
pm2 serve build/generic/ 4321 --name pdfjs --spa
```

Open `localhost:4321/web/viewer.html`