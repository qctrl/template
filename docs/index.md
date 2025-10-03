# Home

To turn your project docs into a website, first start by adding folders and Markdown files in the `docs/` directory.

It is strongly recommended to use the [Q-CTRL MkDocs Theme](https://github.com/qctrl/mkdocs-theme), which provides a highly opinionated, low configuration theme for making consistent Q-CTRL project documentation. For more information, see the [Q-CTRL MkDocs documentation](https://crispy-dollop-z25wl2k.pages.github.io/).

## Enabling GitHub Pages

To serve your site from the [`gh-pages`](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages) branch, you’ll first need to configure your GitHub repository settings. See the steps below.

- Go to your GitHub repository and create a new branch named `gh-pages`.
    - ⚠️ This **should** be done in the Github web interface, **not** via the `git` command

- This will create the `gh-pages` settings and deployment workflows automatically.

- Use the Q-CTRL [MkDocs reusable workflow](https://qctrl.github.io/reusable-workflows/workflows/#mkdocs-build-and-deploy) to deploy with `mkdocs`
    - ℹ️ Use subcommand `build` for `on-push` event to any branch. See example [here](https://github.com/qctrl/reusable-workflows/blob/master/.github/workflows/build-docs.yaml)
    - ℹ️ Use subcommand `gh-deploy` for `on-push` event to master branch. See example [here](https://github.com/qctrl/reusable-workflows/blob/master/.github/workflows/deploy-docs.yaml)

### Helpful links

- [material-mkdocs](https://squidfunk.github.io/mkdocs-material/reference/) references
- [user-guide/writing-your-docs](https://www.mkdocs.org/user-guide/writing-your-docs/)
- [mkdocs/catalog](https://github.com/mkdocs/catalog)

### Plugins to consider

- [mkdocstrings](https://mkdocstrings.github.io/)
- [mknotebooks](https://github.com/greenape/mknotebooks)
- [mike](https://pypi.org/project/mike/)
