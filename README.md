# Ahmed Alharbi — DHS coursework

Jekyll course website deployed by GitHub Pages from **master / (root)**.
The site URL is https://aka7979nyu.github.io/dhs/ and `_config.yml` keeps `baseurl: /dhs`.

## Content

- `index.html`: project portfolio homepage.
- `_pages/`: about, writing, archive and error pages.
- `_posts/`: add real coursework using `YYYY-MM-DD-title.md` with title front matter.
- `BH_featuremapNEW.html`: published Bahrain Leaflet map. Keep this filename and its four layers, Thunderforest.Outdoors basemap and metric scale bar.
- `assets/css/site.css`: responsive site styles.

The Bahrain assignment blog post is pending, but website has been redesigned. 

## Build

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll build
bundle exec jekyll serve
```

Open http://localhost:4000/dhs/. GitHub Pages uses the same `github-pages` dependencies.
Local layouts and ordinary Liquid/Markdown require no custom plugins or JavaScript build step.
