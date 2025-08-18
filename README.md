# David Plumridge's Personal Site

![Jekyll](https://img.shields.io/badge/Jekyll-4.3.4-red)
![Ruby](https://img.shields.io/badge/Ruby-3.2.2-red)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-latest-green)

My personal website built with Jekyll and hosted on GitHub Pages. Visit at [davidplumridge.com](http://davidplumridge.com).

## 📋 Prerequisites

- Ruby 3.2.2 (install via [rbenv](https://github.com/rbenv/rbenv) or [rvm](https://rvm.io/))
- Bundler gem

## 🧪 Development Commands

```bash
# Quick start (recommended - uses correct Ruby version)
sh _runDev.sh

# Or manually:
# Install dependencies
bundle install

# Start Jekyll development server
bundle exec jekyll serve

# Build the site
bundle exec jekyll build

# Clean the build
bundle exec jekyll clean
```

## 🛠️ Setup Notes

- The project uses Ruby 3.2.2 (specified in `.ruby-version`)
- If using rbenv, it will automatically switch to the correct Ruby version
- Dependencies are installed locally to `vendor/bundle/` to avoid permission issues