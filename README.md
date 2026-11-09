# Chirpy Starter

[![Gem Version](https://img.shields.io/gem/v/jekyll-theme-chirpy)][gem]&nbsp;
[![GitHub license](https://img.shields.io/github/license/cotes2020/chirpy-starter.svg?color=blue)][mit]

A minimal, ready-to-use template for creating a blog with the [**Chirpy**][chirpy] Jekyll theme. Get up and running in minutes with all critical files pre-configured.

## Why This Starter Exists

When installing Chirpy through [RubyGems.org][gem], Jekyll can only read a subset of theme files (`_data`, `_layouts`, `_includes`, `_sass`, `assets`) and limited `_config.yml` options from the gem. As a result, users cannot enjoy the full out-of-the-box experience that Chirpy offers.

To unlock all features, the following files must be present in your Jekyll site:

```shell
.
├── _config.yml
├── _plugins
├── _tabs
└── index.html
```

This starter bundles those files from the latest **Chirpy** release along with a [CD][CD] workflow, so you can start writing immediately.

## Usage

Check out the [theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

## Updating the website (step by step)

The site is published with GitHub Pages. Every push to `main` triggers the workflow in `.github/workflows/pages-deploy.yml`, which builds and deploys the site automatically.

1. Edit the files (for example `_tabs/about-me.md`, `_tabs/teaching.md`, `_tabs/research.md`).
2. (Optional) Preview locally from the project folder:

   ```shell
   bundle exec jekyll serve --livereload
   ```

   Then open <http://127.0.0.1:4000> and check the changes. Stop it with `Ctrl+C`.
3. Review what changed:

   ```shell
   git status
   git diff
   ```
4. Stage only the files you changed, for example:

   ```shell
   git add _tabs/about-me.md
   ```
5. Commit with a short message:

   ```shell
   git commit -m "Update about me"
   ```
6. Push to GitHub:

   ```shell
   git push origin main
   ```
7. Wait 1–3 minutes and check the deployment in the repository's **Actions** tab on GitHub. When it shows a green check, the changes are live at <https://mariosuaza.github.io>.

Notes:

- A push that only changes `README.md`, `LICENSE` or `.gitignore` does **not** trigger a deployment.
- To redeploy without changing anything, go to **Actions → Build and Deploy → Run workflow**.
- If the page does not show the changes, force-refresh the browser (`Cmd+Shift+R`).

## Contributing

This repository is automatically updated with new releases from the theme repository. If you encounter any issues or want to contribute to its improvement, please visit the [theme repository][chirpy] to provide feedback.

## License

This work is published under [MIT][mit] License.

[gem]: https://rubygems.org/gems/jekyll-theme-chirpy
[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[CD]: https://en.wikipedia.org/wiki/Continuous_deployment
[mit]: https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE


bundle exec jekyll serve 

bundle exec jekyll serve --livereload