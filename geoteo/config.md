# Arch ([btw](https://iusearchbtw.lol)) workflow

I've used [Qtile](http://www.qtile.org) for a while now and it's a good window manager; it has its source code and config file written in Python, plus a neat [documentation](http://docs.qtile.org/en/latest) comes in support if you fancy to play with it. The only problem imo is stability: in [more than one occasion](https://github.com/qtile/qtile/issues) I had to deal with issues appearing just because of last update.

So I decided to change and I knew exactly what I want: my new window manager has to be dynamic (just like with Qtile I do not want to deal with window repositioning), must have an inegrated bar and a usable default config (I didn't have much time for tinkering), plus It would be great if it had good documentation too.

The choice narrowed to [dwm](https://dwm.suckless.org), [Xmonad](https://xmonad.org), [Awesome](https://awesomewm.org) and the latter seems perfect for the job: I am no Lua programmer but with very little effort the wm is configured and it flies.

![](pics/scrot_1.png){ width=100% }

![](pics/scrot_2.png){ width=100% }

To have a rough idea on how it works, browse through my [dotfiles](https://github.com/matteogiorgi/.dotfiles) or just take a look at the sample above.
