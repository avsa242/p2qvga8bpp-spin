# p2qvga8bpp-spin
-----------------

This is a P2X8C4M64P/Propeller 2 VGA (QVGA 320x200, 8bpp) display engine.

**IMPORTANT**: This software is meant to be used with the [p2-spin-standard-library](https://github.com/avsa242/p2-spin-standard-library) (P2X8C4M64P). Please install the library first before attempting to use this code, otherwise you will be missing several files required to build the project.

## Salient Features

* QVGA 320x200 resolution (signalled as 640x480)
* Integration with generic bitmap graphics library
* Optional double-buffering
* Optional wait for VSync signal
* Includes simple video timing adjustment utility

## Requirements

P2/SPIN2:
* p2-spin-standard-library

## Compiler Compatibility

* P2/SPIN2: FastSpin (tested with 4.2.3-beta)
* ~~Propeller Tool~~ (incompatible - no preprocessor)
* ~~PNut~~ (incompatible - no preprocessor)

## Limitations

* Very early in development - may malfunction, or outright fail to build
* P2 Clock frequency must be defined in the driver, and be equivalent to that defined in the top-level application

## TODO

- [ ] Make streamer frequency setting adjustable at runtime
