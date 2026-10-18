# QA Notes: Quest Explorer

## 1. Code-level checks (done)

| Check | Result |
|---|---|
| Every internal link points to an existing page or anchor (5 pages) | Pass |
| One `h1` per page, no skipped heading levels | Pass |
| Landmarks present on every page (`header`, `nav`, `main`, `footer`) | Pass |
| `lang`, `title` and viewport meta tag on every page | Pass |
| Skip link target `#main` exists on every page | Pass |
| Exactly one `aria-current="page"` link in the nav of each page | Pass |
| Duplicate `id` values | None found |
| Images missing `alt` text | None (the site uses no `img` elements) |

## 2. Color contrast (calculated from the CSS colors)

Target: WCAG AA, 4.5:1 for normal text.

| Pair | Before fix | After fix |
|---|---|---|
| Teal link on card | 3.99, fail | 6.94, pass |
| Teal link on page background | 3.37, fail | 5.87, pass |
| Muted text on lilac map tiles | 4.03, fail | 5.46, pass |
| White text on teal "done" checkpoint | 4.06, fail | 7.06, pass |
| Body text, nav, hero text, footer, active nav, mint/sky/sand tiles | 6.4 to 16.5, pass | unchanged |

**Fix made:** `--teal` changed from `#2a8c82` to `#1a6359` and `--muted` from `#4a4868` to `#363457` in `css/styles.css`.

## 3. Navigation findings

- Header nav links the same four destinations on every page and marks the current page.
- The "Mission" nav link always opens Light the Lanterns, even when the user is on the Reedmarsh page. (Both mission pages mark "Mission" as current.)
- **Open issue:** Sunken Harbor, Amber Dunes and Lantern Gate map cards open the Light the Lanterns page, which does not match their names.
- **Open issue:** the home page's "Wake the Sunken Bell" card links to the world map instead of a mission.
- Mission pages link to each other and to the map through the suggestion cards.

## 4. Accessibility findings

- Visible focus outline on all links, buttons and `summary` elements (4px rose outline).
- Badges and route states always carry text (Easy, Medium, Hard; Complete, Current, Locked), not color alone.
- Progress bars are hidden from screen readers, and the percentage appears in text next to each one.
- `prefers-reduced-motion` turns off all animations and transitions.
- Hints use native `details`, which works by keyboard (Tab, then Enter or Space).
- Risk: card rotations and the hero lantern are decorative. Check that the lantern does not overlap the headline on narrow phones.