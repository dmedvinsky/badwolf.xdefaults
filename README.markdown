Bad Wolf for X11 resources
==========================

Colors for your .Xresources (or .Xdefaults, or whatever you have).

Basically these were made for rxvt, but they should work for other stuff, like
xterm or something.

The colors are based (pertly snatched, really) on badwolf, a color scheme for
Vim pieced together by Steve Losh.

License
-------

As is original work by Steve, this thing is MIT/X11 licensed. Why would I want
to relicense it? I dunno.

Installation
------------

 * git clone git://github.com/dmedvinsky/badwolf.xdefaults.git

 * ln -s badwolf.xdefaults/xdefaults.colors ~/.Xdefaults.colors

 * vim ~/.Xdefaults

   Add the following line somewhere (change `username` to your login):

        # include "/home/username/.Xdefaults.colors"

   Sadly, I don't know the way to use variables in the `#include` directive. If
   you know, tell me please!

 * xrdb ~/.Xdefaults

If for some reason your resourses aren't loaded after starting X11, check if
you have the following line in your `~/.xinitrc`:

    xrdb -merge "${HOME}/.Xdefaults"
