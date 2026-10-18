# Quest Explorer: Kanban Timeline

HTML and CSS Portfolio Project · Track B, Adventure Pack, Bonus Feature 2

## Roles

- **Arjun Baskar:** layout, navigation, content, repository and final release
- **Yasmine Anderson:** components, motion, accessibility, the bonus feature and its documentation

## Phase 1: Plan + Structure (Days 1-3)

| # | Card | Label | Owner | Est. | Definition of done |
| --- | --- | --- | --- | --- | --- |
| 1 | Confirm track, extension pack and bonus feature | docs | Both | 1 h | Choices match the signed proposal |
| 2 | Create GitHub repo, `.gitignore` and folder structure (`css/`, `images/`) | docs | Arjun | 1 h | Both members can clone and push |
| 3 | Set up this Kanban board and add all cards | docs | Yasmine | 1 h | Cards, labels and WIP rules visible |
| 4 | Read through `index.html` and `world-map.html`; note one question per section | layout | Arjun | 2 h | Questions posted to the team |
| 5 | Read through `mission.html` and `team.html` | bonus | Yasmine | 2 h | Questions posted to the team |
| 6 | Read through `styles.css` (variables, cards, animations) | css-motion | Yasmine | 2 h | Can explain each section aloud |
| 7 | Open every page in a browser and list defects | testing | Both | 1 h | Defect list added as cards |
| 8 | Draw wireframes for all four pages (paper is fine) | layout | Arjun | 2 h | Photos stored in `docs/` |
| 9 | Decide your own palette, fonts and world name | content | Both | 2 h | Design decisions written in README |

**Checkpoint at end of Day 3:** repo works, board is live, everyone has read the whole code once.

## Phase 2: Layout + Components (Days 4-7)

| # | Card | Label | Owner | Est. | Definition of done |
| --- | --- | --- | --- | --- | --- |
| 10 | Review semantic structure and heading order on every page | a11y | Yasmine | 2 h | One `h1` per page, logical order |
| 11 | Tune the Grid layout of the world map | layout | Arjun | 3 h | Regions reflow at 360, 768, 1024 and 1440 px |
| 12 | Refine shared header and navigation | layout | Arjun | 2 h | Same nav on all pages, current page marked |
| 13 | Finalize card, button and badge components | components | Yasmine | 3 h | Used consistently on all four pages |
| 14 | Add missing small-screen breakpoint rules | layout | Arjun | 2 h | No horizontal scrolling at 360 px |
| 15 | Build the mission page route steps | components | Yasmine | 3 h | Step list matches the proposal |
| 16 | Add a visible-focus pass for every interactive element | a11y | Yasmine | 2 h | Keyboard-only tab-through succeeds |
| 17 | Write the real content for the world map regions | content | Arjun | 3 h | No placeholder text left on map page |

**Checkpoint at end of Day 7:** all four pages are responsive and use the shared components.

## Phase 3: Styling + Motion (Days 8-11)

| # | Card | Label | Owner | Est. | Definition of done |
| --- | --- | --- | --- | --- | --- |
| 18 | Apply your chosen palette and fonts through CSS variables | css-motion | Arjun | 3 h | Colors changed in `:root` only |
| 19 | Tune hero visual and the lantern animation | css-motion | Yasmine | 3 h | Looks good and respects reduced motion |
| 20 | Review all animations (at least three) and the reduced-motion fallback | css-motion | Yasmine | 2 h | Animations stop with the OS setting on |
| 21 | Complete the Adventure Pack route timeline states | components | Arjun | 3 h | Done, current and locked states are clear in text, not color only |
| 22 | Build the Recommendation Engine UI cards with confidence labels | bonus | Yasmine | 3 h | Three suggestion cards with hints |
| 23 | Add the explainability hints and the simulation notice | bonus | Yasmine | 2 h | Notice says suggestions are simulated |
| 24 | Check text and UI contrast with a contrast tool | a11y | Arjun | 2 h | All text meets WCAG AA, fixes committed |
| 25 | Write real missions and links between pages | content | Arjun | 3 h | Every link goes somewhere sensible |
| 26 | Peer review of all styling cards | testing | Both | 2 h | Review notes added as comments |

**Checkpoint at end of Day 11:** design is final, extension pack and bonus feature are integrated into the main flow.

## Phase 4: QA + Portfolio Packaging (Days 12-14)

| # | Card | Label | Owner | Est. | Definition of done |
| --- | --- | --- | --- | --- | --- |
| 27 | Run the W3C HTML validator on all pages | testing | Arjun | 1 h | Zero errors, or documented exceptions |
| 28 | Run the W3C CSS validator | testing | Yasmine | 1 h | Zero errors, or documented exceptions |
| 29 | Run Lighthouse accessibility checks | a11y | Yasmine | 2 h | Score recorded in README |
| 30 | Responsive test at 360, 768, 1024 and 1440 px (plus one real device if possible) | testing | Both | 2 h | Results table in README |
| 31 | Usability test with at least three peers, using three tasks | testing | Both | 3 h | Task table with notes saved |
| 32 | Write 3+ bonus feature test checks (layout, accessibility, responsive) | docs | Arjun | 2 h | Documented in README |
| 33 | Write the bonus README section (purpose, implementation, trade-offs, AI concept mapping, innovation note) | docs | Yasmine | 3 h | All six qualification items present |
| 34 | Take screenshots and record a short GIF | docs | Yasmine | 2 h | Files in `images/` |
| 35 | Finish README: project story, setup, reflection on design trade-offs | docs | Both | 3 h | Matches the real final project |
| 36 | Clean up file names and organization, then review commit history | docs | Arjun | 1 h | Commits are meaningful |

**Checkpoint at end of Day 14:** the project is complete and submittable.

## Buffer Days 15-17: Polish only

No major new features. Use these days for:

| # | Card | Label | Owner | Est. | Definition of done |
| --- | --- | --- | --- | --- | --- |
| 37 | Fix bugs found in QA | bug | Whoever found it | as needed | Re-tested and closed |
| 38 | Apply peer-feedback fixes | content | Both | 4 h | Each fix linked to a commit |
| 39 | Final read-through of all text for typos | content | Yasmine | 1 h | No spelling errors |
| 40 | Rehearse the presentation; each person explains their own part of the code | docs | Both | 3 h | Both can answer questions on their area |
| 41 | Final push, tag the release and test a fresh clone | docs | Arjun | 1 h | Site opens correctly from a clean download |
