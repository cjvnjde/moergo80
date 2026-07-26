# cjvnjde's Glove80 Layout

Version 1 of cjvnjde's personal [MoErgo Glove80](https://www.moergo.com/) layout.

[Open the layout in MoErgo Layout Editor](https://my.moergo.com/glove80/#/layout/user/8fa685c6-d1cb-4726-92e0-b6292b6f6668)

## Important: host keyboard layout

Dvorak is implemented directly in keyboard firmware. Keep computer input layout set to **English (US) / QWERTY**. Setting operating system to Dvorak remaps keys a second time and produces incorrect characters.

## Design

Layout keeps full number and function rows while making Dvorak primary typing layer. Dedicated layers provide QWERTY compatibility, navigation, numpad, media controls, programming symbols, Bluetooth management, RGB controls, and firmware utilities.

No home-row modifiers or combos are configured. Two hold-tap keys provide quick access to secondary layers:

- **Symbol / Escape**: tap for `Escape`; hold for Symbol layer.
- **Lower / Delete**: tap for `Delete`; hold for Lower layer.

Both use hold-preferred behavior with a 200 ms tapping term.

## Layers

### 0 — Dvorak

Primary layer. Standard Dvorak alpha arrangement is emitted by keyboard, with:

- Number and function rows
- Dedicated modifiers
- Arrow keys and Page Up/Page Down
- Backspace, Enter, Space, brackets, slash, and equals in thumb/edge positions
- Hold-tap access to Lower and Symbol layers
- Dedicated Magic-layer key

### 1 — QWERTY

Fallback QWERTY alpha layer. Most surrounding keys and layer access remain consistent with Dvorak layer. Toggle this layer from Magic layer.

### 2 — Lower

Utility layer containing:

- Display brightness and media controls
- Home, End, Page Up/Page Down, arrows, and Insert
- Full numeric keypad and keypad operators
- Print Screen, Scroll Lock, Pause, and application/menu key
- Caps Word and key repeat

Hold **Lower / Delete** to use this layer.

### 3 — Symbol

Programming and punctuation layer containing brackets, braces, parentheses, operators, quotes, slashes, and navigation arrows.

Hold **Symbol / Escape** to use this layer.

### 4 — Magic

Keyboard-management layer containing:

- Bluetooth profile selection and bond clearing
- USB output selection
- RGB toggle, effect, speed, saturation, hue, and brightness controls
- Bootloader and reset controls
- QWERTY-layer toggle

Use reset, bootloader, and Bluetooth-clear keys carefully.

## Files

- [`keymap.json`](keymap.json) — MoErgo Layout Editor backup/import file.

## Import and build

1. Sign in to [MoErgo Layout Editor](https://my.moergo.com/glove80/).
2. Open **Settings** and enable **Local Backup and Restore**.
3. Open Layout Editor and use bottom-left **Import** controls to import `keymap.json`.
4. Review layout, then use **Save and Build** to build firmware for Glove80.

MoErgo marks JSON import/export as experimental, so format compatibility may change with future Layout Editor versions.
