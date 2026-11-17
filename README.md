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

## Deploy

Live at https://hoseungdev0914.github.io (GitHub Pages, `main` branch, root).
Pushing to `main` redeploys; the build takes a minute or two.

The working copy lives at C:\Dev\hoseungkwack-site on the Windows machine and
is NOT the same checkout as this repo, so changes have to be copied across.
That local folder also keeps pit-of-hell.html and a few unused images that are
deliberately left out of this repo.

### Custom domain, when hoseungkwack.com is bought
1. Settings > Pages > Custom domain: enter hoseungkwack.com, Save.
   That writes a CNAME file to this repo.
2. At the registrar, point the apex A records at GitHub:
   185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   and a CNAME for www -> hoseungdev0914.github.io
3. Wait for the DNS check to pass, then tick "Enforce HTTPS".

The github.io address keeps working and redirects after that.
