# Figure Prompts

Use these prompts to generate original, website-safe scientific illustrations for `hw-si.github.io`. They are written for schematic/editorial science figures, not for fake observations or fake plots.

General requirements for every image:

- Export as `.webp` if possible; `.png` is also acceptable.
- Use lowercase filenames with hyphens, saved under `images/`.
- No text labels inside the image. Captions will be written in HTML/Markdown.
- No institutional logos, telescope logos, collaboration logos, fake signatures, or watermarks.
- No fake plot axes, false-color maps, detector event displays, spectra, or observational data products unless based on a real cited source.
- Prefer clean scientific schematic clarity over cinematic fantasy art.
- Keep colors restrained: black, deep navy, white, grey, cyan/teal accents, and small warm highlights are fine.
- Avoid purple-gradient portfolio aesthetics; the site should feel academic and research-focused.
- Leave visual breathing room near edges so the image works in responsive website layouts.

## 1. Microquasar Hero Figure

- **Filename:** `images/microquasar-hero.webp`
- **Use:** Homepage hero or top visual context image
- **Aspect ratio:** `16:9`
- **Recommended size:** `1920 x 1080 px`
- **Crop priority:** central compact binary and bipolar jets must remain visible after mild center-cropping
- **Caption idea:** `Schematic view of a microquasar: accretion onto a stellar-mass black hole launches relativistic jets.`

Prompt:

```text
Create a clean scientific editorial illustration of a stellar-mass black hole binary microquasar for an academic astrophysics website. Show a compact black hole accreting gas from a companion star through a luminous accretion disk, with two narrow relativistic jets emerging perpendicular to the disk. The system should be scientifically plausible, with a restrained dark space background, subtle accretion glow, and clear jet geometry. Use a modern academic schematic style, not fantasy art. No text labels, no logos, no fake data axes, no observatory imagery, no watermark. Composition must work as a 16:9 website hero image with the binary and jets centered and enough negative space around the edges.
```

Reject/regenerate if:

- The black hole looks like a giant cinematic wormhole rather than a compact accreting object.
- The jets are wide flames instead of collimated relativistic outflows.
- The image includes labels, equations, plots, logos, or fake telescope data.

## 2. Jet-Medium Interaction Schematic

- **Filename:** `images/jet-medium-interaction.webp`
- **Use:** Research page current-project figure
- **Aspect ratio:** `4:3`
- **Recommended size:** `1600 x 1200 px`
- **Crop priority:** jet termination region and bow shock should be near center-right
- **Caption idea:** `Schematic jet-medium interaction region where shocks and particle transport can shape gamma-ray and neutrino signatures.`

Prompt:

```text
Create a scientific schematic illustration of a relativistic jet from a microquasar propagating into the surrounding interstellar medium. Show a narrow jet, a jet termination region, a bow shock, a turbulent interaction zone, and subtle particle trajectories representing accelerated cosmic rays and neutrino/gamma-ray production. The visual style should be clean, academic, and physically motivated, with muted colors and high contrast. Use a light or neutral background suitable for a research webpage. No text labels, no arrows with words, no fake data, no institutional logos, no telescope logos, no watermark. Composition should fit a 4:3 research figure, with the source on the left and the interaction region near the center-right.
```

Reject/regenerate if:

- It becomes an explosion scene rather than a jet/shock schematic.
- It shows planets, spacecraft, or unrelated sci-fi elements.
- It includes labels, fake plots, or unrealistic colored detector overlays.

## 3. Multi-messenger Pipeline Figure

- **Filename:** `images/multimessenger-pipeline.webp`
- **Use:** Homepage or blog explainer figure
- **Aspect ratio:** `21:9`
- **Recommended size:** `2100 x 900 px`
- **Crop priority:** all four stages should remain visible on desktop; center crop should still show stages 2 and 3
- **Caption idea:** `Conceptual workflow connecting jet emission, interaction regions, Galactic transport, and detector-space predictions.`

Prompt:

```text
Create a horizontal scientific workflow illustration for a high-energy astrophysics website. Show four connected visual stages without text labels: 1) compact-object jet emission from a microquasar, 2) jet termination and shock interaction region, 3) Galactic particle transport with subtle curved trajectories, and 4) abstract detector-space predictions for gamma rays and neutrinos. Use physically motivated schematic elements, clean spacing, and a white or very light background. Use restrained colors with teal/cyan accents and small warm highlights. No written labels, no fake axes, no fake spectra, no real observatory logos, no institutional logos, no watermark. Composition must be panoramic 21:9 and suitable for a wide homepage or blog banner.
```

Reject/regenerate if:

- The four stages are not visually distinct.
- It contains text inside the image.
- It looks like a corporate infographic rather than a scientific schematic.

## 4. Microquasar-SMBH Comparison Figure

- **Filename:** `images/microquasar-smbh-comparison.webp`
- **Use:** Research page or blog post comparing mass scales
- **Aspect ratio:** `16:9`
- **Recommended size:** `1920 x 1080 px`
- **Crop priority:** both panels should remain balanced after resizing
- **Caption idea:** `Schematic comparison of jet physics across stellar-mass and supermassive black-hole systems.`

Prompt:

```text
Create a split-panel scientific illustration comparing a microquasar jet and a supermassive black-hole jet. The left side should show a stellar-mass black hole binary with an accretion disk and compact relativistic jets. The right side should show a supermassive black hole accretion flow with a much larger relativistic jet, suggesting similar jet physics across different mass scales. Use a clean academic schematic style with realistic but simplified accretion flows. Keep the two panels visually balanced, restrained, and readable. No text labels, no logos, no fake data axes, no telescope image textures, no watermark. Composition must fit a 16:9 website figure.
```

Reject/regenerate if:

- The two systems are not clearly different in scale.
- It uses real-looking EHT/radio data textures without citation.
- It adds labels, logos, or decorative fantasy effects.

## 5. Blog Header: Research Notes

- **Filename:** `images/blog-research-notes-header.webp`
- **Use:** Optional blog index/header image
- **Aspect ratio:** `3:1`
- **Recommended size:** `1800 x 600 px`
- **Crop priority:** abstract jet/network motif should remain visible across the full width
- **Caption idea:** usually no caption needed if used as a decorative blog header

Prompt:

```text
Create a restrained abstract scientific header image for an astrophysics research blog. Use visual motifs of compact-object jets, particle trajectories, and faint network-like paths suggesting modeling and multi-messenger inference. The image should be subtle, academic, and suitable behind or above blog content on a white website. Use dark navy, grey, white, and teal accents. No text, no equations, no fake charts, no logos, no watermark, no dramatic fantasy scene. Composition must be very wide, 3:1 aspect ratio, with enough quiet negative space for a website header.
```

Reject/regenerate if:

- It looks like a generic AI technology banner.
- It includes circuit-board imagery unrelated to astrophysics.
- It is too visually busy for a blog header.

## Suggested Replacement Order

1. Generate `microquasar-hero.webp` first for the homepage.
2. Generate `jet-medium-interaction.webp` for the Research page.
3. Generate `multimessenger-pipeline.webp` only if you want a clearer workflow visual.
4. Generate `microquasar-smbh-comparison.webp` for a future explainer or blog post.
5. Generate `blog-research-notes-header.webp` only if the blog page needs a visual header.

When you return generated images, send the files or exact filenames you want to use, and I can wire them into the site with captions and alt text.
