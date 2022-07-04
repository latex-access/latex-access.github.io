---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Latex-access, providing easy on-the-fly Braille and speech access to LaTeX documents
description: "The latex-access project is a Python package designed to provide a realtime translation of a line of LaTeX into braille, using either the Nemeth or UEB code, which can be read on a refreshable braille display. This will greatly improve the ease of use of LaTeX to blind mathematicians and scientists.  The project also translates the current line into english speech which is easier to listen to than LaTeX source."
---

## What is the Latex-access Project?
The latex-access project is designed to provide a realtime translation of a line of LaTeX into braille, using either the Nemeth or UEB code, which can be read on a refreshable braille display. This will greatly improve the ease of use of LaTeX to blind mathematicians and scientists.  The project also translates the current line into english speech which is easier to listen to than LaTeX source.

Note that this project is largely aimed at people wishing to read LaTeX using a refreshable braille display and/or speech synthesiser, and people who will probably want to edit LaTeX documents. For example, a university student could receive  worksheets in LaTeX format and produce their work using LaTeX. Using the latex-access scripts, they  will be  able to get a fairly good translation of the question and then an on-the-fly translation of their work as they produce it. If you are not concerned with editing LaTeX documents and simply want a braille translation of an entire laTeX document, then this project is not for you.

## Why the Need for the Project Latex-access?
It is widely thought that LaTeX is a good system for a blind mathematician or scientist to use to create and read scientific documents, as it is a linear code and so the user does not have to interact  with two-dimensional notation, such as fractions and column vectors. By reading this linear code, a blind person can take in and understand scientific documents in the same way that a sighted person would do by studying a printed document. It should be noted that normally, laTeX is just a source from which documents are converted into an attractive-looking, typeset document that can be printed or viewed on screen, often in a .pdf, .dvi or .ps format. For various technical reasons, documents in such formats are currently inaccessible with current screen-reading technology. The best current solution therefore is not to concern ourselves with documents in these formats, but rather to read and interpret the LaTeX source code itself.

## Reading a LaTeX Document
It is entirely possible to read a LaTeX document simply by reading the LaTeX source itself. This however, is often a time-consuming and pain-staking process, and it is often not particularly nice to read. For example, the LaTeX source for the quadratic formula is <br/>
```tex
$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$
```
It is therefore the aim of the project to translate a line of LaTeX into a line of braille code, which can be read using a refreshable braille display. The project also aims to provide an audible translation of the LaTeX source which will be output through current screen-reading technology.

## Current Features
Latex-access currently contains the following features:
* Translation of many mathematical expressions from LaTeX to Nemeth or UEB  braille and English speech. These include, but are not confined to:
  * Translation of fractions, both numerical and algebraic.
  * Translation of trigonometric functions and hyperbolic functions.
  * Translation of powers, including square roots.
  * Translation of expressions used in calculus, including partial derivatives.
  * Translation of numerous  mathematical symbols, such as the Greek letters.
  * Many commands used to create a visually attractive document are either translated or ignored, often it is not necessary to see some formatting commands.
* A matrix browser feature to enable easier reading of larger matrices in LaTeX, see the description below.
*  Support for custom defined LaTeX commands.
* Interfaces to the Windows screen readers [JAWS](https://www.freedomscientific.com/products/software/jaws/) and [NVDA](https://www.nvaccess.org/about-nvda/).
* Interfaces to [BRLTTY](http://mielke.cc/brltty/) and [Emacspeak](http://emacspeak.sourceforge.net/) under Linux.
  * When using BRLTTY, cursor routing keys on Braille displays are supported making navigation much simpler.

## The matrix browser
As most refreshable braille displays are currently limited to one line, manipulating matrices (EG multiplication) simply by reading LaTeX source code poses a problem, as we often need to see elements in different rows of a matrix at the same time. For smaller matrices we can usually do this by memorising the matrix, however for larger matrices (usually 3 by 3 and above), this becomes impossible. Therefore we have developed a browser interface which greatly eases the stress involved in performing matrix operations.

## The Preprocessor
One of the many powerful features of LaTeX is the ability to define custom commands.  Latex-access includes a mechanism, the preprocessor, for including the definitions of such commands in the translation.  Once commands have been added to the preprocessor they can be saved to a file for future use.

## Obtaining the scripts
The scripts are  available on Github. The URL for the repository is<br/>
[https://github.com/latex-access/latex-access](https://github.com/latex-access/latex-access)
You can clone it with the following command<br/>
```
git clone --recursive https://github.com/latex-access/latex-access.git
```


## Contacting the Developers
The developers of the project are always happy to answer any questions you may have.  We are also keen to hear suggestions for any improvements or new features.  Rather than contacting an individual developer directly it is probably best that you do one of the following:
* Use our [mailing list](https://lists.sourceforge.net/lists/listinfo/latex-access-devel)
* Use the [issue tracker](https://github.com/latex-access/latex-access/issues) on Github to report any bugs or offer feature suggestions. You can create a new one [here](https://github.com/latex-access/latex-access/issues/new).
