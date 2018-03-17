# The `apalike-german` package: an author year style for BibTeX

## Objective

I made `apalike-german.bst` because I was forced to use plain old BibTeX in conjunction with `apalike.bst` but I needed German localization. It is simply a copy of the original file. My editions concern the following:

 - Inserted words were translated to German.
 - Puryifing of label numbers is removed. Thus, dots in the label year shall not be removed.
 - Capitalization of title words will remain.

## Installing

Create the directory `{TEXMF}/bibtex/bst/apalike-german`, move `apalike-german.bst` there and update the file name database.

## Usage

First let me point out that if you are not forced to use plain BibTeX it is much better to rely on the `biblatex` package, preferably in conjunction with Biber. Thus, you gain much more flexibility for your references. If you took this into account, call `\bibliographystyle{apalike-german}` as usual after `\begin{document}`.

In case a numerical year lacks you can use an expression like "n.d.":

    @MISC{undated-item,
      ...
      year = {o.J.},
    }

The dots are kept, but only four digits are allowed!

## Help

Best is to use the [GitHub tracker](https://github.com/CarlOrff/apalike-german).

Or visit me on [my website and use the comment function](https://ingram-braun.net/public/programming/tex/apalike-german-bst-bibtex-bibliography-author-date-style#ib_campaign=$apalike-german&ib_medium=repository&ib_source=readme) there.

## History

 - 11-sep-2016: Original version by Ingram Braun
 - 17-mar-2018: Macro `mar` bug fixed ([Issue #1](https://github.com/CarlOrff/apalike-german/issues/1)).

## Copyright

© 2016–2018 by [Ingram Braun](https://ingram-braun.net/#ib_campaign=$apalike-german&ib_medium=repository&ib_source=readme), 1986–2010 by Oren Patashnik.

## License

[The LaTeX Project Public License 1.3c or later](http://www.latex-project.org/lppl.txt)