# mike.fi

My home page at mike.fi, hosted with GitHub Pages using Jekyll.

## Local setup

Installing from scratch with homebrew:

```sh
brew install rbenv
# On an ARM-based M1 Mac, instead run:
# CFLAGS="-Wno-error=implicit-function-declaration" RUBY_CONFIGURE_OPTS='--with-readline-dir=/usr/local/opt/readline/' arch -x86_64 rbenv install 2.5.3
rbenv install 2.5.3
rbenv shell 2.5.3
gem install bundle
rm Gemfile.lock
bundle install --path vendor/bundle
```

Then start the server:

```sh
bundle exec jekyll serve
```

Or build:

```sh
bundle exec jekyll build
```


## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
