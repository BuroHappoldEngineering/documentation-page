# Editing the documentation

This documentation is set as a simple set of Markdown documents, transformed into a proper web page thanks to [mkdocs](https://www.mkdocs.org/). 

If you want to add a page, just add an new markdown document. You also can embed:

- HTML blocks
- Latex/Mathjax, e.g. $f(x) = x^2$ (enclose the formula between single `$` for inline and double `$$` for block).


## Customising the ordering of the pages in the menu

Check the `.pages` file in the `docs` folder.

You can customise it according to [mkdocs awesome pages plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin).

## Customising the appearance of the documentation

See the available customisations of [Material for Mkdocs](https://squidfunk.github.io/): [setup](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/) and [extra elements](https://squidfunk.github.io/mkdocs-material/reference/).

The settings are placed in the `mkdocs.yml` file in the root of this repo.

## Technical addendums
### How do the markdown documents get translated to a web page?
The markdown documents are automatically grabbed and transformed into an HTML website thanks to a set of GitHub actions.

The actions were configured as described in https://squidfunk.github.io/mkdocs-material/publishing-your-site/.
Some extra actions are also configured in order to make the [dependencies](#Dependencies) available.

### Dependencies

On top of [mkdocs](https://www.mkdocs.org/), we also use:

- an extender theme called [Material for Mkdocs](https://squidfunk.github.io/mkdocs-material/), which exposes more customisation and [extra functionality](https://squidfunk.github.io/mkdocs-material/reference/).
- a plugin for customising the sorting of the pages: [mkdocs awesome pages plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin)