# Portfolio Development Rules

## Required Context

Before making a meaningful change:

1. Read `PROJECT.md`.
2. Inspect the relevant parts of `index.html`.
3. Do not read unrelated files unless necessary.

`PROJECT.md` contains the current project truth.
It is not a changelog.

## Architecture

Keep the project lightweight.

Default structure:

- `index.html`
- `PROJECT.md`
- `AGENTS.md`
- `README.md`

Use one self-contained `index.html` unless the user explicitly requests
something more complex.

Use:

- semantic HTML
- CSS inside `<style>`
- minimal JavaScript inside `<script>`
- CSS variables for reusable values
- responsive CSS

Do not introduce:

- React
- Tailwind
- Next.js
- npm
- build systems
- frameworks

unless explicitly requested or genuinely required.

## Editing Behavior

Always modify the existing implementation before considering a rewrite.

For normal changes:

1. Understand the existing implementation.
2. Identify the smallest correct change.
3. Modify only relevant code.
4. Remove code made obsolete by the change.
5. Preserve unrelated functionality.
6. Verify the result.

Never rebuild the entire page for a small visual change.

Do not create duplicate implementations.

## Visual Direction

Preserve the established minimalist editorial portfolio aesthetic.

General characteristics:

- off-white / neutral background
- black typography
- strong typographic hierarchy
- generous whitespace
- restrained borders
- subtle interactions
- minimal shadows
- purposeful asymmetry

Avoid:

- generic SaaS aesthetics
- excessive cards
- excessive rounded containers
- unnecessary gradients
- excessive shadows
- excessive animations
- decorative UI without purpose

## Current Hero Rules

Desktop composition:

LEFT DETAILS | CENTER PORTRAIT | RIGHT LINKS

The portrait:

- is horizontally centered
- is visually dominant
- is anchored to the bottom of the hero
- preserves its aspect ratio
- has no visible image container
- does NOT overlap the large name
- maintains a small intentional gap between hair and typography

Large name:

- JULIANE is outlined
- GONZALES is solid black

Left side:

- Web Designer & AI Automation Specialist
- supporting description
- Let's collaborate CTA

Right side:

- Selected Work
- Web Design
- AI Automation

The left and right groups sit BESIDE the portrait on desktop,
not underneath it.

## Navbar

Use only one primary navigation.

Desktop:

JG. | Work | Services | About | Contact | Available for work

The navbar:

- remains visible while scrolling
- uses readable navigation text
- stays above page content
- matches the site's neutral background
- avoids unnecessary effects

Do not recreate duplicate navigation inside the hero.

## Responsive Design

Every meaningful layout change must account for:

- desktop
- tablet
- mobile

Desktop may use the three-column hero composition.

Mobile may stack content when necessary.

Never introduce horizontal scrolling.

Never sacrifice readability just to preserve the desktop layout.

## Verification

After meaningful visual changes:

1. Check for overflow.
2. Check positioning.
3. Check responsive behavior.
4. Check that unrelated sections were not broken.
5. Check that obsolete CSS was removed.

Never claim something works unless it has actually been verified.

## Project Memory

Update `PROJECT.md` only when an important project decision changes.

Replace outdated information rather than appending history.

Do not turn `PROJECT.md` into a changelog.