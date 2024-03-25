# `hmun-web` Contributing Guide

## 1. Get up & running locally

After cloning, run this in a terminal:

```sh
npm ci
```

This will install all build dependencies you need to start working.

To spin up a local development server, run:

```sh
npm run dev
```

This will start a Zola instance at http://localhost:1111, and a PostCSS build
script, all hot-reloading changes in the current directory.

## 2. Directory structure

We use a semi-modified set of Zola's default directory structure:

- `content/` contains Markdown for each individual page. Every `.md` file added
  will automatically appear on the navigation bar.
- `static/` contains non-code assets that are included in the final build.
- `styles/` contains common CSS code for [every page](styles/base.css) and
  specifically [the content pages](styles/page.css).
- `templates/` contains the template for [every page](templates/base.html),
  common elements like the [navbar](templates/navbar.html) and
  [footer](templates/footer.html), [the index page](templates/index.html), and
  [the content pages](templates/page.html).
- `templates/shortcodes/` contains Zola shortcodes, and also JavaScript code.
  Include these in `content/*.md` files with the `{{ shortcode() }}` syntax.

## 3. Commit conventions

Please use descriptive commit messages, and batch commits together into a
single push.
