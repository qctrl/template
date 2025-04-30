# Home

Add folders and markdown files in the `docs/` directory

## Enabling Github Pages

To serve your site from the [gh-pages](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages) branch, you’ll first need to configure your GitHub repository settings. See the steps below.

- Go to your Github repository and create a new branch named `gh-pages`.
    - ⚠️ This **should** be done in the Github web interface, **not** via the `git` command

- This will create the `gh-pages` settings and deployment workflows automatically.

- Use the Q-Ctrl [mkdocs reusable workflow](https://qctrl.github.io/reusable-workflows/workflows/#mkdocs-build-and-deploy) to deploy with `mkdocs`
    - ℹ️ Use subcommand `build` for `on-push` event to any branch. See example [here](https://github.com/qctrl/reusable-workflows/blob/master/.github/workflows/build-docs.yaml)
    - ℹ️ Use subcommand `gh-deploy` for `on-push` event to master branch. See example [here](https://github.com/qctrl/reusable-workflows/blob/master/.github/workflows/deploy-docs.yaml)

### Helpful links

- [material-mkdocs](https://squidfunk.github.io/mkdocs-material/reference/) references
- [user-guide/writing-your-docs](https://www.mkdocs.org/user-guide/writing-your-docs/)
- [mkdocs/catalog](https://github.com/mkdocs/catalog)

### Plugins to consider

- [docstrings](https://mkdocstrings.github.io/)
- [mkdocs-jupyter/](https://pypi.org/project/mkdocs-jupyter/)
- [mike](https://pypi.org/project/mike/)
