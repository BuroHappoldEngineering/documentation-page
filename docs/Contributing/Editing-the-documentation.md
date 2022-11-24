# Editing the documentation

This documentation is set as a simple set of Markdown documents. 

The markdown documents are automatically grabbed and transformed into an HTML website thanks to a set of GitHub actions that run [mkdocs](https://www.mkdocs.org/).

On top of Mkdocs, we also use:
- an extender theme called [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/), which exposes more customisation and [extra functionality](https://squidfunk.github.io/mkdocs-material/reference/).
- a plugin for customising the sorting of the pages: [mkdocs awesome pages plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin)


## Customising the ordering of the pages in the menu

Check the `.pages` file in the `docs` folder.

You can customise it according to [mkdocs awesome pages plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin).

## Customising the appearance of the documentation

See the available customisations of [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/).

The settings are placed in the `mkdocs.yml` file in the root of this repo.