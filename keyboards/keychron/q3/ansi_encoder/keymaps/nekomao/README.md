# NekoMaO's Keychron Q3 keymap v1.0.0
Big thanks elpekeñin#2234 for staying around, teaching me and helping me in making this.

Thanks to QMK discord server people too! awesome peeps like filterpaper#2878 , waffle#0087, and ANDY#1129

## Difference between stock (Note : VIA is enabled)
- Added 1 additional FN layer which can be accessible by `MO(4)`. (`XTD_FN` Layer = `MO(4)`)
  - By default `RGUI`/`ROPT` has been replaced with `MO(4)`, please modify if it doesn't fit your use case. 
- Enabling `CapsLock` will turn Alpha, Number, and Symbols LED red.
  - Capslock Indicator behavior is only on base layer.(`MAC_BASE` and `WIN_BASE`)
- Keys that are assigned in FN layers will glow in color, when FN key is pressed.
  - `MAC_FN` and `WIN_FN` assigned keys LED is `GREEN`.
  - `XTD_FN` assigned keys LED is `CYAN`.
- GUI/Option Lock toggle key combination is `FN+LGUI` in windows or `FN+LOPT` in mac.[^1] Can be relocated with VIA[^2]
- GUI LED indicator would glow `GOLD` color when lock is enabled.
- FN Layer `XTD_FN` F1-F12 replaced with F13-F24
- FN Layer `WIN_FN` has mouse controls.(Windows)
  - `FN+UP` Mouse cursor up
  - `FN+DOWN` Mouse cursor down
  - `FN+LEFT` Mouse cursor left
  - `FN+RIGHT` Mouse cursor right
  - `FN+INS` Mouse Left click
  - `FN+HOME` Mouse right click
  - `FN+DEL` Mouse back button
  - `FN+END` Mouse forward button
  - `FN` + `Knob` counter clockwise send numpad `-` and clockwise sends numpad `+`
    - it serves as a `Zoom In/Out` function. Hold `FN+RIGHT CTRL` + Knob movement, if zoom doesn't seem to work.[^3]

[^1]: dont be alarmed when you see raw hexcode `0x700B` in VIA, it is GUI_TOG function.
[^2]: if you wished to change the hotkey location in VIA, do take note that VIA dont have a dedicated button/unfunction for `GUI_TOG`, you will need to use `ANY` in `SPECIAL` and input hexcode `0x700B` for GUI_TOG.
[^3]: i've decided to not use `C(KC_PMNS)` and `C(KC_PPLS)`, just incase we encounter any applications that doesn't use modifier `CTRL` + Hotkey for zoom function.

### 30-December-2022 v1.0.0
- Initial release

Feature
