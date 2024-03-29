# p2qvga8bpp-spin
-----------------

This is a P2X8C4M64P/Propeller 2 QVGA display engine.

**IMPORTANT**: This software is meant to be used with the [p2-spin-standard-library](https://github.com/avsa242/p2-spin-standard-library) (P2X8C4M64P). Please install the library first before attempting to use this code, otherwise you will be missing several files required to build the project.

## Salient Features

* QVGA 320x240 resolution (signalled as 640x480, with pixel-doubling), 8bpp color
* Integration with generic bitmap graphics library
* Double-buffering (optional)
* Wait for vsync, or current vsync status (function calls)
* Display intensity
* Includes simple video timing adjustment utility


## Requirements

P2/SPIN2:
* p2-spin-standard-library
* 1 extra core/cog for the PASM engine
* 76.8kBytes RAM for single-buffered display, or 153.6kBytes for double-buffered
* graphics.common.spin2h (provided by p2-spin-standard-library)


## Compiler Compatibility

| Processor | Language | Compiler               | Backend      | Status                |
|-----------|----------|------------------------|--------------|-----------------------|
| P2        | SPIN2    | FlexSpin (6.5.0)       | NuCode       | FTBFS                 |
| P2        | SPIN2    | FlexSpin (6.5.0)       | Native/PASM2 | OK                    |

(other versions or toolchains not listed are __not supported__, and _may or may not_ work)


## Limitations

* Changing the palette array while the driver is running has no effect - it must be restarted to take effect

