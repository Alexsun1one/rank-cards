# QA Checklist

## Accept

Every PASS must be justified by something visible in the RENDERED file, not by the plan you
wrote. If your only evidence is the prompt, the item is UNVERIFIED — regenerate or inspect, do
not accept. Run these three falsifiable image-level tests first; they decide the gates.

- **Squint/thumbnail test (falsifiable):** produce an actual 2cm-wide (≈200px) downscaled copy
  of the finished card and look at THAT, not the full-size image. In one second, (a) read the
  title, (b) read the top-tier name(s), and (c) name which subject is ranked #1 by position /
  size / color ALONE — without reading any label. If any of the three fails, regenerate; do not
  accept on the full-size image. If you cannot generate or view a real thumbnail, you have not
  run this test — do not check it off.
- **Blur-the-faces unity test (falsifiable):** apply a heavy blur or shrink so faces are
  unreadable, then scan the portrait row. If ANY single cell pops out — a different crop scale,
  a leftover rectangular photo background, a brighter/cooler tint, a ringed face among bare ones
  — the pipeline failed; pull that cell back through the five locks (crop / background /
  treatment / edge / register). "Could not have come from one studio" is decided HERE, on the
  image, not by reading the plan.
- **Next-to-a-real-card test (falsifiable):** name one real reference in this exact register —
  a real FIFA/Panini card for sports, a real 文人画 album leaf for poets, a real
  university-crest poster for schools. Placed beside it, does this card look more amateur —
  looser type, muddier tiers, collage seams? If yes, regenerate. If you cannot name a real
  reference, you do not know this register's bar — find one before accepting.

Supporting checks (still must hold on the rendered image):

- **Asset-routing checks:** the chosen role (GOAT pyramid / top-N / tier-list / before-after /
  carousel page) is visible; wrong-owner jobs were rerouted (quote → quote-cards, cover-only →
  cover-pop, org structure → lego-town, cooperation → busy-town) instead of forced into a rank
  card. See `asset-routing-and-truth.md`.
- **Exact-order contract (falsifiable):** diff rendered names, tiers, and scores against the
  locked plan table. Invented ranks, swapped order, dropped/extra names, or fabricated scores
  fail — regenerate. Covers may show a subset but must not contradict carousel inner pages.
- The basis and scope are printed on the card and defensible (credibility gate).
- The tier system is one vocabulary, parallel in form, 3–6 tiers, top tier scarce.
- Color encodes rank correctly FOR THIS DOMAIN: for S/A/B/C and 段位/GOAT systems, a warm→cool
  ramp (red→blue) at consistent saturation; for non-pass/fail domains (城市/专业/学校, quality
  bands like 一线/二线, 王牌/天坑), a SINGLE-HUE value ramp (one accent, dark/saturated top →
  light bottom) — a warm→cool ramp on these is a WRONG, misleading traffic light and must
  regenerate.
- **Text exact-match test (falsifiable):** lay the rendered title, basis line, and EVERY subject
  name side by side with the plan text. They must match character-for-character — no extra,
  melted, or doubled glyphs, no name swapped between tiers. If the model could not render any of
  them cleanly, shorten the text and regenerate or run a text-fix edit. Empty plates plus editor
  overlay are allowed only when the user explicitly asks for editable/post-production text.
  A rendered-but-wrong glyph is a regenerate, never an accept. Label budgets follow
  `text-strategy.md`.
- **Name-readability test:** at the 2cm squint test above, every subject name must be readable;
  if any name only resolves at full size, put it on a higher-contrast plate at the shared size
  and baseline and regenerate.
- Rank numerals are legible on top of portraits.
- The layout has one clear focal structure (covers). Cover vs carousel ratio follows
  `layout-handoff.md` (default cover 3:4; dense grids stay inner).
- Era and affiliation (jersey/prop) are consistent across all subjects.
- Portraits are not AI-plastic (waxy identical faces / beauty-filter sheen) and pass the unity
  pipeline.
- Scan `failure-patterns.md` before accept: invented ranks, sports-only template lock,
  unreadable names, wrong order, plastic portraits.
- If this is a README/gallery/showcase card, the visual register proves domain routing. A tea, poetry, city, book, or tool ranking should not look like a sports trading card unless the user explicitly asks for that tension.

## Regenerate

- Names, order, tiers, or scores were invented or disagree with the exact-order contract.
- Portraits are a collage: mismatched crops, backgrounds, lighting, or art styles.
- Original photo backgrounds are still behind cut-out subjects.
- A painted portrait sits next to a modern photo next to a cartoon.
- AI plastic portraits / waxy identical faces break the register.
- One soft, low-res, or watermarked face among sharp ones.
- The ranking has no stated basis or scope.
- Sports-only chrome was applied to a non-sports domain without an explicit override.
- The color ramp is wrong for the domain: warm→cool used on a 城市/专业/学校/quality-band card
  (a false red-green traffic light), OR no monotonic rank-encoding ramp at all.
- Tiers sprawl past 6, or labels mix forms (S / 天王 / 二流 together).
- The top tier is overcrowded — scarcity is lost.
- Names or numbers are unreadable at thumbnail size.
- A dense tier-row/grid was used as a short-video cover and fails the squint test.
- It looks like a bare default tier-maker (gray rows, clip-art).
- One subject is in club colors and another in national team, with no reason.
- The job belonged to quote-cards / cover-pop / lego-town / busy-town and should be rerouted.

## Repair Moves

If portraits look like a collage:

```text
Pull every portrait through one pipeline: same crop (all chest-up, eyelines aligned), one
shared background, one duotone treatment, same edge. Knock out every original background.
Render all subjects in one consistent pass.
```

If ranks were invented or order is wrong:

```text
Reject the card. Re-lock the exact-order contract (name | tier-or-# | score). Regenerate with
Exact text / Exact order blocks only — no filler GOAT, no swapped cells, no fabricated chips.
```

If the ranking feels arbitrary:

```text
Add a printed basis line and scope: pick one primary criterion (+ optional weights) and state
现役/历史 · 位置 · 俱乐部/国家队. Print it under the title.
```

If sports chrome locked onto a non-sports subject:

```text
Re-route with style-routing.md. Rebuild inside the correct register (ink-wash / crest /
editorial / single-hue value ramp). Do not keep duotone FIFA chrome as a default.
```

If portraits look AI-plastic:

```text
Regenerate through one portrait pipeline with harder negatives against waxy skin, beauty-filter
faces, and identical smile templates. Prefer illustrated/editorial unity over fake photo-real.
```

If tiers sprawl or labels are mixed:

```text
Cut to 3-5 tiers, one vocabulary, parallel form. Keep the top tier to 1-3 names. Apply the
rank-encoding ramp FOR THIS DOMAIN: warm→cool at consistent saturation for S/A/B/C and 段位/GOAT
systems; a single-hue value ramp (dark/saturated top → light bottom) for 城市/专业/学校 and
quality bands, where warm→cool reads as a false traffic light.
```

If text is unreadable or garbled:

```text
Re-render the title, basis line, and all names as exact clean Chinese characters. Put names on
high-contrast plates at one size and baseline. Outline big numerals. If clean text is still
impossible, simplify labels and regenerate; leave plates empty only when the user explicitly
requests editable/post-production text.
```

If it looks like a default tier-maker:

```text
Replace the chrome: a real title, refined warm→cool palette at consistent saturation, unified
portrait treatment, and proper type hierarchy. Escape the bare gray-row look.
```

If the job is the wrong owner:

```text
Reroute: single quote → quote-cards; non-ranking cover → cover-pop; org/module structure →
lego-town; multi-role cooperation → busy-town. Say the better owner; do not force a tier card.
```
