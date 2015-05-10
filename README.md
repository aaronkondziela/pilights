pilights
========

An automated home lighting control system that runs on a Raspberry Pi.
Created for personal use, and not nearly finished.

Usage
-----

You will need to set the GPIO pins in the command files appropriately
for your hardware setup. I'm using pins 19 and 20 on a model B+ board.
The older models don't have these pins on the header.

Depends on the RPi.GPIO Python package.

Notes
-----

The reason we've broken things out into many small files is twofold:

* First, to keep each file tiny and trivial to comprehend.
* Second, to have the rules implemented in way that reads like English when done up in bash.

TODO
----

Cleanup and installer makefile, if I feel like. Factor out some of the
larger and more repetitive scripts.

This started as a basic hack to automate the lighting controls. Under
development is a message bus system with rules engine, that can handle
more complex state transitions and cover all the various use cases
envisioned.

License
-------

Published under the MIT License. See LICENSE file.
