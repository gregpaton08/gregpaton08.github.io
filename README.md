# [gregpaton08.com](gregpaton08.com)

## Instructions to Run Locally

### Install jekyll

```bash
brew update
brew install ruby
export GEM_HOME="$HOME/.gem"
gem install bundler jekyll
export PATH=$HOME/.gem/bin:$PATH

# You may also need to:
rm Gemfile.lock
bundle install

docker run --rm \
  --volume="$PWD:/srv/jekyll:Z" \
  -it jekyll/jekyll \
  jekyll build
```

### Build and Run

```bash
jekyll build
jekyll serve
```

## References

[jekyll](https://jekyllrb.com/docs/)  
[liquid](https://shopify.github.io/liquid/)
[minima](https://github.com/jekyll/minima)
