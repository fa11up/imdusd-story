# "Nobody Works Here": character plates (round 2)

Round 1 (`BRIEF.md`) painted empty backgrounds. This round puts the **characters into the scenes**. Every
rule from `BRIEF.md` still applies (two styles, exact palettes, the 320×180 pixel grid upscaled 6× nearest-neighbour,
no legible text, letters, numerals or logos, no human faces), with ONE change: **frogs are now wanted**.

## The frog

The hero is our own pixel Pepe-style frog: see `refs/pixel/agent-pepe.png` (hooded, the casual look) and
`refs/pixel/feels-stable.png` (in a suit). Green skin `#5B9B3D` with `#447F31` shading, ink `#16202E`
outlines, ivory eye whites, brick `#B5544B` lips, heavy-lidded smug eyes. Keep him recognisably the same
frog in every plate. In pixel scenes he is drawn in the same 320×180 grid as the room, not smoother.

## Edit, don't redraw

Plates marked **EDIT** must keep the base image's pixels everywhere except where the character goes. Start
from the given base (`base/…-1x.png`, the native 320×180 grid) and paint the character into it, so the
plate cuts seamlessly with the base. Pairs marked **A/B** are two animation frames: identical except for
the moving part.

## The plates

| File | Base | What |
|---|---|---|
| `p01-seated-a.png` | EDIT `base/p01-room-night-1x.png` | The hooded frog SITTING in the desk chair, typing at the keyboard. Seen from behind at three-quarters: hood up, a little of his cheek and one eye visible turned toward the screen, shoulders and back filling the chair, both arms reaching forward to the keyboard, hands on the keys. His whole upper body is visible; he sits IN the chair, not floating above it. The CRT screen stays a flat empty dark rectangle. |
| `p01-seated-b.png` | EDIT, same as A | Identical, except both hands are lifted slightly off the keys (the other typing frame). |
| `p01-bed-night.png` | EDIT `base/p01-room-night-1x.png` | The chair EMPTY. The frog asleep on the bed on the right, lying on his side under the blanket, head on the pillow, eyes closed, a peaceful smug smile. |
| `p02-bed-dawn.png` | EDIT `base/p02-room-dawn-1x.png` | The same sleeping frog, same pixels, in the dawn version of the room (recolour of p01-bed-night with the dawn palette, exactly as p02 is a recolour of p01). |
| `e3-stamp-down.png` | EDIT `base/e3-stamp-clean.png` (ENGRAVED, 1920×1080) | The same desk, the same hand and cuff, but the hand has brought the rubber stamp DOWN: the stamp is pressed flat on the centre of the form. Everything else unchanged so the two images cut together as one motion. Stamp face and form stay blank. |
| `p14-furnace-a.png` | new (PIXEL) | A foundry at night: a huge furnace mouth at left-centre glowing amber and dawn-yellow, a chute or conveyor at the right where GOLD BARS come out and stack (gold = `#F2C46B` and `#D98E3B` with ink outlines), the floor in front clear. Two frogs in hoodies (one deep green, one brick) stand at the furnace mouth throwing paper banknotes (plain ivory rectangles, no markings) into the fire. Pose A: arms drawn back holding a stack of notes. |
| `p14-furnace-b.png` | EDIT `p14-furnace-a` | Identical, except both frogs' arms are thrown forward and the notes are leaving their hands toward the fire. |
| `p15-oval-office.png` | new (PIXEL) | A grand oval office in sunlight: tall windows with trees, gold curtains, two flags on poles (plain fabric, NO real flag, emblem or seal), a large carved wooden desk centre-front, a leather executive chair behind it, and stacks of gold bars piled high on both sides of the room. The chair EMPTY. A blank brass plate on the desk front. Warm and triumphant. |
| `p15-president.png` | EDIT `p15-oval-office` | The same room with the frog sitting in the chair at the desk like a president: navy suit, white shirt, tie, relaxed and smug, holding a gold mug (blank, no words) in one hand. Base his suit on `refs/pixel/feels-stable.png`. |

Pixel plates: deliver the 1920×1080 file and its native `-1x.png` (320×180). The engraved plate is 1920×1080 only.

## Deliver

`artifacts/` holds the 9 plates, the 8 native `-1x` grids, and `sheet-2.png` (all 9 small, labelled in the margin).
Inspect every plate before delivering it. Redo any plate that has text, numerals, a real flag or seal, a human face, colours outside the
palette, a frog who doesn't match the reference, or (EDIT plates) changed pixels outside the character. The README
lists each file and says plainly any rule it still breaks.
