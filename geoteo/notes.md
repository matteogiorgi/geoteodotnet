# Computability notes

I know there is a vast bibliography on the subject but I just wanted to write something intuitive and easy to read on such essential and extensive topic for a computer scientist.

The notes are written in italian and follow professor [P. Degano](http://pages.di.unipi.it/degano/) lectures at [B.Sc. Computer Science](https://didattica.di.unipi.it/en/undergraduate-programme-in-computer-science/) University of Pisa. The source code can be compiled using R with [Rmarkdown](https://cran.r-project.org/web/packages/rmarkdown/index.html) package, just use these teeny-tiny Rscript:

~~~ r
#! /usr/bin/env Rscript
require(rmarkdown)
render(commandArgs(trailingOnly=TRUE))
~~~

You can take a look and download the notes [here](https://matteogiorgi.github.io/computability/src/notes.pdf) or in the window below. Unfortunately there won't be any updates soon, anyhow it was quite fun to play with LaTeX templates and the Rmarkdown package.

<!-- ![](https://matteogiorgi.github.io/computability/src/notes.pdf){ width=100% height=600px } -->

<object data="https://matteogiorgi.github.io/computability/src/notes.pdf" type="application/pdf" width="100%" height="600px">
<p style="color: #bfbfbf; background-color: #2e2f3e; margin: 0; padding-left: 2em; padding-right: 2em; padding-top: 0.5em; padding-bottom: 0.5em; border-left: 0.5em #44475a solid; font-style: italic;">
  <a href="https://matteogiorgi.github.io/computability/src/notes.pdf" title="Download PDF"><img src="pics/extraction.png" /></a>
  <b>No PDF support, click above and download the thing.</b>
</p>
</object>

---

To tell the the all truth, this little project had a second purpose: create a $\LaTeX$ template to write reports/articles in markdown (so to be humanly readable even just through the source code), where I could easily edit every single chapter separately and maintain the code neat and clean.

But there's more: I find [literate programming](http://literateprogramming.com) very useful and I've played with tools like [Wolfram Mathematica](https://www.wolfram.com/mathematica), [Jupyter Notebook](https://jupyter.org) and [Org Mode](https://orgmode.org) in particular; needless to say I wanted to have something like this in my new template. Lucky me R has the [Knitr](https://yihui.org/knitr/) package that enables integration of R code into LaTeX, HTML and Markdown. Short story short, every block of code (no matter the language) is evalueted in the order it appears in the document and the shell output is printed just below each block.

One great advantage of this, is the possibility to display graphs and diagrams inside the document just by writing chunks of code that can output them.
