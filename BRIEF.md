# "Nobody Works Here": style frames

A 2-minute film for imdUSD, a dollar stablecoin run by the IdentityMD agent swarm. It has no narrator
and no captions, only sound and music, so these frames have to tell the story on their own.

This brief asks for **the background plates only**. Everything that moves or carries words is added
afterwards in code: the frogs, the keepers, every letter and number, glowing screens, lit windows and
the dissolve. Leave room for those things as described below and **do not draw them yourself**.

## The story in one paragraph

At 3:47 AM an anonymous frog in a hoodie types one question into an old CRT terminal: *who decides
what a dollar is worth?* For five hundred years a bank decided (an engraved world: marble, locks,
boardrooms, stamps). The question leaves his screen as one green trace and wakes machines all over
the world (pixel world: a server rack, a dorm laptop, a tiny computer taped under a desk). The
engraved bank dissolves line by line into pixels, the machines agree, a press prints a banknote. A
storm hits the market at night, and small keepers clean it up. At dawn the camera pulls back to
reveal one building where every window is an agent: a whole company with nobody in it. The frog
wakes up, smiles, closes his laptop and goes back to sleep.

## Two worlds, two styles: never mix them in one frame

**ENGRAVED (the old world).** Match `refs/engraved/` exactly: k1-k6 are frames from our previous
film and set the register; `note-front-16x9.png` and `portrait-detail.png` are the banknote. Fine
intaglio linework, hatching and cross-hatching, guilloché, no flat colour, no gradients, no
photographic texture. Colours, only these:

| ivory paper | ink linework | engraved green | oxblood (ONE lamp or seal per frame, or none) | hairline |
|---|---|---|---|---|
| `#F7F5EF` | `#16202E` | `#2F5D50` | `#8C2F2F` | `#D8D3C7` |

**PIXEL (the swarm).** Real pixel art, matching `refs/pixel/` (our own pixel Pepe: hard square
pixels, dark outlines, no anti-aliasing). Draw each frame on a **320×180 grid**, then upscale it
**6× with nearest-neighbour** to 1920×1080. Every pixel in the 1920 file is a clean 6×6 block.
Colours, only these 15:

```
#0B1018 night     #16202E ink       #22314A navy      #3A4A63 slate     #6A7A8C mist
#C9C4B8 stone     #F7F5EF ivory     #2F5D50 deep green #447F31 moss     #5B9B3D leaf
#39FF7A terminal  #8C2F2F oxblood   #B5544B brick     #D98E3B amber     #F2C46B dawn
```
`#39FF7A` terminal green is reserved for things that are ON (screens, LEDs) and must be used sparingly.
If your image tool can't produce exact pixel art, generate the image, then enforce the grid and palette in code:
downscale to 320×180 with nearest-neighbour or box sampling, map every pixel to the nearest palette
colour, clean up stray single pixels, and upscale 6× with nearest-neighbour. Look at the result and
redo it if it reads as mush.

## Hard rules (every frame)

- **No legible text, letters, numerals, logos or brand marks anywhere**, including screens, signs,
  clocks, keyboards, books, stickers and posters. Clock faces have ticks and no numbers. Blank signs
  stay blank.
- **No frogs and no visible human faces.** The frogs are added in code. People may appear only as
  shapes asleep under a blanket or as suits seen from behind (engraved only).
- No real bank, building, company, currency or product. Everything is clearly fictional.
- Every frame 1920×1080 unless stated. Compose so **a centre crop to 1080×1080 and to 608×1080
  (9:16) still holds the subject**. The film ships square and vertical too.
- Screens that the story needs lit (marked ⬚ below) are drawn as **flat, empty, dark rectangles**
  with a clean edge, so a glowing screen can be laid exactly over them.

## The frames

### Engraved (4)

| File | Scene | Leave for us |
|---|---|---|
| `e1-hall.png` | a vast marble banking hall, empty, long counters behind bars, a huge wall clock, light falling in shafts | clock face with ticks, no numerals, no hands (we animate them) |
| `e2-vault-door.png` | a round vault door seen head-on, seven heavy bolts and locks around its rim, all closed | none |
| `e3-stamp.png` | close on a desk: a form on the blotter (ruled lines, no words), a heavy rubber stamp raised above it in a hand in a suit cuff | the form's centre clear; the stamp face blank |
| `e4-tower.png` | **3840×2160.** A tall bank TOWER at dawn, drawn like a bank's engraved façade stretched into a skyscraper: columns at its foot, a pediment with an EMPTY cartouche at the top, and a strict grid of many small identical windows up its whole height, all DARK. City roofs below, sky above | windows dark and regular (we light them one by one); cartouche empty; tower centred so a crop to 1920×1080 at any height still frames it |

### Pixel (13)

| File | Scene | Leave for us |
|---|---|---|
| `p01-room-night.png` | 3:47 AM, a small bedroom-office lit only by a CRT on a cluttered desk: an energy-drink can (no label), a mechanical keyboard, a cat asleep curled on a wifi router, cables, a window with a night city, a wall clock | ⬚ CRT screen; the desk chair EMPTY and turned slightly toward the viewer (our frog sits in it); clock with ticks, no hands |
| `p02-room-dawn.png` | **the same room, same composition pixel for pixel**, now at dawn: warm light through the window, CRT off. Make it by recolouring p01 (same 320×180 grid), not by redrawing | same as p01 |
| `p03-map-night.png` | looking down at a night city from high above, a dark grid of streets and rooftops with scattered warm windows, one cable running out of a window at lower left | street paths clear so a green trace can run along them |
| `p04-rack.png` | a cold server room in a northern city: one tall rack of servers, fans, blinking LEDs, snow falling past a small window | ⬚ a tiny status screen on the rack |
| `p05-dorm.png` | a dorm room at night: a laptop open on a messy bed, someone asleep under the blanket beside it (a shape, no face), posters on the wall with NO text or images | ⬚ laptop screen |
| `p06-pi.png` | low angle under a desk: a tiny bare circuit board computer taped to the underside, one cable, dust, a sock | one LED spot left dark (we blink it) |
| `p07-chart.png` | a wall-sized market chart at night: candlesticks falling hard to the right, in brick and oxblood, rain on a window over it | no axis labels, no numbers |
| `p08-sea.png` | a dark stormy pixel sea under lightning, big waves, an empty patch of water at centre | the centre water open (our pixel whale breaches there) |
| `p09-keeper-floor.png` | a dim vault floor at night: a wooden crate, a lantern on the floor (unlit), a trapdoor, a stack of paper notes on a table bleeding ink at the edges | space left of centre for two small figures; lantern unlit |
| `p10-floor-vault.png` | inside the tower, the vault floor: a round vault door open, coin trays, a coin chute | none |
| `p11-floor-desk.png` | inside the tower, a research floor: a wall of dozens of small monitors in a grid, no people | ⬚ every monitor |
| `p12-floor-hr.png` | inside the tower, a small empty office with the lights on, chairs pushed neatly under desks, a potted plant, a door at centre with a blank sign plate | sign plate blank and flat, facing the camera |
| `p13-city-dawn.png` | the city at dawn seen from high outside a window, rooftops, a tall tower in the distance | tower windows dark |

## Deliver

`artifacts/` holds the 17 files above, plus for every pixel frame its native grid as
`pNN-name@1x.png` (320×180) so we can recolour and animate it, plus `sheet.png` (all 17 small,
in order, labelled by file name in plain text in the sheet's margins only).

Inspect every frame before delivering it, and regenerate any that has text, numerals, a logo, a frog, a face,
an off-palette colour, or (pixel only) pixels that aren't clean 6×6 blocks. The README lists each file with its size and says plainly any rule it still breaks.
