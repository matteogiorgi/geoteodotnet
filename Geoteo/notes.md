<nav class="site-nav" style="font-weight:bold; padding-bottom:1em; border-bottom:1px solid #d0d0cc">
  Computability notes: an attempt
  <div style="float:right">
  <a href="javascript:history.back()" style="color:black; float:right">&crarr;</a>
  </div>
</nav>


I know there is a vast bibliography on the subject but I just wanted to write something intuitive and easy to read on such essential and extensive topic for a computer scientist.

The notes are written in italian and follow professor [P. Degano](http://pages.di.unipi.it/degano/) lectures at [B.Sc. Computer Science](https://didattica.di.unipi.it/en/undergraduate-programme-in-computer-science/) University of Pisa. The source code can be compiled using R with [Rmarkdown](https://cran.r-project.org/web/packages/rmarkdown/index.html) package, just use these teeny-tiny Rscript:

~~~ r
#! /usr/bin/env Rscript
require(rmarkdown)
render(commandArgs(trailingOnly=TRUE))
~~~

You can take a look and download the notes [here](https://matteogiorgi.github.io/computability/src/notes.pdf) or in the window below. Unfortunately there won't be any updates soon, anyhow it was quite fun to play with $\LaTeX$ templates and the Rmarkdown package.

<object data="https://matteogiorgi.github.io/computability/src/notes.pdf" type="application/pdf" width="100%" height="600px">
<p style="font-size:10px; color:#d0d0cc; text-align:center; border:1px solid #d0d0cc;">
  <img width=60% style="padding:30px;" src="pics/extraction.png">\
  No PDF support, <a style="color:#d0d0cc; text-decoration:underline" href="https://matteogiorgi.github.io/computability/src/notes.pdf" title="Download PDF">click clack</a> and download the thing.
</p>
</object>

To tell the the all truth, this little project had a second purpose too: create a $\LaTeX$ template to write reports/articles in markdown (so to be humanly readable even just through the source code), where I could easily edit every single chapter separately while maintaining the code neat and clean.

But there's more: I find [literate programming](http://literateprogramming.com) very useful and I've played with tools like [Wolfram Mathematica](https://www.wolfram.com/mathematica), [Jupyter Notebook](https://jupyter.org) and the magnificent Emacs mode [Org Mode](https://orgmode.org); needless to say I wanted to have something like this in my new template. Lucky me R has the [Knitr](https://yihui.org/knitr/) package that enables integration of R code into $\LaTeX$, HTML and Markdown. Short story short, every block of code (no matter the language) is evalueted in the order it appears in the document and the shell output is printed just below each block.

One great advantage of this, is the possibility to display graphs and diagrams inside the document just by writing chunks of code that can output them.
