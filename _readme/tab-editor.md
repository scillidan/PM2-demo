## Localhost

```sh
npm i
```

Edit near line `33` of `server.js`:

```js title="server.js"
app.listen(3005, 'localhost', function(err) {
  if (err) {
    return console.log(err);
  }

  console.log('Listening at http://localhost:3005');
});
```

```sh
npm start
```