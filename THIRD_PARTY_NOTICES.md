# Third-Party Notices

This project uses the following third-party libraries and assets. Full license
texts are in `LICENSES/` and in `assets/OpenSans-OFL.txt` (in release archives,
`OpenSans-OFL.txt`).

## Summary

| Component | License | Used for | License text |
|---|---|---|---|
| cJSON | MIT | `source/vendor/cJSON.c`, `source/vendor/cJSON.h` | `LICENSES/cJSON.txt` |
| Open Sans | SIL Open Font License 1.1 | `assets/OpenSans-*.ttf`, `source/assets_font.h` | `assets/OpenSans-OFL.txt` |
| cburnett chess pieces | BSD 3-Clause | `assets/pieces/*.png`, `gfx/pieces.t3x` | `LICENSES/cburnett-BSD-3-Clause.txt` |
| libctru | zlib | 3DS runtime / libctru | `LICENSES/libctru.txt` |
| citro2d | zlib | 2D graphics | `LICENSES/citro2d.txt` |
| citro3d | zlib | 3D graphics | `LICENSES/citro3d.txt` |
| libcurl | curl license (MIT-like) | `3ds-curl` | `LICENSES/libcurl.txt` |
| mbedTLS | Apache-2.0 (also available under GPL-2.0-or-later) | `3ds-mbedtls` | `LICENSES/mbedTLS.txt` |
| zlib | zlib license | `3ds-zlib` | `LICENSES/zlib.txt` |
| devkitARM / newlib | BSD-style licenses | toolchain | see links below |

## cJSON

- Copyright (c) 2009-2017 Dave Gamble and cJSON contributors.
- License: MIT.
- Used for parsing Lichess JSON responses.
- Text: `LICENSES/cJSON.txt`.
- Source: https://github.com/DaveGamble/cJSON

## Open Sans

- Copyright 2020 The Open Sans Project Authors.
- License: SIL Open Font License 1.1.
- Used for the UI and for generating `source/assets_font.h`.
- Text: `assets/OpenSans-OFL.txt` (in release archives, `OpenSans-OFL.txt`).
- Source: https://github.com/googlefonts/opensans

## cburnett Chess Pieces

- Creator: Colin M.L. Burnett (User:Cburnett).
- Source: the standard transparent SVG chess pieces on Wikimedia Commons, for
  example https://commons.wikimedia.org/wiki/File:Chess_klt45.svg and the
  eleven sibling files (`Chess_{k,q,r,b,n,p}{l,d}t45.svg`).
- Also distributed in the Lichess repository:
  https://github.com/lichess-org/lila/tree/master/public/piece/cburnett
- License: BSD 3-Clause. The author also offers the artwork under GFDL 1.2+,
  CC BY-SA 3.0, and GPL 2+; this project uses the BSD 3-Clause option.
- Changes: the SVG artwork was rendered to PNG, scaled to 250×250, and packed
  into `gfx/pieces.t3x` / `source/assets_pieces.h` for this project.
- Text: `LICENSES/cburnett-BSD-3-Clause.txt`.

## libctru

- Copyright (C) libctru contributors.
- License: zlib.
- Used as the main 3DS homebrew library.
- Text: `LICENSES/libctru.txt`.
- Source: https://github.com/devkitPro/libctru

## citro2d

- Copyright (C) 2017-2018 fincs.
- License: zlib.
- Used for rendering the UI and the board.
- Text: `LICENSES/citro2d.txt`.
- Source: https://github.com/devkitPro/citro2d

## citro3d

- Copyright (C) 2014-2018 fincs.
- License: zlib.
- Used as the graphics layer beneath citro2d.
- Text: `LICENSES/citro3d.txt`.
- Source: https://github.com/devkitPro/citro3d

## libcurl

- Copyright (c) 1996-2023, Daniel Stenberg, <daniel@haxx.se>, and contributors.
- License: curl license (MIT-like).
- Used for HTTP/HTTPS requests to the Lichess Board API.
- Text: `LICENSES/libcurl.txt`.
- Source: https://curl.se/docs/copyright.html

## mbedTLS

- Copyright (C) ARM Limited and contributors.
- License: dual Apache-2.0 / GPL-2.0-or-later; this project uses Apache-2.0.
- Used for TLS.
- Text: `LICENSES/mbedTLS.txt`.
- Source: https://github.com/Mbed-TLS/mbedtls

## zlib

- Copyright (C) 1995-2024 Jean-loup Gailly and Mark Adler.
- License: zlib license.
- Used through `3ds-zlib`.
- Text: `LICENSES/zlib.txt`.
- Source: https://zlib.net/

## devkitARM / newlib

- devkitARM and newlib are used only for building; the binary includes the
  standard library and runtime.
- newlib is distributed under BSD-style licenses.
- Links: https://devkitpro.org/ , https://github.com/devkitPro/newlib

## Lichess Board API and Stockfish

- The Lichess Board API is used as an external service; no Lichess source code
  is included in this project.
- Computer games are played through Stockfish on the Lichess side; no Stockfish
  binary is included in this project.
- Lichess is a trademark of Lichess.org. This project is not affiliated with
  Lichess.org.
- API terms: https://lichess.org/api

## Other Assets

### `icon.png` and `gfx/banner.png`

Original project icon and banner. If third-party elements were used to create
them, add the source and license here.

### `assets/banner_silence.wav`

Generated silence used for the CIA banner. It contains no third-party material.

## Redistribution Checklist

When distributing builds, include:

- `LICENSE` — the project source-code license;
- `THIRD_PARTY_NOTICES.md` — this file;
- `LICENSES/` — third-party license texts;
- `OpenSans-OFL.txt` — the Open Sans license (in the source tree,
  `assets/OpenSans-OFL.txt`).

This file is not legal advice. Before a public release, verify the licenses of
all assets added to the project.
