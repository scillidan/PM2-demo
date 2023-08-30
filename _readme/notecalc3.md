## Localhost

```sh
cargo install wasm-pack
```

```sh
rustup override set nightly-2020-11-17
```

```sh
wasm-pack build --release --target no-modules frontend-web
```

But it didn't work. So just:

```sh
serve -s . -p 4321
```