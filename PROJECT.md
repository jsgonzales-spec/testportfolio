# Project Context

## Repository https://github.com/jsgonzales-spec/testportfolio
## Deployment Live at https://testportfolio-pearl.vercel.app, redeploys automatically from main.
## Product Personal portfolio for a web designer and AI automation specialist.
## Audience Small businesses and startups looking for web design or practical AI automation.
## Goal Land freelance clients by showing capabilities, portfolio work, and a clear contact path.
## Brand Juliane Gonzales; modern, capable, practical, honest about being early in the professional journey.
## Visual Direction Minimal, typography-led portfolio hero inspired closely by the supplied reference: oversized outlined/solid name, centered portrait, compact navigation, status pill, and floating text/link groups. No framed card around the hero or photo.
## Page Structure Sticky primary navbar (blurred off-white background), hero with real portrait cutout, moving service marquee, selected work, services, about, contact CTA, footer.
## Navbar Sticky (position:sticky, 76px desktop / 68px mobile), rgba off-white background with backdrop-filter blur, single Work/Services/About/Contact link set (the hero no longer duplicates these — it only keeps its own status pill and “Let’s Talk” CTA). Sections carry scroll-margin-top so anchor links land below the sticky bar.
## Hero Portrait Real transparent PNG cutout at images/juliane.png (background removed from the uploaded headshot, downscaled + pngquant-compressed for file size). Sits in normal document flow between the name and the role/links row, pulled up with a negative top margin so it overlaps the giant typography (name behind, portrait in front) while keeping clear space above the role heading so text is never covered. object-fit:contain, object-position:center bottom, never stretched.
## Services Section Accordion-style list (eyebrow label, large uppercase row names, one panel open at a time). First item open by default with a dark expanded panel holding the description and a small abstract layered-card visual (no stock imagery); collapsed rows show name + plus icon that rotates to a close (×) state when open. Pure CSS grid-rows expand/collapse, no height calc in JS.
## Copy Direction Direct, specific, client-focused, no exaggerated experience claims.
## Assets Hero portrait is a real photo (images/juliane.png, transparent cutout, background removed).
## Functionality Sticky nav, responsive navigation anchors with scroll-margin offset, animated hero entrance (top bar/name/portrait/info staggered), a JS fit-to-width safety net so the giant name can never overflow at any viewport, marquee, scroll reveals, project hover motion, reduced-motion support (static hero + paused marquee), contact mailto CTA.
## Avoid Fake client results, invented experience, excessive decoration, generic filler copy, and unnecessary boxed/card treatment in the hero.
## Current Decisions Main CTA is “Let’s work together”. Services are Web Design, AI Automation, and Virtual Assistant. Target is small businesses/startups. The hero portrait uses flow-based positioning (not absolute) because this hero centers itself vertically within a capped min-height — absolute+bottom-anchoring was tried and broke on tall viewports (portrait detached from the rest of the hero content and bled into later sections), so flow + negative margins is the deliberate choice here.
