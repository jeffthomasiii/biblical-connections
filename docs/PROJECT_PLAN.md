# Biblical Connections — Implementation Plan

## Purpose
An interactive, Scripture-first visualization library hosted on GitHub Pages. Visitors explore relationships and download SVG and high-resolution PNG rendered from the live visualization, not static pre-generated artwork.

## Initial collection
1. Tree of Life: Genesis to Revelation (first release)
2. Bible cross-reference network
3. Kings and prophets timeline
4. Old Testament in Revelation
5. Covenants of Scripture

## Proposed stack
React + TypeScript + Vite + SVG/D3, deployed with GitHub Actions to GitHub Pages at `/biblical-connections/`. Prefer structured, reviewable JSON/TypeScript passage data. Browser-based SVG export and high-resolution PNG rendering.

## First visualization: Tree of Life
**Direct mentions:** Genesis 2:9; 3:22,24; Revelation 2:7; 22:2,14 (also Revelation 22:19, with manuscript variation to research).

**Figurative uses:** Proverbs 3:18; 11:30; 13:12; 15:4.

**Related imagery, not direct references:** Ezekiel 47:1–12; compare Revelation 22:1–2. Additional Christological associations require careful interpretive labeling.

**Text-critical notes:** Revelation 22:14 has a variant ('wash their robes' / 'do his commandments'); Revelation 22:19 has a variant ('tree of life' / 'book of life'). Research and cite critical editions before definitive treatment.

## UX requirements
- Home page with five visualization cards, progress indicators, research method.
- Tree of Life interactive reference map, keyboard accessible and responsive.
- Select passage to see context, evidence class, and interpretation note.
- Toggle direct mentions versus metaphorical and thematic connections.
- Export clean SVG and print-resolution PNG from current view.
- Sources and methodology page, with explicit labels for direct statements, inference, and debated readings.

## Milestones
1. Scaffold application, design system, GitHub Pages deployment.
2. Curate verse dataset and validate wording/textual variants.
3. Build interactive Tree of Life visualization and study panels.
4. Add image export, responsive layout, accessibility checks.
5. Test deployment and publish first release.

## Acceptance criteria
`npm run build` passes; Pages site loads on repository subpath; selected verses and filters update the visualization; exported images reflect selected view; research notes distinguish textual statements from inference; no unsupported biblical imagery or claims.
