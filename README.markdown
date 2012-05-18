Bad Wolf for X11 resources
==========================

Colors for your .Xresources (or .Xdefaults, or whatever you have).

Basically these were made for rxvt, but they sould work for other stuff, like
xterm or something.

The colors are based (pertly snatched, really) from badwolf, a color scheme for
Vim pieced together by Steve Losh.

License
-------

As is original work by Steve, this thing is MIT/X11 licensed. Why would I want
to relicense it? I dunno.

Installation
------------

 * git clone git://github.com/dmedvinsky/badwolf.xdefaults
 * ln -s badwolf.xdefaults/xdefaults.colors ~/.Xdefaults.colors
 * vim ~/.Xdefaults

Add the following line somewhere:

    # include "/home/username/.Xdefaults.colors"

Don't forget to type your username in the path.

Sadly, I don't know the way to use variables in the `#include` directive. If
you know, tell me about it, please!

 * xrdb ~/.Xdefaults
 * vim ~/.xinitrc

Add the following line somewhere:

    xrdb -merge "${HOME}/.Xdefaults"
