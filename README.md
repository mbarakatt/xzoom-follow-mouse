# xzoom with mouse follow feature
This is a fork of the xzoom program.
I quickly patched the feature to follow the mouse and made it the default behaviour.
Works great with a window manager.

# To build
```bash
xmkmf # provided by the imake package of arch-linux
make
```

# Sources:
xzoom from: http://webdiis.unizar.es/pub/unix/X11/xzoom-0.3.tgz
Applied the follow patch: ftp://ftp.acc.umu.se/mirror/cdimage/snapshot/Debian/pool/main/x/xzoom/xzoom_0.3-23.diff.gz

To do this I read the pkgbuild file here: https://aur.archlinux.org/packages/xzoom/

# License
Refence to the original license contained in : http://webdiis.unizar.es/pub/unix/X11/xzoom-0.3.tgz

# The following is the original readme:
This is xzoom 0.3.

I got a few letters from people who tried xzoom-0.1.
I want to thank all these people for the responses.
Some people have requested to add features. Some
also suggested their own contribution.
I am sory that I could not satisfy all. I will try
to do so in the next releases.

What's changed since release 0.1:

Mainly I added command line options. With these
you can start xzoom and focus at any point in the screen
and at any magnification which you want. Look at the
man page for details.

A second thing that you might have noticed is a memory
leak in 0.1 (funny, I did not get any mail about it).
As I finally found, the leak was due to some X events queing
up and not discarded. Finally I found the documentation
for XSHM in the X11R6 CDROM (disk 2, file
distrib/xc/doc/specs/Xext/mit-shm.ms). The MS macros
came from the BSD cdrom and with that help I could
find the bug and fix it.

Plese send comments, requests, suggestions to
nahshon@best.com.

Itai Nahshon
