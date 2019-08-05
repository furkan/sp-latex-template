# sp-latex-template

This is a LaTeX template for METU EEE Summer Practice reports.

I advise using [Overleaf](https://www.overleaf.com/read/gymnzgjmzzwh) instead of running locally.

After copying the project on Overleaf, just change what's inside the `document` folder. You do not need to engage with the `main.tex` file or the `config` folder.

Enjoy... (Despise less)

## Short Tutorial

[Adding Chapters](#adding-chapters)

[Adding Sections](#adding-sections)

[Adding Figures](#adding-figures)

[Referencing Figures](#referencing-figures)

[Citations](#citations)

#### Adding Chapters

* To add a new chapter called `My Experience`, in the `documents/content` folder, create a new file called `myexperience.tex` (or whatever) and make its first line `\chapter{MY EXPERIENCE}`.

* In the file `documents/content.tex`, add a line that calls this chapter: `\input{document/content/introduction.tex}`. (Note that the order of the lines in this file is important, as that is the same order with which they will show up on the document.)

#### Adding Sections

* See [document/company.tex](https://github.com/furkan/sp-latex-template/blob/master/document/content/company.tex)

#### Adding Figures

```
\begin{figure}[tb]
\centering
\includegraphics[width = 0.4\hsize]{document/figures/odtu_logo.png}
\caption{Caption will be here.}
\label{fig:logo}
\end{figure}
```

* Label is important if you plan on referencing the figure later.

#### Referencing Figures

```
Figure~\ref{fig:logo} is an example of a figure.
```


#### Citations

* Work in progress...
