## Localhost (TBD)

```sh
rbenv install 3.3
```

```sh
gem install bundler
bundle install
bundle exec thor docs:download --default
bundle exec rackup
```


## Troubleshot

- [Any pod command fails for lack of libcurl.dll on a Windows machine.](https://github.com/CocoaPods/CocoaPods/issues/9955)
- [Not installable on Windows](https://github.com/freeCodeCamp/devdocs/issues/1152)