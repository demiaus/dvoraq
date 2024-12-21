## dvoraq

### Another Finnish Programmer Dvorak layout

Inspired by Pekka Oinas' Finnish Dvorak layout. I used this for a while in 2021. Now this is mostly just an archive. I still think this is the best Dvorak there is but losing all QWERTY ability made me return to the dark side.


#### Quickstart

###### Clone repo
```
$ git clone https://github.com/quunnb/dvoraq && cd dvoraq
```
###### Copy files
```
# cp dvoraq /usr/share/X11/xkb/symbols/
```
###### Load keymap
```
$ setxkbmap -config dvoraq.conf
```

#### Default layer
```
,---,---,---,---,---,---,---,---,---,---,---,---,---,-------,
| ` | 7 | 5 | 3 | 1 | 9 | 8 | 0 | 2 | 4 | 6 | [ | ] | <-    |
|---'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-----|
| ->| | ' | , | . | u | y | f | g | l | r | c | / | = |     |
|-----',--',--',--',--',--',--',--',--',--',--',--',--'|    |
| Esc  | a | o | e | i | p | d | h | t | n | s | - | \ |    |
|----,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'---'----|
| LS | ö | ä | q | j | k | x | b | m | w | v | z |  Shift   |
|----'-,-',--'--,'---'---'---'---'---'---',--'---',--,------|
| Ctrl |  | Alt |                         | AltGr |  | Ctrl |
'------'  '-----'-------------------------'-------'  '------'
```

#### Shift layer
```
,---,---,---,---,---,---,---,---,---,---,---,---,---,-------,
| ~ | ^ | @ | # | ! | % | & | ( | ) | { | } | * | $ | <-    |
|---'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-----|
| ->| | " | ; | : | U | Y | F | G | L | R | C | ? | + |     |
|-----',--',--',--',--',--',--',--',--',--',--',--',--'|    |
| Esc  | A | O | E | I | P | D | H | T | N | S | _ | | |    |
|----,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'-,-'---'----|
| LS | ö | ä | Q | J | K | X | B | M | W | V | Z |  Shift   |
|----'-,-',--'--,'---'---'---'---'---'---',--'---',--,------|
| Ctrl |  | Alt |                         | AltGr |  | Ctrl |
'------'  '-----'-------------------------'-------'  '------'
```

#### AltGr layer
Not pictured but `,` and `.` are `<` and `>`. Rest are pretty much just Greek letters.

### Summary

#### On left-hand side:
- Rotates index finger letters `I`, `U` and `P` around clockwise
    - `I` is very common, so now straight under index finger
    - `U` sits still quite comfortably next to somewhat visually similar `Y`
    - `P` is demoted to center column: we don't like lateral movement
- Pekka Oinas found the optimal keys for `Ä` and `Ö`, but I switch them around
    - `Ä` is far more common than `Ö` in Finnish, so `Ä` is given easier access

#### On right-hand side:
- Switches `C` and `L` for more comfort especially in writing Finnish
    - `L` is also somewhat more common in English than `C`

#### Number row:
- Uses 'Classic/Programmer Dvorak'-inspired number row: `7531980246[]`
- Unlike its inspirations, both odd and even numbers move outward until `8` and `9` "wrap around" to the middle column
- Index fingers get the most common `0` and `1` numbers.
- Parity is strictly divided between hands.
- Symbols are rearranged: `~^@#!%&(){}*$`.
- Relative to Oinas' Dvorak number row's `2`. layer:
    - `()` and `{}` move `2` keys left/inwards for easier access.
    - `*` takes `{`'s old place, `$` takes `}'`s old place (`$`, grep symbol for end-of-line, visually on the right end).
    - `!` takes `$`'s old premium place under left index finger same key as `1`.
    - `^` takes `!`'s old place under left pinky (grep symbol for 'start-of-line' visually on the left 'end').
    - `&` takes `^`'s old place on the right-hand center column (the regular Finnish position).

#### Third & Fourth level:
- Tries to use almost all the Greek letters for easier math etc. equations.
- Third layer space is `_`
- Non-breaking space is moved to fourth level to prevent mistyping.

#### Other keys:
- `CapsLock` is `Escape`
- Numpad `Delete`:
    - Default: `.`
    - Second layer: `,`
    - Third layer: `:`
    - Fourth layer: `;`


#### Extra:
You can analyze the layout by importing the json file to this website:
https://stevep99.github.io/keyboard-layout-analyzer/
