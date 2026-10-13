# boot_swill

A tiny monochrome, text-mode homage to Midway's 1977 arcade game
[Boot Hill](https://en.wikipedia.org/wiki/Boot_Hill_(video_game)) — it runs in
the browser and looks (and sounds) a bit like a ZX81 game.

Everything lives in a single `index.html`. There is no build step and no
dependencies.

## Play

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Controls

| Key | Action |
| --- | ------ |
| `Q` | move up |
| `A` | move down |
| `I` | fire up |
| `O` | fire straight to the side |
| `P` | fire down |
| `SPACE` | draw / continue |
| `M` | mute |

You and the other gunman face off across the field. Each of you has six
bullets a round; when they run out you reload. Cacti and wagons give temporary
cover and fall apart when shot. Land a hit to win the round; take three hits
and it's over.

## Notes

Graphics are ASCII characters on a black canvas. Sound effects are generated
with the Web Audio API's square-wave beeper and are intentionally terrible.

The in-game music is a square-wave rendition of the cowboy standard "Home on
the Range", and a snippet of Chopin's Funeral March plays when you take a hit.
Both tunes are long out of copyright.
