# Design record: elileomir.github.io

## Register
Quiet, technical, developer audience. One page family for the Sandboxed YouTube channel: home, privacy
policy, terms. Static HTML and one stylesheet, no scripts.

## Brand
- Sandboxed brand kit: Glovebox mark (box with a viewing window and two glove ports), wordmark
  `sandboxed_` in SF Mono with an amber cursor.
- One accent only: caution amber.

## Theme scenes and tokens (sandboxed/style.css :root)
| Token | Dark (default) | Light |
|---|---|---|
| --bg | #0F1012 ink | #F6F4EF warm paper |
| --panel | #17191C | #FFFDF8 |
| --line | #2C2F34 | #DDD8CE |
| --text | #ECE8DF paper | #1A1B1D |
| --muted | #A29E96 | #5E5A53 |
| --amber | #F2B705 | #8A6500 |

- Light-mode amber is #8A6500 because #F2B705 on light paper fails text contrast (about 1.6:1); #8A6500
  keeps links and the cursor above 4.5:1.
- The brand paper colour #ECE8DF is the dark-mode text colour; light mode uses a lighter paper (#F6F4EF)
  as background so body text keeps strong contrast.
- The mark switches to the ink version (mark.svg) in light mode so the logo holds at least 3:1.

## Type
Scale 12 13 14 16 18 20 24 30 36 48 60. Body 16px/1.6, h1 30px, h2 20px, footer 14px, wordmark 30px mono.

## Accessibility
Footer links and the contact email link (`.contact`) get 4px vertical padding (about 26 to 30px tall), and 12px on touch screens (about 44px). Focus is a 2px amber outline, 3px offset.
