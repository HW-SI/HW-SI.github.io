# Figure Prompts

Use these prompts to generate original, website-safe scientific illustrations for `hw-si.github.io`. The target is closer to NASA/JPL and ESA public-science artwork: physically readable artist's impressions, careful explanatory schematics, restrained color, and captions that make the science clear. Avoid generic AI space art, cinematic sci-fi, fake detector interfaces, and anything that looks like uncited observational data.

Reference style to emulate:

- NASA/JPL-style artist's concepts: recognizable accretion disk, compact object, jet/outflow, and physically motivated geometry.
- ESA-style science illustrations: clean composition, restrained contrast, clear separation between source, outflow, and surrounding medium.
- Academic webpage figures: readable at small size, calm enough to sit beside text, and not visually louder than the research content.

General requirements for every image:

- Export as `.webp` if possible; `.png` is also acceptable.
- Use lowercase filenames with hyphens, saved under `images/`.
- No text labels inside the image. Captions will be written in HTML/Markdown.
- No institutional logos, telescope logos, collaboration logos, fake signatures, or watermarks.
- No fake plot axes, spectra, detector event displays, detector grids, circuit-board panels, control-room screens, or observational data products unless based on a real cited source.
- Prefer explanatory scientific illustration over dramatic fantasy art.
- Keep colors restrained: white/light grey backgrounds for schematics; deep navy/black only where a space background is needed; teal/cyan accents and small warm disk highlights are acceptable.
- Avoid purple-gradient portfolio aesthetics, neon glow overload, lens flares, huge beams, particle-spray fireworks, and dense starfields.
- Leave visual breathing room near edges so the image works in responsive website layouts.
- The physical story must be clear without labels: source -> jet/outflow -> interaction/transport/detection concept.

Current generated image assessment:

- `jet-medium-interaction.png`: closest to usable. It has a clear jet and interaction region, but the right side is still too decorative. Improve by making the shock/contact discontinuity cleaner and reducing random glowing particle tracks.
- `microquasar-hero.png`: visually strong but too cinematic. The jet is over-bright and the system looks more like sci-fi artwork than a NASA/ESA explanatory artist's impression.
- `microquasar-smbh-comparison.png`: too cinematic and scale is not scientifically communicated. The SMBH side looks like a dramatic galaxy poster, not a controlled comparison schematic.
- `multimessenger-pipeline.png`: do not use as-is. The detector-like panels on the right look fake and imply real instrumentation/data. Replace them with abstract response curves or generic telescope/detector silhouettes only if needed.
- `blog-research-notes-header.png`: acceptable as an abstract header, but it is too generic AI/network imagery. Make it quieter and more astrophysics-specific.

## 1. Microquasar Hero Figure

- **Filename:** `images/microquasar-hero.webp`
- **Use:** Homepage hero or top visual context image
- **Aspect ratio:** `16:9`
- **Recommended size:** `1920 x 1080 px`
- **Crop priority:** compact binary, accretion disk, and both jet directions must remain visible after mild center-cropping
- **Caption idea:** `Artist's impression of a microquasar: a stellar-mass black hole accretes from a companion star and launches relativistic jets.`

Prompt:

```text
Create a NASA/JPL-style scientific artist's impression of a microquasar for an academic astrophysics website. Show a stellar-mass black hole accreting gas from a companion star through a compact accretion disk. Show two narrow, collimated relativistic jets perpendicular to the disk. The companion star, mass-transfer stream, accretion disk, compact object, and jet axis should be physically readable. Use a restrained public-science illustration style: clear forms, moderate contrast, subtle disk glow, limited star background, no cinematic lens flare, no fantasy wormhole, no huge energy beam. The image should feel like an official NASA or ESA science outreach graphic, not science fiction. No text labels, no logos, no fake data, no watermark. 16:9 composition, centered source, enough quiet space around the edges for responsive website cropping.
```

Negative prompt:

```text
Do not create a dramatic sci-fi poster, fantasy black hole portal, oversized glowing beam, dense starfield, explosion, spacecraft, planets, equations, labels, UI panels, or fake observational image.
```

Reject/regenerate if:

- The black hole looks like a giant cinematic wormhole instead of a compact accreting object.
- The jets are wide blue flames or magical beams rather than collimated outflows.
- The companion star and accretion geometry are unclear.
- The image includes labels, equations, plots, logos, or fake telescope data.

## 2. Jet-Medium Interaction Schematic

- **Filename:** `images/jet-medium-interaction.webp`
- **Use:** Research page current-project figure
- **Aspect ratio:** `4:3`
- **Recommended size:** `1600 x 1200 px`
- **Crop priority:** jet termination region and bow shock/contact discontinuity should be near center-right
- **Caption idea:** `Schematic jet-medium interaction region where shocks and particle transport can shape gamma-ray and neutrino signatures.`

Prompt:

```text
Create an ESA-style scientific schematic of a microquasar jet interacting with the surrounding interstellar medium. Show a compact source on the left launching one narrow, collimated jet into a diffuse ambient medium. The jet should terminate in a clear shock/contact region with a bow-shock-like boundary and a downstream turbulent cocoon. Add only a small number of subtle particle trajectories to suggest accelerated particles, gamma rays, and neutrinos; keep them sparse and physically suggestive, not decorative. Use a clean light grey or white background, restrained blue-grey gas textures, and small warm highlights at the shock. Make the structure readable like an official science outreach figure. No text labels, no fake detector elements, no circuit-board panels, no fake plots, no logos, no watermark. 4:3 composition.
```

Negative prompt:

```text
No explosion scene, no fireball, no sci-fi force field, no excessive glowing particle spaghetti, no spacecraft, no planets, no detector grid, no fake data, no labels.
```

Reject/regenerate if:

- It becomes an explosion scene rather than a jet/shock schematic.
- Particle trajectories dominate the image instead of the jet-medium structure.
- It shows detector panels, circuit grids, planets, spacecraft, or unrelated sci-fi elements.
- The shock/contact region is not visually clear.

## 3. Multi-messenger Pipeline Figure

- **Filename:** `images/multimessenger-pipeline.webp`
- **Use:** Homepage or blog explainer figure
- **Aspect ratio:** `21:9`
- **Recommended size:** `2100 x 900 px`
- **Crop priority:** all four stages should remain visible on desktop; center crop should still show stages 2 and 3
- **Caption idea:** `Conceptual workflow connecting jet emission, interaction regions, Galactic transport, and detector-space predictions.`

Prompt:

```text
Create a clean ESA/NASA-style horizontal scientific workflow illustration for a high-energy astrophysics website. Show four visually connected stages without text labels: 1) a compact microquasar source with accretion disk and jet, 2) a jet termination shock and turbulent interaction region, 3) sparse Galactic particle transport paths through diffuse gas, and 4) generic detector-space prediction represented only by simple abstract response curves or minimal telescope/detector silhouettes. The fourth stage must not look like real detector data or a specific instrument. Use a white/light grey background, restrained blue-grey gas textures, teal/cyan trajectories, and small warm highlights at acceleration sites. Keep the figure calm, explanatory, and physically readable, like an official space-agency public-science schematic. No text labels, no fake axes with numbers, no fake spectra, no detector grids, no circuit boards, no logos, no watermark. Panoramic 21:9 composition.
```

Negative prompt:

```text
No fake detector panels, no control screens, no circuit-board arrays, no data plots with axes, no instrument logos, no dramatic nebula poster, no dense particle spaghetti, no labels.
```

Reject/regenerate if:

- The four stages are not visually distinct.
- The detector stage looks like real data or fake hardware.
- It contains text inside the image.
- It looks like a corporate AI/network infographic rather than an astrophysics schematic.

## 4. Microquasar-SMBH Comparison Figure

- **Filename:** `images/microquasar-smbh-comparison.webp`
- **Use:** Research page or blog post comparing mass scales
- **Aspect ratio:** `16:9`
- **Recommended size:** `1920 x 1080 px`
- **Crop priority:** both panels should remain balanced after resizing
- **Caption idea:** `Artist's impression comparing jet-launching accretion systems across stellar-mass and supermassive black-hole scales.`

Prompt:

```text
Create a restrained NASA/ESA-style split-panel scientific artist's impression comparing a microquasar and an active galactic nucleus. Left panel: a stellar-mass black hole binary with companion star, mass-transfer stream, compact accretion disk, and narrow jets. Right panel: a supermassive black hole accretion disk at a galactic nucleus with a collimated jet and a subdued host-galaxy environment. The comparison should communicate similar jet-launching physics at different mass scales without exaggerating either system. Use matched viewing angles where possible, balanced brightness, and a calm public-science illustration style. Avoid cinematic poster lighting and dense starfields. No text labels, no scale bars, no logos, no fake EHT/radio texture, no fake data, no watermark. 16:9 composition with a simple clean division between panels.
```

Negative prompt:

```text
No giant fantasy galaxy poster, no over-bright blue energy columns, no impossible scale mixing, no labels, no equations, no fake telescope image texture, no logo, no watermark.
```

Reject/regenerate if:

- The two systems are not clearly different in physical context.
- The SMBH side looks like an uncited observational image or sci-fi galaxy wallpaper.
- The jets become decorative beams rather than collimated outflows.
- It adds labels, logos, or fantasy effects.

## 5. Blog Header: Research Notes

- **Filename:** `images/blog-research-notes-header.webp`
- **Use:** Optional blog index/header image
- **Aspect ratio:** `3:1`
- **Recommended size:** `1800 x 600 px`
- **Crop priority:** abstract jet/transport motif should remain visible across the full width
- **Caption idea:** usually no caption needed if used as a decorative blog header

Prompt:

```text
Create a quiet, official-science-style abstract header image for an astrophysics research blog. Use subtle motifs from compact-object jet physics: a small accretion-flow silhouette at one side, a faint collimated jet or transport path across the frame, and sparse particle trajectories fading into a clean light background. The result should feel like a NASA/ESA science webpage header, not a generic AI network banner. Use white, pale grey, blue-grey, and restrained teal accents. Keep it minimal, calm, and readable behind or above text. No text, no equations, no fake charts, no circuit-board network, no logos, no watermark, no dramatic fantasy scene. Very wide 3:1 aspect ratio.
```

Negative prompt:

```text
No generic technology network, no neural-network/circuit-board pattern, no dramatic black-hole poster, no dense nodes, no fake plots, no text, no labels.
```

Reject/regenerate if:

- It looks like a generic AI technology banner.
- It includes circuit-board or neural-network imagery unrelated to astrophysics.
- It is too visually busy for a blog header.
- The compact-object/jet motif is not recognizable.

## Suggested Replacement Order

1. Regenerate `microquasar-hero.webp`; current output is too cinematic.
2. Keep the idea of `jet-medium-interaction.webp` but regenerate with a cleaner shock/contact region and fewer decorative particle tracks.
3. Regenerate `multimessenger-pipeline.webp`; current detector panels should not be used.
4. Regenerate `microquasar-smbh-comparison.webp`; current version is too poster-like and not controlled enough scientifically.
5. Regenerate `blog-research-notes-header.webp` only if the blog page needs a visual header; current one is serviceable but generic.

When you return generated images, send the files or exact filenames you want to use, and I can wire them into the site with captions and alt text.
