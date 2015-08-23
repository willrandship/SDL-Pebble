SDL 2.0 for the Pebble Smartwatch
---------------------------------
Ported by William Shipley, kept under the same license. (zlib)
For details read COPYING.txt.

BUILDING
--------
To build, open build-scripts/pebble and build with the pebble sdk, as follows:

    # pebble build

This will generate an SDL.a file, a static library. To use it
in your own applications, copy it and the contents of the include/ directory to <project src>/SDL/.

Include <SDL/SDL.h> as per the usual style. From there it is a
standard SDL environment, so existing applications should, to a certain
extent, just work.

Don't forget to statically link SDL.a in your build. Look at
wscript-example if you're using waf and don't know how.
