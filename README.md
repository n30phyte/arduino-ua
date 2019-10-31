# arduino-ua

A modified version of arduino-ua for CMPUT 274/275 that works better ~~with Fedora~~ in general.

## Changes / Fixes

- Added /dev/ttyUSB* detection into port select
  - Cheap Chinese arduino compatibility (CH34XX instead of the usual FTDI serial interface)
- Made makefile actually use selected port
- Fixed problems when using newer Arduino IDE version
- Make sure that code gets compiled with gnu++98, following older version bundled in 18.04.
- Fix minicom not unlocking ports
- Deleted old unused files

## Credits

- Arduino IDE version detection from [sudar/Arduino-Makefile](https://www.github.com/sudar/Arduino-Makefile)