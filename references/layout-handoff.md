# Layout Handoff / 版式交接

Use this reference when a Rank Card will ship as a short-video cover, carousel page, README figure, article embed, slide, or social post.

Rank Cards create the **ranking surface**. The outer layout may own the debate paragraph, citations, CTA, and platform chrome — but for short-video covers, native title/basis/names usually stay inside the image.

## Handoff Fields

Return these fields when planning a generated asset:

```text
final container:
asset role:
layout archetype:
recommended ratio:
safe margin:
headline inside image: yes/no
caption outside image:
crop guidance:
exact order contract locked: yes/no
handoff owner:
```

## Short-Video Cover Vs Carousel

| Container | Ratio | Layout bias | Notes |
| --- | --- | --- | --- |
| 视频号 / 抖音 / 小红书 **cover** | **3:4** (1080×1440) | podium / versus / single-hero / pyramid; tier-row only if ≤3×4 | must pass 2cm thumbnail: title + #1 readable |
| Carousel **inner** page | **3:4** or **1:1** | tier-row / ranked grid / single-hero per page | denser OK; still one pipeline |
| Grid carousel / square post | **1:1** | Top-6/9 grid or compact tier-row | equal cell weight |
| YouTube / landscape hero | **16:9** | podium or versus with side margin | leave quiet zones if outer title exists |
| README / article figure | 16:9 or 3:4 | any archetype that survives shrink | caption outside may carry source |
| Slide center image | 16:9 or 4:3 | center illustration mode if slide owns title | safe margins |

### Cover rules

- One focal structure. If the layout becomes noise at thumbnail size, it is a carousel page, not a cover.
- Prefer crowning a winner (podium / pyramid / versus / single-hero) on page 1.
- Keep the exact-order contract identical across cover and inner pages — covers may show a subset, never a conflicting order.

### Carousel rules

- Page 1 = hook (winner / debate / scarcity).
- Later pages = full tier-row, Top-N grid, or one-subject hero cards.
- Do not change basis mid-carousel unless a page is explicitly labeled as a different criterion.

## Text Ownership

### Image Owns

- title, basis, tiers, rank numerals, names, short chips (see `text-strategy.md`)

### Outer Layout Owns

- long debate copy, citations, CTA, series title cards that are not the ranking table

If a generated cover already contains a paragraph, regenerate with fewer labels instead of relying on layout cropping.

## Crop & Margin Rules

- Keep the **#1 / apex / VS conflict** in the central 70%.
- Tier caps on the left need left safe margin; name plates need bottom safe margin for platform UI chrome.
- Before/after spreads need a clear gutter that survives center crop.
- Prefer regenerating a simpler cover over asking the editor to crop chaos.

## Handoff Notes

In final delivery, include:

- full image path
- aspect ratio
- exact native text rendered (title / basis / tiers / names / scores)
- recommended outside caption (source / debate context)
- crop warnings
- whether the card survives phone thumbnail

## Anti-Patterns

- shipping a dense 10-row tier list as the cover
- stuffing the README title into the card and also into the markdown heading as conflicting claims
- assuming the carousel will "explain the real order" while the cover invents a different Top-3
- handing off a text-empty collage and expecting the caption to carry the ranking
