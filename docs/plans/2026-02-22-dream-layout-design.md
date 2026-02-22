# Totem Dream Layout Design

## Overview

5-layer Colemak-DH layout for a 38-key Totem split keyboard, optimised for dev work (VS Code, terminal, tmux), Salesforce (Apex/LWC), markdown writing, and Japanese input via romaji IME.

## Layers

| # | Layer | Access | Purpose |
|---|-------|--------|---------|
| 0 | BASE  | default | Colemak-DH + home row mods |
| 1 | NAV   | hold left middle thumb | Navigation, numbers, clipboard |
| 2 | SYM   | hold right middle thumb | Programming symbols, quotes, brackets, media |
| 3 | FN    | hold NAV + SYM together | F-keys, BT management, Japanese IME toggle |
| 4 | MOUSE | hold left outer thumb | Mouse movement + clicks |

## Layer 0: BASE - Colemak-DH + Home Row Mods

```
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |  Q  |  W  |  F  |  P  |  B  |   |  J  |  L  |  U  |  Y  |  ;  |
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             | # A | $ R | ^ S | & T |  G  |   |  M  | & N | ^ E | $ I | # O |
// +-----+-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
// | ESC |  Z  |  X  |  C  |  D  |  V  |   |  K  |  H  |  ,  |  .  |  /  |  \  |
// +-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
//                   | MSE | NAV |     |   |     | SYM |     |
//                   |BSPC | TAB | SPC |   | ENT | DEL |BSPC |
//                   +-----+-----+-----+   +-----+-----+-----+
```

Home row mods (# = GUI, $ = Alt, ^ = Ctrl, & = Shift):
- Left:  GUI(A), Alt(R), Ctrl(S), Shift(T)
- Right: Shift(N), Ctrl(E), Alt(I), GUI(O)

Thumb keys:
- Left outer: hold = MOUSE layer, tap = BSPC
- Left middle: hold = NAV layer, tap = TAB
- Left inner: SPC
- Right inner: ENTER
- Right middle: hold = SYM layer, tap = DEL
- Right outer: BSPC

Outer pinky keys:
- Left: ESC (dedicated, no layer needed)
- Right: \ (backslash, useful for dev paths and escaping)

## Layer 1: NAV - Navigation + Numbers (hold NAV/TAB)

```
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             | ESC |REDO |  UP |  =  |  `  |   |  ~  |  7  |  8  |  9  |  0  |
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |UNDO | LEFT| DOWN|RIGHT| TAB |   |  -  |  4  |  5  |  6  |  +  |
// +-----+-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
// |     | DEL | CUT |COPY |PASTE|     |   |  _  |  1  |  2  |  3  |  *  |     |
// +-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
//                   |     |#####|     |   | >FN |  0  |     |
//                   +-----+-----+-----+   +-----+-----+-----+
```

- Left hand: arrows on home row, undo/redo, clipboard (cut/copy/paste send Cmd+X/C/V macros)
- Right hand: number row layout (not numpad), arithmetic operators
- Backtick and tilde for dev (template literals, home dir, markdown code blocks)

## Layer 2: SYM - Symbols + Dev (hold SYM/DEL)

```
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |  !  |  @  |  #  |  $  |  %  |   |  ^  |  &  |  *  |  '  |  "  |
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |     |  |  |     |     |     |   |MUTE |  (  |  )  |  [  |  ]  |
// +-----+-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
// |     |     |     |     |     |     |   |VOL- |VOL+ |  {  |  }  |  \  |     |
// +-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
//                   |     | GIF | >FN |   |     |#####|     |
//                   +-----+-----+-----+   +-----+-----+-----+
```

- Left hand: shifted number symbols !@#$%, pipe
- Right hand: all bracket types grouped logically - () home, [] above, {} below
- Quotes on right top for easy string/markdown access
- Media controls: mute, volume, play/pause (on GIF macro position - can keep or replace)

## Layer 3: FN - F-Keys + Board + IME (hold NAV + SYM)

```
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |RESET|BTCLR|OUTTG|     |JPIME|   |     | F7  | F8  | F9  | F12 |
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |BOOT |BTNXT|     |     |     |   |     | F4  | F5  | F6  | F11 |
// +-----+-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
// |     |     |BTPRV|     |     |     |   |PREV |NEXT | F1  | F2  | F3  | F10 |
// +-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
//                   |     |#####|     |   |PLAY |#####|     |
//                   +-----+-----+-----+   +-----+-----+-----+
```

- Left hand: board management (BT clear/next/prev, output toggle, reset, bootloader)
- Right hand: F-keys in grid layout
- JP IME: sends Ctrl+Space to toggle macOS Japanese input source
- Media: prev/next track, play/pause on thumbs

## Layer 4: MOUSE - Mouse Keys (hold MSE/BSPC)

```
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |     |     |     |     |     |   |     |     |MS UP|     |     |
//             +-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
//             |     |     |     |     |     |   |     |MS LT|MS DN|MS RT|     |
// +-----+-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
// |     |     |     |     |     |     |   |     |LCLK |RCLK |MCLK |     |     |
// +-----+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+-----+
//                   |#####|     |     |   |LCLK |RCLK |     |
//                   +-----+-----+-----+   +-----+-----+-----+
```

- Right hand: mouse movement on home row (NEI = Left/Down/Right, U = Up)
- Click buttons directly below movement keys (L/R/M click)
- Thumb L/R click as backup
- Left thumb holds layer, right hand does everything

## Combos

| Keys | Action | Notes |
|------|--------|-------|
| Q + W | ESC | Existing combo (keep as backup, ESC also on outer pinky) |
| S + T | Ctrl+A | Tmux prefix - press both together or hold Ctrl(S) tap T |

## Tmux Setup

Recommended `.tmux.conf`:
```
set -g prefix C-a
unbind C-b
bind C-a send-prefix
```

With home row mods, Ctrl+A = hold S (Ctrl) + tap A. Adjacent fingers, very ergonomic.

## Japanese Input

Uses macOS romaji input method. The JP IME key on the FN layer sends Ctrl+Space to toggle between English and Japanese input sources. Type in romaji and macOS converts to hiragana/katakana/kanji.

## ZMK Features Required

- `&mt` (mod-tap) for home row mods
- `&lt` (layer-tap) for thumb layer keys
- `&kp` for standard keys
- `&mkp` and mouse movement keys for MOUSE layer (requires ZMK mouse keys support)
- Macros for: clipboard shortcuts (Cmd+Z/X/C/V), JP IME toggle, GIF, tmux prefix combo

## Future Considerations

### One-handed mirror layer
A mirror layer that flips the right half onto the left hand (or vice versa) for one-handed typing while using an external mouse. Would require a 6th layer. Save for a future iteration once the 5-layer setup is proven.

### Code macros
Arrow `=>`, `->`, `::`, `&&`, `||` as macros on the SYM layer blank spots. Add once actual pain points are identified through daily use.

### Home row mod tuning
The `&mt` behaviour may need tuning:
- `tapping-term-ms`: currently 170ms, may need adjustment
- `quick-tap-ms`: currently 100ms
- `flavor`: currently tap-preferred, balanced may work better
- `global-quick-tap`: helps prevent misfires during fast typing
