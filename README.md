# Ryan Peterson Personal Site

A blog-oriented jekyll site using [Hydejack](https://hydejack.com/).

## Quick Start
### Running locally
1. Clone repository (git users), or [download] and unzip.
2. Open terminal, `cd` into root directory (where `_config.yml` is located)
3. Run `bundle install` [^1]
4. Run `bundle exec jekyll serve`
5. Open <http://localhost:4000/>

### Troubleshooting
I ran into some issues on mac, but ended up doing everything with `chruby` I think the following steps worked:

```
brew install chruby
ruby-install ruby-3.2.2
```

Added below to `~/.zshrc`:
```
source /usr/local/share/chruby/chruby.sh
source /usr/local/share/chruby/auto.sh
```

This should allow `chruby` to auto-switch to the version in this repo (specified in `.ruby-version`)

**Note:** You may need to update xcode if you run into an error running `ruby-install`. I fixed it with `xcode-select --install` from [here](https://stackoverflow.com/questions/55505603/error-while-running-configure-when-installing-ruby-via-rvm-c-compiler-cannot-cr#comment118281048_55506052)

On mac, I used `brew install chruby` and then `ruby-install ruby-3.2.2` before getting bundler. You may need to follow the chruby installation steps from their website because it was quite a hassle.

## What's next?
* Open files and read the comments
* Read the [docs](https://hydejack.com/docs/)
* Buy the [PRO version](https://hydejack.com/download/) to get the project and resume layout, newsletter subscription box, custom forms, and more.

[^1]: Requires Bundler. Install with `gem install bundler`.

[download]: https://github.com/hydecorp/hydejack-starter-kit/archive/master.zip
