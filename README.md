# hoseungkwack.com

Portfolio site. Plain HTML and CSS, no builder.

## Files
- index.html: home (hero + selected work)
- work/into-the-shadow.html: PROJECT OVERVIEW, not a case study. It carries the
  whole of my work on the capstone (audio, animation/rigging, VFX, UI,
  integration) and links out to the per-part case studies below it.
- work/its-adaptive-music.html: part case study 1, the adaptive BGM
  More part case studies go next to it as its-*.html, linked from the
  "My work" section of into-the-shadow.html. Next one: the Shadow-In
  animation change (section 03 there is the short version).
- work/: the other case studies (cents-for-sense, the-answer-is-7, sisyphus)
  pit-of-hell.html is kept but not linked from anywhere
- css/style.css: all styles (ink skin, breakpoints at 1100px and 760px)
- img/: images
- docs/: PDFs linked from the site

## Still to fill (search for "TODO" in the HTML)
- Gameplay video and Steam link for IntoTheShadow
- Full case study for the Shadow-In animation change
- Stage-one waveform figure on the adaptive music page
- "What I would change" for Sisyphus
- Playtest finding, materials links on the IntoTheShadow page

docs/Hoseung-Kwack-Resume.pdf is rebuilt from scratch (Nov 2026) and has real
selectable text, so ATS can read it. The old Webflow PDF had none.
Source: scratchpad resume.html, rendered to PDF with Playwright. To change it,
edit the HTML and re-render; keep the filename, it is what every Resume button
on the site points at.
Open items on it: the header links itch.io rather than a portfolio domain
(swap to hoseungkwack.com once that is live), and Memory (TOJam 2025) was
dropped to keep it to one page.

Home links are written as index.html, not "./", so the site also works when
opened straight from disk with file://.

img/sisyphus.jpg looks AI-generated. Replace it if the no-AI-art rule applies
to that project too.

The Answer is 7 images are captures from the live 1.0 WebGL build (no AI art).
The game's own title screen still uses an AI-looking classroom background
(TA7/Assets/Images/introBackground.png), so no title-screen shot is used here.

## Preview
Open index.html in a browser. Everything uses relative paths.

## Deploy (GitHub Pages + custom domain)
1. Push this folder to a GitHub repo, enable Pages on the main branch.
2. Buy hoseungkwack.com, add a CNAME file containing `hoseungkwack.com`.
3. Point the domain's DNS at GitHub Pages, then turn on "Enforce HTTPS".

IntoTheShadow is in development. It is NOT confirmed for a 2027 Steam release:
say "in development", with Level Up in April 2027 as the first public milestone.
