# Quest Explorer

A four-page static website built with only HTML and CSS. Follow a traveler through the realm of Hollowmere: choose a region on the world map, take on a mission, and follow a route of checkpoints to the Lantern Gate.

**Team:** Arjun Baskar and Yasmine Anderson
**Track:** B, Quest Explorer
**Extension pack:** Adventure Pack
**Bonus feature:** Feature 2, Recommendation Engine UI

## Setup

No build step. Download or clone the repository and open `index.html` in a browser. Fonts load from Google Fonts, so use an internet connection to see them. Without one, system fonts are used.

## Files

```
index.html        Home
world-map.html    World map (six regions, legend, route)
mission.html      Mission detail and suggested next steps
team.html         Team and project story
css/styles.css    Shared design system (variables, components, animations)
images/           Screenshots and GIF (add before submitting)
```

## Project story

We built Hollowmere to practice semantic HTML, a CSS variable design system, Grid and Flexbox, and motion that helps users instead of distracting them. The site follows one traveler along a route of three checkpoints: Mossgate Village, Lantern Pass, and the Lantern Gate. The look is a hand-inked trail map, with stamp-style cards, a dusk hero scene, and one glowing lantern as the focal point.

## Design system

- CSS variables in `:root` for colors, fonts, spacing and shadows.
- Shared classes: `.card`, `.btn`, `.badge`, `.nav-link`, `.grid`, `.flex`, `.progress`, `.route`.
- Four animations: hero entrance, progress-bar fill, pulsing current checkpoint, and badge shine. A lantern flicker adds a fifth. All stop under `prefers-reduced-motion`.

## Accessibility

Skip link, semantic landmarks, one `h1` per page, visible focus outlines, text labels beside every color cue (badges and checkpoint states), AA contrast target, and reduced-motion support.

## Bonus feature: Recommendation Engine UI

**Purpose:** Help a visitor decide where to go next after reading a mission, the way a guide would.

**Implementation:** On `mission.html`, three "Suggested next step" cards each show a confidence label (High, Medium or Low) and a "Why this suggestion?" hint that opens with a native `details` element. A notice states that the suggestions are simulated. The cards link back into the world map, so the feature sits inside the main user flow.

**AI concept mapping:** The feature represents a recommendation system that ranks options from a user's state. Here the "state" is the traveler's progress (Mossgate complete, Lantern Pass 60 percent done). The UI simulates the ranking with fixed content and shows explainability by stating the reasoning in each hint. Confidence labels simulate model confidence. There is no real model and no data collection.

**Innovation:** Confidence is shown in text and explained in plain language, and lower-confidence cards say why they rank lower, so the user is not asked to trust a score without a reason.

**Trade-offs:** CSS-only means the suggestions cannot change with real user behavior. A `details` element is accessible and needs no JavaScript, but it cannot be animated as smoothly as a custom component.


## Design trade-offs

- Only CSS is used, so interactions rely on `:hover`, `:focus` and `details` instead of JavaScript.
- The map is a grid of region cards rather than a drawn map, which keeps it readable on small screens and easy to maintain.
- The dusk hero and the lantern are drawn with CSS shapes and gradients, which keeps the site light but limits detail.

## Credits and assets

- Fonts: Caprasimo and Atkinson Hyperlegible via Google Fonts (SIL Open Font License). Fallback: Georgia and the system sans-serif font.
- All artwork is created with CSS. No external images.
