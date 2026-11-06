# Сторонние компоненты и лицензии

Проект использует следующие сторонние библиотеки и ресурсы. Полные тексты
лицензий находятся в каталоге `LICENSES/` и в файле `assets/OpenSans-OFL.txt`
(в релизном архиве — `OpenSans-OFL.txt`).

## Краткая таблица

| Компонент | Лицензия | Где используется | Текст лицензии |
|---|---|---|---|
| cJSON | MIT | `source/vendor/cJSON.c`, `source/vendor/cJSON.h` | `LICENSES/cJSON.txt` |
| Open Sans | SIL Open Font License 1.1 | `assets/OpenSans-*.ttf`, `source/assets_font.h` | `assets/OpenSans-OFL.txt` |
| libctru | zlib | 3DS runtime / libctru | `LICENSES/libctru.txt` |
| citro2d | zlib | 2D-графика | `LICENSES/citro2d.txt` |
| citro3d | zlib | 3D-графика | `LICENSES/citro3d.txt` |
| libcurl | curl license (MIT-подобная) | `3ds-curl` | `LICENSES/libcurl.txt` |
| mbedTLS | Apache-2.0 (также доступна GPL-2.0-or-later) | `3ds-mbedtls` | `LICENSES/mbedTLS.txt` |
| zlib | zlib license | `3ds-zlib` | `LICENSES/zlib.txt` |
| devkitARM / newlib | BSD-подобные лицензии | toolchain | см. ссылки ниже |

## cJSON

- Copyright (c) 2009-2017 Dave Gamble and cJSON contributors.
- Лицензия: MIT.
- Используется для разбора JSON-ответов Lichess.
- Текст: `LICENSES/cJSON.txt`.
- Источник: https://github.com/DaveGamble/cJSON

## Open Sans

- Copyright 2020 The Open Sans Project Authors.
- Лицензия: SIL Open Font License 1.1.
- Используется для интерфейса и генерации `source/assets_font.h`.
- Текст: `assets/OpenSans-OFL.txt` (в релизном архиве — `OpenSans-OFL.txt`).
- Источник: https://github.com/googlefonts/opensans

## libctru

- Copyright (C) libctru contributors.
- Лицензия: zlib.
- Используется как основная библиотека 3DS homebrew.
- Текст: `LICENSES/libctru.txt`.
- Источник: https://github.com/devkitPro/libctru

## citro2d

- Copyright (C) 2017-2018 fincs.
- Лицензия: zlib.
- Используется для отрисовки интерфейса и доски.
- Текст: `LICENSES/citro2d.txt`.
- Источник: https://github.com/devkitPro/citro2d

## citro3d

- Copyright (C) 2014-2018 fincs.
- Лицензия: zlib.
- Используется как графический слой citro2d.
- Текст: `LICENSES/citro3d.txt`.
- Источник: https://github.com/devkitPro/citro3d

## libcurl

- Copyright (c) 1996-2023, Daniel Stenberg, <daniel@haxx.se>, and contributors.
- Лицензия: curl license (MIT-подобная).
- Используется для HTTP/HTTPS-запросов к Lichess Board API.
- Текст: `LICENSES/libcurl.txt`.
- Источник: https://curl.se/docs/copyright.html

## mbedTLS

- Copyright (C) ARM Limited and contributors.
- Лицензия: dual Apache-2.0 / GPL-2.0-or-later; в проекте используется Apache-2.0.
- Используется для TLS.
- Текст: `LICENSES/mbedTLS.txt`.
- Источник: https://github.com/Mbed-TLS/mbedtls

## zlib

- Copyright (C) 1995-2024 Jean-loup Gailly and Mark Adler.
- Лицензия: zlib license.
- Используется через `3ds-zlib`.
- Текст: `LICENSES/zlib.txt`.
- Источник: https://zlib.net/

## devkitARM / newlib

- devkitARM и newlib используются только для сборки; в бинарник попадают
  стандартная библиотека и runtime.
- newlib распространяется по BSD-подобным лицензиям.
- Ссылки: https://devkitpro.org/ , https://github.com/devkitPro/newlib

## Lichess Board API и Stockfish

- Lichess Board API используется как внешний сервис; код Lichess в проект не
  включён.
- Игра с компьютером выполняется на стороне Lichess через Stockfish; бинарник
  Stockfish в проект не включён.
- Lichess — товарный знак Lichess.org. Проект не связан с Lichess.org.
- Условия использования API: https://lichess.org/api

## Графические ресурсы

### `assets/pieces/*.png`

Источник и лицензия этих PNG в репозитории не задокументированы. **Перед
публикацией проверьте происхождение набора.** Если используется набор
cburnett, укажите автора Colin M.L. Burnett и лицензию CC BY-SA 3.0. Если
фигуры нарисованы вами — замените этот раздел на своё указание авторства и
лицензии.

### `icon.png` и `gfx/banner.png`

Иконка и баннер проекта. Если при их создании использовались сторонние
элементы, добавьте сюда источник и лицензию.

### `assets/banner_silence.wav`

Сгенерированный файл тишины для баннера CIA. Сторонних прав не содержит.

## Если вы распространяете сборки

Приложите к релизу:

- `LICENSE` — лицензия исходного кода проекта;
- `THIRD_PARTY_NOTICES.md` — этот файл;
- `LICENSES/` — тексты лицензий сторонних библиотек;
- `OpenSans-OFL.txt` — лицензия шрифта Open Sans (в исходниках —
  `assets/OpenSans-OFL.txt`).

Этот файл не является юридической консультацией. Перед публичным релизом
проверьте лицензии на все ассеты, которые вы добавляете в проект.
