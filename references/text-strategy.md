# Text Strategy / 文字策略

Use this reference whenever title, basis line, tier labels, rank numerals, subject names, or score chips matter.

Rank cards die two ways with text: too little (pretty portraits, no claim) and too much (paragraphs stuffed into cells). Prefer **native text** rendered by the image model inside the card pixels. Editor overlay is not the default.

## Label Budget By Asset Role

| Asset role | Label budget | What the labels name |
| --- | --- | --- |
| GOAT Pyramid | title + basis + 1 tier label per band + names | apex scarce; short names only |
| Top-N List | title + basis + `#N` + names (+ optional 1 score chip each) | order first; chips secondary |
| Tier List | title + basis + 3–6 tier caps + names | parallel-form tier vocab only |
| Before / After Rank | 1 banner per panel + shared basis + names | delta must be readable without a paragraph |
| Carousel cover | title + basis + top 1–3 names | survive 2cm thumbnail |
| Carousel inner | denser names/chips OK | still one size/baseline per row |
| Center illustration for outer layout | 0–4 short labels | outer layout owns headline |

Chinese names: prefer the **shortest recognizable form** that still matches the exact-order contract (e.g. `梅西` not a full legal name unless the user locked it). Longer strings melt first.

## Good Label Shapes

Prefer:

- **title**: one ranking question, ≤12 Chinese chars when possible
- **basis line**: one printed criterion + scope (`按巅峰统治力 · 仅限现役中后卫`)
- **tier caps**: one vocabulary, parallel form (`S/A/B/C` or `神品/逸品/妙品`)
- **rank numerals**: oversized `#1` `#2` on Top-N / podium
- **name plates**: high-contrast plate, one size, one baseline per row
- **score chips**: short (`金球×8`, `89分`) — only if supplied

Avoid:

- full sentences inside cells
- mixing letter tiers with noun tiers on one card
- tiny captions on busy chrome or photo texture
- inventing score chips to "look official"
- doubled / melted / swapped glyphs
- empty plates + silent overlay unless the user explicitly asked for editable text

## Exact Text Block

For final prompts, state:

```text
Exact text: include only these strings:
- title: "…"
- basis: "…"
- tiers: "…", "…", "…"
- names in exact order: "…", "…", "…"
- scores (if any): "…"
No other text, no fake paragraphs, no watermark, no publisher logo.
```

## Text Ownership Split

### Image Owns (native text first)

- title, basis/scope line
- tier labels and rank numerals
- subject names on plates
- short score / affiliation chips that belong to a cell

### Outer Layout Owns

- long explanation / debate paragraph
- citations / source essay
- CTA / author note
- platform metadata
- carousel page captions that are not part of the ranking table

## Repair Policy

If portraits are good but text is wrong:

1. One regeneration with a stricter exact-text block and shorter names.
2. Put names on larger high-contrast plates; outline big numerals.
3. If Chinese is still unstable and the user explicitly wants editable text, regenerate with blank plates of the right shape/size and overlay in post — note this in the output contract.
4. Never silently accept invented ranks, swapped names, or melted glyphs on public/showcase cards.

## Anti-Patterns

- stuffing title + subtitle + basis essay + 12 chips into one cover
- leaving names off "so portraits look cleaner"
- English tier jargon on a Chinese audience card without reason
- accepting a beautiful card whose order does not match the exact-order contract
