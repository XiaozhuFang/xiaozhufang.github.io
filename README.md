# Xiaozhu Fang’s academic website

This Jekyll site is served at [xiaozhufang.github.io](https://xiaozhufang.github.io/).

## Editing the site

- Edit the profile, research interests, thesis and education in `_pages/about.md`.
- Edit publications in `_data/papers.yml`. Each entry belongs to the journal, conference or manuscript category. Add `selected: true` to feature an entry on the homepage.
- Update awards, service and teaching in their respective files under `_pages/`.
- Change the portrait, contact links and location in `_config.yml`. The menu is in `_data/navigation.yml`.

The shared layout is `_layouts/academic.html`. Styles are in `assets/css/academic.css` and `assets/css/academic-records.css`.

## Local preview

With Ruby and Bundler installed, run the following from this directory.

```sh
bundle install
bundle exec jekyll serve
```

Open [localhost:4000](http://localhost:4000/) to preview the site. GitHub Pages uses the same source files.
