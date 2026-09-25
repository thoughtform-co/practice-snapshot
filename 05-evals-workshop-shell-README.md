Pre-existing background material of the author. First published 2026-09-24 as release package-v1.0.0; this is release package-v1.0.2 of 2026-09-25, at https://github.com/thoughtform-co/practice-snapshot/releases/tag/package-v1.0.2. Cite entries by their BG id.

# The evals workshop shell

`04-evals-workshop-shell.html` is one self-contained file: no external fonts, scripts, images or requests. Open it from disk in any current browser. It is the structure of a working session on evals with placeholder words and pictures, meant to be replaced with a room's own material.

## The shape

A thin bar, a hero, fourteen sections, a colophon. Every section is one idea: a kicker (named in the source and printed on paper, not shown on screen), a two-part headline (a first part in ink, a second part in the accent colour that finishes the sentence), one short sub, and exactly one picture. A "beat" is a section with no picture: the headline large and centred, twenty seconds of silence in the room. Sections alternate a light band so the eye registers the turn of the page.

Each section fills one screen at 1280 by 720 and never scrolls. A sentence that does not fit is a sentence to cut, never a column to widen. The caps are declared on the elements themselves as `data-cap` attributes:

| Element | Cap (characters) |
|---|---|
| headline, ink part | 44 |
| headline, accent part | 56 |
| sub | 170 |
| hero lede | 220 |
| kicker (`data-kicker`) | 28 |

Seven to sixteen sections, hero and colophon not counted. Sixteen is a ceiling, not a target.

## Keys

| Key | Does |
|---|---|
| Right, Down, PageDown, Space | next section |
| Left, Up, PageUp | previous section |
| Home, End | first, last |
| F | full screen |
| P | print the handout |

The rail on the right shows one tick per section; click a tick to jump. The address bar carries `#s=<n>` so a section can be linked directly.

## Adding, removing or reordering a section

Copy one `<section>` block in the `<main class="deck">`, give it a new `id` and `data-kicker`, replace the headline, sub and picture, and place it where it belongs. The sections number themselves, the bands alternate by position, and the script builds the rail; nothing is hand-numbered. For a beat, use `class="beat"` and leave out the picture. Keep one picture per section: a single object, never a list of images.

Where scripts cannot run (a locked-down viewer, a document preview pane), the page falls back to a scrolling document with one section per screen. Everything is still readable; only the keys and the rail need the script.

## Pictures

Each picture is an inline SVG with a `viewBox`, drawn with the page's colour tokens so it follows the accent. Replace the SVG with your own, or with an `<img>` that carries a data URI if the file must stay self-contained. A picture is one object with one bright part.

## Colours and type

The tokens at the top of the stylesheet (`--ink`, `--paper`, `--band-a`, `--band-b`, `--accent`, `--muted`, `--rule`) restyle the whole page. The type is the system stack, so nothing is downloaded; set `--font-head` and `--font-body` if a licensed face is available where the page is shown.

## Printing

P, or the browser's print. The page prints landscape, one section per sheet, with the kicker shown and the bar and rail hidden. The colophon prints the provenance line.

## Verifying

`?check=1` on the address bar makes the page write a small JSON report into the colophon: section count, any section taller than the screen, any capped text over its cap. The author's verifier script does the same headless and drives every key.
