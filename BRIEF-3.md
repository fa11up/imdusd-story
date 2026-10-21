# "One Terminal": device plates (round 3)

Rounds 1 and 2 painted the story film. This round is a different, shorter film: a **35-second product film**
in the style of a modern app launch video: a real device floating in a dark studio, the product on its screen,
one feature per beat in large type. We add the type, the product screens and the characters in house. **You
paint the devices and the studio.**

## The look

- A **dark studio**: near-black ink `#16202E` to black, a soft cool horizon glow low in the frame (desaturated
  ivory `#F7F5EF` at low opacity, like a floor catching light far away), faint volumetric haze. No props.
- The **device**: a sleek, thin, dark-bezel desktop monitor (no stand visible, floating), rendered like a
  product shot: clean reflections, a soft rim light, slight depth of field. Photoreal 3D, not illustration.
- The **screen is a flat, uniform, very dark rectangle** (`#0B0F14`), with only a faint green glow
  (`#39FF7A` at low opacity) spilling from its edges onto the bezel. Nothing drawn on it: we composite the real
  interface on afterwards. A slightly perspective-tilted screen is fine; it must be a clean quadrilateral.
- **No text, letters, numerals, logos, brand marks or icons anywhere**, including on the device. No frogs,
  no people, no hands.
- 1920×1080, 16:9. Compose so centre crops to 1:1 and 9:16 still hold the device.

## Two homage backgrounds

Two plates place a faint world BEHIND the floating device instead of the plain studio:
- `d05`: the engraved bank hall from `refs/engraved/k1-bank.png`, far behind, darkened and desaturated to
  ~20% so the device reads first. Engraved hatching, no colour.
- `d06`: the pixel night map from `refs/pixel/` style (a dark map with a few lit points; see the story's
  `base/p03-map-night-1x.png`), far behind, dark, out of focus.

## The plates

| File | What |
|---|---|
| `d01-hero-left.png` | The monitor floating, three-quarter view turned ~25° to the left, slightly below eye level, centred. The hero plate. |
| `d02-hero-right.png` | The same monitor, three-quarter ~25° to the right, from a slightly low angle. |
| `d03-front.png` | Straight on, the screen filling ~60% of the frame width, perfectly rectangular. |
| `d04-phone.png` | A dark modern phone floating at a three-quarter angle, same studio, same blank screen rule; the phone fills ~45% of the frame height. |
| `d05-hall.png` | As d01 but with the engraved hall faint behind (above). |
| `d06-map.png` | As d02 but with the pixel night map faint behind (above). |
| `d07-end.png` | The empty studio only: no device, a single soft spotlight pool centre-frame on the dark floor, for the end card. |
| `d08-crt.png` | The STORY's CRT monitor (a chunky beige-grey 1990s CRT, see `base/p01-room-night-1x.png` for its shape) rendered in the SAME photoreal 3D studio style as the others, floating, three-quarter left, its curved glass a flat dark rectangle with the green glow. This plate bridges the story film into the product film. |
| `d09-coins.png` | The plain studio with a loose cloud of small dark metal coins floating in depth, blank faces (no markings), catching the rim light; the centre of the frame left clear for a character. |
| `sheet-3.png` | All 9 plates small, in order, file names only in its margins. |

## Report the screen corners

For every device plate, write the pixel coordinates of the screen rectangle's four corners (top-left,
top-right, bottom-right, bottom-left, in 1920×1080 pixels, to the nearest pixel) in `README.md`, so the
interface can be warped onto the screen exactly. Measure them from the delivered file.

## Deliver

`artifacts/` holds the 9 plates and `sheet-3.png`. Inspect every plate before delivering it. Redo any plate
that has text, a logo, an icon, a frog, a person, a hand, anything drawn on a screen, or a screen that is not a
clean quadrilateral. The README lists every file, its dimensions, the screen corners, and states plainly any
rule it still misses.
