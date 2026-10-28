# NNAM VPCL — Baseline 1.0 Requirements

Baseline 1.0, 27 October 2026. Unofficial personal prototype built from the NNAM Volunteer Guide (rev. 20 March 2025). The Guide and Museum staff direction govern.

Verification methods: I = inspection, A = analysis, D = demonstration, T = test.

| ID | Requirement | Method | Status at Baseline 1.0 |
|----|-------------|--------|------------------------|
| R-1 | All content comes from the NNAM Volunteer Guide (rev. 20 Mar 2025), with paragraph citations. | I | Met |
| R-2 | Complements, never changes, official guidance. Guide conflicts are flagged (†); suggested memory items are labeled as the checklist's suggestion. | I | Met |
| R-3 | NATOPS pocket-checklist look: white normal side, yellow emergency side with hash border, tabs, memory items, list of effective pages. | I | Met |
| R-4 | Plain language for non-military readers; Navy and Museum terms explained on tap. | I, D | Met |
| R-5 | Suited to older users: pinch to zoom for bigger type (no separate type-size control), large buttons, nothing disappears on its own, a sign when a page has more below. | D | Met |
| R-6 | Works the same on iPhone, Android, iPad, Windows and Mac browsers. | T | Partial (Chrome engine verified; Safari/Firefox engines pending real devices) |
| R-7 | One control model for touch, mouse and keyboard; gestures and keys are shortcuts only. | D | Met |
| R-8 | Opens from a QR code with no account or app store. | T | Met |
| R-9 | Installable; works offline after first visit. | T | Partial (verified in Chrome engine) |
| R-10 | Emergency side one tap away; code card rows and page numbers link directly to procedures. | D | Met |
| R-11 | Low upkeep for the owner. | A | Met (static); at risk if AI features are added |
| R-12 | AI features can never exceed the monthly API credit. | A | Met by design (not yet built) |
| R-13 | Not fielded without approval from the NNAM Volunteer Coordinator or Museum authority. | I | Open gate |

## Configuration
- Product: `index.html` (checklist), `manifest.webmanifest`, `sw.js` (offline), `icons/`.
- Hosting: GitHub Pages, https://lootac.github.io/nnam-vpcl/
- Change 1 (planned): Ask the Guide and Drill instructor via a Cloudflare Worker and the Claude API, isolated so the baseline works without it.
