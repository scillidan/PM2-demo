## Localhost

```sh
yarn install
```

Edit near line `13` of `.eslintrc.json`:

``` title=".eslintrc.json"
	"rules": {
		"prettier/prettier": ["error", {'endOfLine': 'auto'} ]
```

```sh
yarn build
```

```sh
yarn start -- -p 4321
```