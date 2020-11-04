# LaTeX Template for SoftEng and CompSci Papers

This template repository helps you bootstrap writing papers in LaTeX.

The template supports the following popular document classes that are used in popular software engineering and computer science venues:

* [**`acmart`**](https://www.acm.org/binaries/content/assets/publications/consolidated-tex-template/acmart.pdf) - ACM journals and conferences. View source on [CTAN](https://ctan.org/tex-archive/macros/latex/contrib/acmart). Readme available [here](https://www.acm.org/binaries/content/assets/publications/consolidated-tex-template/acmart.pdf).
* [**`IEEEtran`**](https://www.ieee.org/conferences/publishing/templates.html) - IEEE journals and conferences. View source on [CTAN](https://ctan.org/tex-archive/macros/latex/contrib/IEEEtran). Readme available [here](https://ras.papercept.net/conferences/support/files/IEEEtran_HOWTO.pdf).
* [**`llncs`**](https://www.springer.com/gp/computer-science/lncs/conference-proceedings-guidelines) - Springer Lecture Notes in Computer Science, conference proceedings. Readme is avaliable [here](https://cs.brown.edu/about/system/managed/latex/doc/llncs.pdf).
* [**`elsarticle`**](https://www.elsevier.com/authors/author-schemas/latex-instructions) - Elsevier articles. View source on [CTAN](https://ctan.org/tex-archive/macros/latex/contrib/elsarticle).
* [**`IEEEcsmag`**](https://www.springer.com/gp/computer-science/lncs/conference-proceedings-guidelines) - IEEE Computer Society magazine articles.

## Getting Started

Here are the basics with getting started:

1. Write your article within `main.tex`. You can rename this file to the same as your repo, e.g.: `icse2020.tex`.
1. Update the document class on line 1 with the document class and appropriate options suitable to your venue. The document class and associated options are usually provided by your venue's call for papers site.
1. You should also include the `preamble.tex` file and make changes in the preamble within that file. The `preamble.tex` file is already included by default on line 3.
1. Update the associated `frontmatter/` file on line 7 to the one associated with your document class. Each document class has its own frontmatter file. Examples are shown below.
1. Edit the content of the frontmatter file imported with a new title, author(s), abstract and keywords. Additional publication details are included in this file as well.

By default, the `acmart` document class and frontmatter file is used.

**Remember, this template is just to help you get started. You will have to refer to the individual document class READMEs to make suitable changes appropriate to your particular venue.**

Below are a few examples to help guide you.

### Conference Papers
**ACM Conferences:**
Use the `acmart` (ACM article) with the `sigconf` option enabled. The `authordraft` option should be enabled used whilst editing with coauthors, and when you submit your article this should be changed to `review`. Since most ACM conferences are double-blind, you should use `anonymous`.
```latex
\documentclass[sigconf,authordraft,anonymous]{acmart} % <- Replace line 1
\input{preamble}
\begin{document}
\input{frontmatter/acmart-sigconf}                    % <- Replace line 7
\end{document}
```

**IEEE Conferences:**
Use the `IEEEtran` document class with the `conference` option enabled. The vast majority of IEEE papers also use the `10pt` option.
```latex
\documentclass[conference,10pt]{IEEEtran} % <- Replace line 1
\input{preamble}
\begin{document}
\input{frontmatter/IEEEtran-conference}   % <- Replace line 7
\end{document}
```

**Springer Lecture Notes in Computer Science articles:**
Use the `llncs` for Springer Lecture Notes in Computer Science articles. You should use the `runningheads` option unless otherwise specified. <mark>Important!</mark> You must to download a [copy](https://www.win.tue.nl/~setalle/tex/llncs.cls) of the llncs class file and place into the root of your project as it is not pre-uploaded in Overleaf.
```latex
\documentclass[runningheads]{llncs} % <- Replace line 1
\input{preamble}
\begin{document}
\input{frontmatter/llncs}           % <- Replace line 7
\end{document}
```

### Journals & Magazine Articles
**IEEE Journals:**
Use the `IEEEtran` document class with the `journal` and `compsoc` options enabled for IEEE Journal articles. The vast majority of IEEE papers also use the `10pt` option.
```latex
\documentclass[journal,compsoc,10pt]{IEEEtran} % <- Replace line 1
\input{preamble}
\begin{document}
\input{frontmatter/IEEEtran-journal-compsoc}   % <- Replace line 7
\end{document}
```

**Elsevier Article:**
Use the `elsarticle` document class with the `review` option enabled for a Elsevier journal article.
```latex
\documentclass[review]{elsarticle} % <- Replace line 1
\input{preamble}
\begin{document}
\input{frontmatter/elsarticle}     % <- Replace line 7
\end{document}
```

**IEEE Computer Science Magazine:**
Use the `IEEEcsmag` document class for an IEEE Computer magazine article.
```latex
\documentclass{IEEEcsmag}     % <- Replace line 1
\input{preamble}
\begin{document}
\input{frontmatter/IEEEcsmag} % <- Replace line 7
\end{document}
```

## Common Venues and Document Classes

Here are a list of common venues with the document classes they use.

* `acmart`: ESEC/FSE, ICSE, CHI.
* `IEEEtrans` with `conference`: ESEC/FSE, ICSE, ICSME, ESEM.
* `llncs`: ICWE.
* `elsarticle`: IST, JSS.
* `IEEEtrans` with `compsoc,journal`: TSE.
* `IEEEcsmag`: IEEE Computer, IEEE Software.

## Contributing

Please raise an issue on GitHub and/or contribute a fix via a pull request if you:

* find that a popular document class is not listed above;
* find that one of your venues is not listed above;
* if there are any issues with this document template;
* have any suggestions!
