# lilperp.xyz

A tiny Jekyll personal site with two sections: About and Bookshelf.

## Run locally

Install Ruby 3.3.4 first. With `rbenv`, that looks like:

```sh
rbenv install 3.3.4
rbenv local 3.3.4
```

Then run:

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000>.

## Edit content

- About copy: `index.md` and `about.md`
- About content: `_includes/about-content.md`
- Bookshelf content: `_includes/bookshelf-content.md`
- Site title and metadata: `_config.yml`
- Styling: `assets/css/style.css`

## GitHub Pages

1. Push this repo to GitHub.
2. In the repository settings, open **Pages**.
3. Set the source to your default branch.
4. If using a custom domain, enter the domain in GitHub Pages settings. GitHub will create or expect a `CNAME` file containing that exact domain.

## Squarespace domain

In Squarespace DNS settings, point the domain to GitHub Pages:

- Apex/root domain: add these `A` records for `@`:
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`
- `www`: add a `CNAME` record pointing to `<your-github-username>.github.io`.

After DNS resolves, enable **Enforce HTTPS** in GitHub Pages.
