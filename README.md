# p2qvga8bpp-spin
-----------------

This is a P2X8C4M64P/Propeller 2 QVGA display engine.

**IMPORTANT**: This software is meant to be used with the [p2-spin-standard-library](https://github.com/avsa242/p2-spin-standard-library) (P2X8C4M64P). Please install the library first before attempting to use this code, otherwise you will be missing several files required to build the project.

## Salient Features

* QVGA 320x240 resolution (signalled as 640x480, with pixel-doubling), 8bpp color
* Integration with generic bitmap graphics library
* Optional double-buffering
* Optional wait for VSync signal
* Includes simple video timing adjustment utility

## Requirements

P2/SPIN2:
* p2-spin-standard-library
* 1 extra core/cog for the PASM engine
* 76.8kBytes RAM for single-buffered display, or 153.6kBytes for double-buffered
* graphics.common.spin2h (provided by p2-spin-standard-library)

## Compiler Compatibility

| Processor | Language | Compiler               | Backend     | Status                |
|-----------|----------|------------------------|-------------|-----------------------|
| P1        | SPIN1    | FlexSpin (5.9.14-beta) | Bytecode    | Unsupported           |
| P1        | SPIN1    | FlexSpin (5.9.14-beta) | Native code | Unsupported           |
| P1        | SPIN1    | OpenSpin (1.00.81)     | Bytecode    | Unsupported           |
| P2        | SPIN2    | FlexSpin (5.9.14-beta) | NuCode      | Untested              |
| P2        | SPIN2    | FlexSpin (5.9.14-beta) | Native code | OK                    |
| P1        | SPIN1    | Brad's Spin Tool (any) | Bytecode    | Unsupported           |
| P1, P2    | SPIN1, 2 | Propeller Tool (any)   | Bytecode    | Unsupported           |
| P1, P2    | SPIN1, 2 | PNut (any)             | Bytecode    | Unsupported           |

## Limitations

* TBD

