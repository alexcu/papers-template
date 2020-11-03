# LaTeX Template for Software Engineering Papers

This is a template repository to bootstrap writing papers in LaTeX.

The template repository supports the following popular LaTeX classes used in
Software Engineering venues:

* [**`acmart`**](https://www.acm.org/binaries/content/assets/publications/consolidated-tex-template/acmart.pdf) - ACM journals and conferences
* [**`IEEEtran`**]() - IEEE Transactions journals and conferences
* [**`llncs`**](https://www.springer.com/gp/computer-science/lncs/conference-proceedings-guidelines) - Springer conference proceedings
* [**`IEEEcsmag`**](https://www.springer.com/gp/computer-science/lncs/conference-proceedings-guidelines) - IEEE Computer Society magazine articles
* [**`elsarticle`**](https://www.elsevier.com/authors/author-schemas/latex-instructions) - Elsevier articles

## Template Structure

* Write your article within `main.tex`. You can choose to rename this file to your venue.
* Make additional preamble modifications within `preamble.tex`.
* Enter in appropriate frontmatter (e.g., authors, titles) within `frontmatter/[clsname].tex`. Use the frontmatter file suitable for your selected venue.
* Place images within `images/` and, if you wish, tables within `tables/`.
* Select which `cls` file you want within the `\documentclass{./cls/[clsname]}`. These are within `cls/` directory. Then add suitable options to this class.
* Select which options for the selected class you want under `\documentclass[opt1,opt2...]{clsname}`.

## Options for classes

### Conference proceeding mode

### Journal article mode

### Draft mode

### Camere ready mode