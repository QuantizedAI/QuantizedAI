# Swissup Docs

[quantizedai.com](https://quantizedai.com/)

## Requirements

 -  Ruby and ruby-dev
 -  Node.js and NPM

## Installation

```bash
git clone git@github.com:swissup/swissup.github.io.git && cd swissup.github.io

# Install bundler is you don't have it
gem install bundler

# Install dependencies
bundle install && npm install
```

## Updating

```bash
git pull && bundle install && npm install
```

## Running

With Gulp:

```bash
gulp
```

Without Gulp:

```bash
bundle exec jekyll serve --livereload --incremental
```
