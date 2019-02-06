# rebuttal.sty

The rebuttal LaTeX class provides environments and macros to format a point by point response to a journal article review. A section can be defined for each reviewer and the reviewer's points are automatically numbered. Labels can be added to the reviewers' points so that they can be cross referenced from responses.

The class can be used to format the rebuttal serially, i.e. reviewer's point followed by authors' response, or as two columns so that the authors' response appears alongside the reviewer's comment.

## Usage
The file rebuttal.sty from this package can either be placed in the directory in which the rebuttal document is being edited, or in one of the conventional places for storing local TeX and LaTeX files on your system. Then add one of the following lines to the preamble of your LaTeX document.

`\usepackage{rebuttal}`

`\usepackage[table]{rebuttal}`

The package accepts two options 'plain' and 'table'; 'plain' is the default option and can be omitted.

The package provides a pair of environments for the reviewer's `point` and a `response`, as well as a pair of macros for a `shortpoint` and a `shortresponse`. A `reviewersection` macro is used to begin each reviewer's comments, e.g.:

```
\reviewersection

\begin{point}
  ...
\end{point}
\begin{response}
  ...
\end{response}

\shortpoint{...}
\shortresponse{...}

```


See the example files included in this package for illustrations of how each option might be used (both source and PDF versions are provided). The default, plain option is the easiest to use. The table option has some formatting issues, can be brittle when used, and requires further refinement.

## Licence
The LaTeX package and examples are licensed under the terms of the Creative Commons CC-BY-SA v3.0. The origin of the macros and the licence are explained in the "History" section below.

## History
The LaTeX package has evolved from reponses to a question on StackOverflow.

* The LaTeX package and the example files are the work of Simon Butler.
* The LaTeX macros that form the core of the package are largely cosmetic revisions of macros published by Friedemann Zenke and available at https://fzenke.net/index.php/goodies/latex-rebuttal/ 
* Friedemann Zenke created his example by revising macros published by Dirk Eddelbuettel, Fran and others in responses to the following question on StackOverflow:  https://tex.stackexchange.com/questions/2317/latex-style-or-macro-for-detailed-response-to-referee-report.

