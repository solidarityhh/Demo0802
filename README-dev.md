# Dev setup

> **NOTE:** Make sure you have Ruby installed.

```bash
bundle install
# will host the page in local network
bundle exec jekyll serve --livereload --host=0.0.0.0
```

## Deployment

This project uses tailwindcss thus requiring an additional build step before deploying to gh actions:

```bash
pnpm install
# takes the content of css/input.css and writes a minified version to css/output.css
pnpm build
```