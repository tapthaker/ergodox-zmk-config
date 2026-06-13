# SliceMK ErgoDox Keymap Layout

This document mirrors `config/slicemk_ergodox.keymap`. Keep it up to date whenever the keymap changes.

## Layers

| Layer | Name | Purpose |
|---:|---|---|
| 0 | `LAYER_MAIN` | Main typing layer |
| 1 | `LAYER_NAV` | Navigation, zoom, volume, screenshot |
| 2 | `LAYER_BLUETOOTH` | Bluetooth and output switching |
| 3 | `LAYER_MOUSE` | Mouse movement, clicks, and scroll |

## Layer 0 — Main

```text
                         [SYS_OFF]

Left hand                                      Right hand
`       1      2      3      4      5  none    none    6      7      8      9      0      [
Tab     Q      W      E      R      T  none    (       Y      U      I      O      P      ]
Ctl/Esc A      S      D      F      G                  H      J      K      L      ;      '
Shift   Z      X      C      V      B  NAV     )       N      M      ,      .      /      -
Ctrl    GUI    Alt    none   none                       none   +      |      \      =

Thumbs / center:
Left:  MOUSE, none, none, none, none, Backspace
Right: none, none, BLUETOOTH, Esc then :, Enter, Space
```

Notes:

- `Ctl/Esc` is `&mt LEFT_CONTROL ESCAPE`: hold for Control, tap for Escape.
- `Esc then :` is the `m_esc_colon` macro.
- `NAV`, `BLUETOOTH`, and `MOUSE` are momentary layer keys.

## Layer 1 — Nav

```text
                         [SYS_OFF]

Left hand                                      Right hand
none    none   none   none   none   none none    PrintScr none   none   none   none   none   VolUp
none    none   none   none   none   none none    none     Home   none   none   End    LG+    VolDn
none    none   none   none   none   none                 Left   Down   Up     Right  LG-    PgUp
none    none   none   none   none   none none    none     none   none   none   none   none   PgDn
none    none   none   none   none                      none     none   none   none   none
```

Important shortcuts:

- `Nav + right-hand top-left` → Print Screen
- `Nav + P` → `LG(PLUS)` / Super-Plus / Command-Plus
- `Nav + ;` → `LG(MINUS)` / Super-Minus / Command-Minus
- `Nav + '` → Page Up
- `Nav + -` → Page Down
- Arrow cluster is on the right home-row area.
- Home/End are on the right hand.
- Volume Up/Down are on the far right.

## Layer 2 — Bluetooth

```text
                         [SYS_OFF]

Left hand useful bindings:
OUT_BLE, BT_SEL 0, BT_SEL 1, BT_SEL 3, BT_SEL 4
OUT_USB

Bottom right:
BT_CLR
```

## Layer 3 — Mouse

```text
                         [SYS_OFF]

Right hand useful bindings:
Scroll Up / Scroll Down on the far-right top keys
Mouse movement: Left, Down, Up, Right
Mouse buttons: Left Click, Right Click
```
