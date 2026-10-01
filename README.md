# Brendan's US QWERTY with Swedish Opt layer

## Installation

```
mkdir -p ~/Library/Keyboard\ Layouts
cp -r se.brendan.* ~/Library/Keyboard\ Layouts
```

Then add **US (Swedish Alt)** in System Settings → Keyboard → Input Sources. You
may need to log out and back in before it shows up.

## Layout

The base and Shift layers are plain US QWERTY. The Option layers follow Apple's
US layout, except where noted below to make room for Swedish and other Nordic
letters.

### Option

| Key | US   | This layout        |
| --- | ---- | ------------------ |
| `[` | “    | å                  |
| `'` | æ    | ä                  |
| `;` | …    | ö                  |
| `a` | å    | æ                  |
| `t` | †    | þ                  |
| `d` | ∂    | ð                  |
| `\` | «    | …                  |
| `]` | ‘    | «                  |

### Shift+Option

| Key | US   | This layout        |
| --- | ---- | ------------------ |
| `[` | ”    | Å                  |
| `'` | Æ    | Ä                  |
| `;` | Ú    | Ö                  |
| `a` | Å    | Æ                  |
| `t` | ˇ    | Þ                  |
| `d` | Î    | Ð                  |
| `s` | Í    | ẞ (capital sharp s) |
| `w` | „    | ˇ                  |
| `]` | ’    | »                  |
| `\` | »    | †                  |
| `,` | ¯    | dead key: macron   |
| `.` | ˘    | dead key: breve    |

Everything else on Option and Shift+Option matches Apple's US layout, which
also has ø œ ç µ ‹ › € ∑ © and friends where you would expect them. There are
no typographic quotes; use guillemets « » ‹ › instead.

### Dead keys

| Keys              | Accent     | Example |
| ----------------- | ---------- | ------- |
| Option+`` ` ``    | grave      | à       |
| Option+E          | acute      | é       |
| Option+U          | diaeresis  | ü       |
| Option+I          | circumflex | ê       |
| Option+N          | tilde      | ñ       |
| Shift+Option+,    | macron     | ā       |
| Shift+Option+.    | breve      | ă       |

A dead key followed by **any** letter (including å, ä, ö, æ, ø, þ, ð, ß, œ and
their capitals) gives the precomposed character if Unicode has one, and
otherwise the letter followed by the combining accent, e.g. q̀, þ́, ǻ. This is
deliberate, so less common letter/accent pairs used by minority languages can
still be typed.

- Dead key then Space, or the same dead key twice: the spacing accent (´ ¨ ˆ ` ˜ ¯ ˘).
- Dead key then a different dead key: the first accent is emitted, and the
  second dead key becomes active.

### Caps Lock, Command and keypad

- **Caps Lock + Option** gives the Option layer with uppercase letters (Å Ä Ö Æ
  Ø Œ Þ Ð Ç ẞ), and dead keys produce uppercase accented letters. Symbols and
  digits stay as on the Option layer. Caps Lock + Shift + Option behaves like
  Shift + Option.
- **Command + Option** uses the base (or Shift) layer, so shortcuts like
  ⌘⌥I and ⌘⌥[ work as in US.
- The numeric keypad and the JIS-specific keys (¥, _, keypad comma, Eisu/Kana)
  work as on Apple's US layouts.
