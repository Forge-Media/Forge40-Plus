# Forge 40+

Follow-up project from my previous [Forge 303 Macropad](https://github.com/Forge-Media/ai03-macropad-pcb) project. The aim of this project is to design and manufacture a low-profile ortholinear grid Bluetooth Kailh Choc 40 percent keyboard, which actually works! The core module of the keyboard is a 40%, however, the Plus denotes that the design will deviate from a traditional 40%, with inspiration taken from the Worklouder creator-board, the design will thus include Rotary Encoder(s) and possibly an OLED (ZMK dependent).

## Core Project Requirements:

- 46 1U + 1 2U Kailh Choc Switches (Solder only due to plateless design)
- 1 Rotary Encoder (EC11 with Push Switch)
- USB-C support (AI03 duaghterboard)
- Bluetooth 5.0 Support
- MCU: Holyiot 18010 (Nordic nRF52840) (Manufacturer flashed with custom bootloader)
- Per-key RGB LED (47 LEDs)
- RGB Underglow (TBD LEDs)
- Support battery and charging (4.2V Lithium @ 100/500mA rate)
- ESD and Reverse Bias protection (Fused VCC and +3.3V)
- ZMK support
- 3D Printed (SLA) / CNC Polycarbonate base plate

### Future Project Requirements:

- Module PCBs with extra Switches & Rotary Encoders
- Expanded grid-system base plate

## CAD

KiCad 6.0 is used for the pcb design, based on:

- [ebastler's ZMK design guide](https://github.com/ebastler/zmk-designguide) | [Archived](https://web.archive.org/web/20210223222617/https://github.com/ebastler/zmk-designguide) | [Archived Mirror](https://imgur.com/D1a6lrI)
- [NiceNano V2 Schematics](https://nicekeyboards.com/docs/nice-nano/pinout-schematic)
- [ai03's guide](https://wiki.ai03.com/books/pcb-design)

**Required KiCad libraries:**

- [ai03's KiCad Type-C symbol](https://github.com/ai03-2725/Type-C.pretty) (HRO-TYPE-C-31-M-12 connector) [Git-Submodule]
- [marbastlib KiCad 6.x library](https://github.com/ebastler/marbastlib/tree/untested) (MCU, RGB LED and MX/Choc switches) [Git-Submodule]
- [Perigoso's KiCad 6.x footprints](https://github.com/perigoso/keyswitch-kicad-library) (MX and Choc switches) [**KiCad 6.0 Plugin**]

**Optional KiCad libraries:**

- [ebastler's kicad 5.x components](https://github.com/ebastler/kicad-keyboard-parts.pretty) (MCU and RGB LED footprints and 3D models) [Git-Submodule]
- [ai03's hybrid footprints](https://github.com/ai03-2725/MX_Alps_Hybrid/tree/master/Kailh_Choc.pretty) (Kailh Hotswap footprints) [Git-Submodule]
- [ai03's random components](https://github.com/ai03-2725/random-keyboard-parts.pretty) (Reset button footprint) [Git-Submodule]

Autocad, Rhino and Fusion 360 are used for the case design.

## References:

- [ebastler's ZMK design guide](https://github.com/ebastler/zmk-designguide)
- [ai03's - pcb guide](https://wiki.ai03.com/books/pcb-design)
- [ai03's KiCad library list](https://wiki.ai03.com/books/pcb-design/page/list-of-kicad-keyboard-parts-libraries)
- [33C Discord](https://discord.gg/6fHK4uk)
- [Keyboard Atelier Discord](https://discord.gg/b7vwhHS)
- [ZMC Docs](https://zmk.dev/docs/)
- (TBD)

## Notable required parts:

- [MCU Holyiot 18010](https://www.aliexpress.com/item/32868002366.html) (Provide holyiot with a bootloader .hex file on order)
- [Kailh Choc Switches V1](https://mechboards.co.uk/products/kailh-low-profile-choc-switches-v1-red)
- [Lithium battery](https://www.aliexpress.com/item/32826961711.html?spm=a2g0o.9042311.0.0.75d84c4dfswF9R) (at least 500mAh large, final supported dimensions TBD)
- [Backlight LEDs](https://lcsc.com/product-detail/Light-Emitting-Diodes-LED_TONYU-DY-S352818-RGBC-6812-2T_C524051.html)
- [Underglow LEDs](https://lcsc.com/product-detail/Light-Emitting-Diodes-LED_Worldsemi-WS2812B-Mini_C527089.html)

## License

MIT License

Copyright (c) 2022 ForgeMedia (Jeremy Paton)

Permission is hereby granted, free of charge, to any person obtaining a copy of this hardware, software, and associated documentation files (the "Product"), to deal in the Product without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Product, and to permit persons to whom the Product is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Product.

THE PRODUCT IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE PRODUCT OR THE USE OR OTHER DEALINGS IN THE PRODUCT.

## For the Keyboard Community

You can produce and sell this keyboard design. ForgeMedia (Jeremy Paton) is not liable. Creator attribution is required however, no use of the creator's or 3rd party branding may be utilised in a derivative. This includes logos and brand names.
