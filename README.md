# saliktehami.com

Source for Salik Tehami's personal site.

The site is built with [Jekyll](https://jekyllrb.com/) and intended for GitHub Pages. It is static-first: no global JavaScript, no external font dependencies, and a small custom CSS file.

## Local setup

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

The local site runs at `http://localhost:4000`.

## Structure

- `_posts/`: typed cases, concepts, reviews, notes, and sample formats.
- `cases.html`, `concepts.html`, `reviews.html`: the public casebook spine.
- `writing.html`: the full archive.
- `reading.md`, `tools.md`, `questions.md`, `about.md`: supporting artifact pages.
- `static/css/site.css`: the visual system.

## Credits

This site started from the permissively licensed `vlad17.github.io` Jekyll repo and was redesigned into a new personal site scaffold. The original repo credited the `hcz-jekyll-blog` theme.
