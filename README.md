# Minimal Glove80 Dvorak Layout

Personal minimal Glove80 layout, version 2. Dvorak, plain Dvorak, QWERTY, Number, Symbol, Function, Emoji, Utility, and Magic are user-facing; eight technical layers implement typing-aware home-row mods. Hold Magic and press its QWERTY or Dvorak key to toggle that plain, home-row-mod-free typing mode. F1-F12 span the top row, with F1 and F12 on the outer edges of the number row. Hold either Delete or right Enter for Symbol; taps remain Delete and Enter. While either key holds Symbol, hold the opposite key for Shift, with either order supported. Symbol preserves the right layout while copying hard number-row, outer-column, and thumb symbols into the left inner area, and puts Win, Alt, Ctrl, and Shift on unused left-side keys in the last row without replacing symbols. The upper-left thumb provides Shift. Tap the upper-middle left-thumb key for Esc or hold it for Number. Hold the upper-right left-thumb key for Function; that layer contains Glorious Engrammer's right-side F1-F15 arrangement plus Win, Alt, Ctrl, and Shift on the left home row, with every other key disabled. Hold Tab for Utility; tap remains Tab. Utility provides Print Screen, clipboard, undo/redo, context-menu, brightness, volume, and track controls on the left hand. Hold the left-thumb Emoji key, or tap it for Word Shift (ZMK Caps Word); Emoji copies Glorious Engrammer's mapping, presets, shifted variants, toggle, and ZWJ.

[`keymap.json`](keymap.json)

## Symbol layer

Tap left Delete or right Enter normally. Hold either key to activate Symbol. While Symbol is active, hold the opposite activation key for Shift; either press order works. Keep the operating-system layout set to English (US), because symbols such as `(` and `{` use shifted US keycodes.

Right-hand symbol block follows Glorious Engrammer/TailorKey design. Placement encodes common programming rolls and Vim/Neovim command grammar, not arbitrary character grouping:

| Keys | Vim/Neovim meaning |
| --- | --- |
| `^` / `$` | First non-blank character/end of line |
| `#` / `*` | Search backward/forward for word under cursor |
| `(` / `)` | Previous/next sentence |
| `{` / `}` | Previous/next paragraph |
| `[` / `]` | Previous/next structural commands; plugins commonly extend this convention for diagnostics, hunks, references, and similar targets |
| `<` / `>` | Decrease/increase indentation |
| `?` / `/` | Search backward/forward |
| `,` / `;` | Reverse/repeat the latest `f`, `F`, `t`, or `T` motion |
| `=` | Auto-indent operator |
| `%` | Jump to matching delimiter |
| `:` | Open command line |
| `:%` | Address the whole buffer from command line |
| `@:` | Repeat the latest Ex command |

Directional pairs keep backward/open/decrease and forward/close/increase actions together. Delimiter pairs and programming sequences such as `()`, `[]`, `{}`, `<>`, `();`, `->`, `=>`, `!=`, `<=`, and `~/` favor short rolls. Left-side copies make harder number-row, outer-column, and thumb symbols reachable when Symbol is held with right Enter.

Rearranging symbols does not break firmware, but can break these Vim direction pairs, programming rolls, and associated muscle memory. Preserve paired relationships unless intentionally redesigning workflow.

## Use

1. Keep operating-system keyboard layout set to **English (US) / QWERTY**.
2. Import `keymap.json` in [MoErgo Layout Editor](https://my.moergo.com/glove80/).
3. Save and build firmware.
