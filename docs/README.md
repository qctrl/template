# Home

To turn your project docs into a website, first start by adding folders and Markdown files in the `docs` directory.

## Enabling GitHub Pages

To serve your site from the `gh-pages` branch, you’ll first need to configure your GitHub repository settings. See the steps below.

1. Go to your GitHub repository and create a new branch named `gh-pages`.
    1. ⚠️ This **must** be done via the GitHub web interface, **not** via the `git` command.
    1. This will create the `gh-pages` settings and deployment workflows automatically.
1. Use the Q-CTRL [MkDocs build and deploy](https://qctrl.github.io/reusable-workflows/workflows/#mkdocs-build-and-deploy) reusable workflow to deploy with MkDocs.
    1. ℹ️ Use subcommand `build` for `on-push` event to any branch.
        1. See the [Build mkdocs](https://github.com/qctrl/reusable-workflows/blob/master/.github/workflows/build-docs.yaml) reusable workflow.
    1. ℹ️ Use subcommand `gh-deploy` for `on-push` event to master branch.
        1. See the [Deploy Docs](https://github.com/qctrl/reusable-workflows/blob/master/.github/workflows/deploy-docs.yaml) reusable workflow.

## Helpful links

- [Q-CTRL MkDocs Theme](https://qctrl.github.io/mkdocs-theme)

## Plugins to consider

- [mkdocstrings](https://mkdocstrings.github.io/): Automatic documentation from sources.
- [mknotebooks](https://github.com/greenape/mknotebooks): Include Jupyter notebooks in your projects.
