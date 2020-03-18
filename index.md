<img align="right" width="160" src="assets/images/alien.gif">

<section id="beep">
</section>

# Beep-boop

Here you go folks, I'm the alien living in [Matteo](https://github.com/MatteoGiorgi)'s head and this is my `main`. Do you want to know something more? Click [this](https://nbviewer.jupyter.org/github/MatteoGiorgi/cv/blob/master/src/cv.pdf) or [that](https://nbviewer.jupyter.org/github/MatteoGiorgi/cv/blob/master/src/cv.pdf).




<section id="notes">
</section>

# Computability notes 📌

I know there is a vast bibliography on the subject but I just wanted to write [something](https://github.com/MatteoGiorgi/computability_notes) intuitive and easy to read on such essential and extensive topic for a computer scientist.

The [notes](https://nbviewer.jupyter.org/github/MatteoGiorgi/computability_notes/blob/master/src/notes.pdf) are written in italian and follow professor [P. Degano](http://pages.di.unipi.it/degano/) lectures at [B.Sc. Computer Science](https://didattica.di.unipi.it/en/undergraduate-programme-in-computer-science/) University of Pisa. The source code can be compiled using R with [*Rmarkdown*](https://cran.r-project.org/web/packages/rmarkdown/index.html) package, just use this tiny bash script below.

```bash
echo "require(rmarkdown); render('$1')" | R --vanilla
```

<p align="center">
  <img width="500" src="assets/images/candy.png"/>
</p>




<section id="attack">
</section>

# Wiener attack

[Here](https://github.com/MatteoGiorgi/wiener_attack) I wrote a brief [paper](https://nbviewer.jupyter.org/github/MatteoGiorgi/wiener_attack/blob/master/src/wiener_attack.pdf) regarding RSA protocol and the attack M.J. Wiener published in 1990. I tried to create a self-contained work, emphasising the power of playing with [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) using *Legendre theorem*.

A simple implementation is included in the end using few lines of [*Wolfram Language*](https://www.wolfram.com/language/). Below there is an example of the *classic attack*.

```mathematica
e = 7502876735617; n = 28562942440499;
fc = ContinuedFraction[e/n];
cList = Convergents[fc];
phiList = Floor[e/Rest[cList]];

check[phi_] := (x/.p) /; (Mod[n,x] /. (p=Solve[x^2-(n-phi+1)x+n==0,x])) == {0, 0};
checkL[phi_List] := Flatten[Cases[check /@ phi,_List]];

primes = Flatten[checkL /@ (phiList-m /. {m->#}& /@ Range[0,9])];
```




<section id="config">
</section>

# My GNU/Linux config

I recently switched to [Qtile](http://www.qtile.org/) from good old [i3](https://i3wm.org/) and I felt right at home. Qtile has its source code and config file written in python, plus a neat [documentation](http://docs.qtile.org/en/latest) comes in support if you fancy to play with it.

You can browse through my [dotfiles](https://github.com/MatteoGiorgi/dotfiles) or just take a look at my workflow, there is a sample below.

<p align="center">
  <img width="500" src="assets/images/qtile.gif"/>
</p>




<section id="asteroids">
</section>

# Asteroids++

Remember [Asteroids](https://en.wikipedia.org/wiki/Asteroids_%28video_game%29), the one all the cool kids used to play with? The original, released by Atari in 1979, was implemented by Rains, Logg, and Walsh on hardware developed by Delman and was a vector game, in which the graphics were composed of lines drawn on a vector monitor.

[This](https://github.com/MatteoGiorgi/asteroids_plus_plus) one is a replica (with few additions) and it is written in JavaScript using [P5.js](https://p5js.org/) libraries; feel free to play using `w`, `a`, `d` to move around and `spc`, `m` to fire and drop bombs. [Enjoy](https://matteogiorgi.github.io/asteroids_plus_plus/src)!




<img align="right" width="160" src="assets/images/run.gif">

<section id="oldies">
</section>

# Old gear

I got some old uni projects waiting to be reorganized but don't worry, I'll take care of them one day or another. Still, you can find them [here](https://github.com/MatteoGiorgi/interprete_funzionale), [there](https://github.com/MatteoGiorgi/graph), [beer](https://github.com/MatteoGiorgi/membox) and [bear](https://github.com/MatteoGiorgi/sparse).

