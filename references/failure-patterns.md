# Failure Patterns / 失败模式库

Use this reference during QA and critique. A polished card can still fail. If one of these failures is present, do not describe the image as "mostly fine." Name the failure and either regenerate or reroute.

## Common Failures

### Invented Ranks

Symptom: names, order, tiers, or scores appear that the user/source did not supply; ties or decimals fabricated to fill cells.

Fix: reject. Lock the exact-order contract from `asset-routing-and-truth.md`; regenerate with only listed subjects. Never invent a GOAT to fill a pyramid tip.

### Sports-Only Template Lock

Symptom: poets, cities, schools, foods, or tools all render as duotone FIFA/Panini chrome with S/A/B/C warm→cool traffic lights.

Fix: re-route with `style-routing.md`. Non-sports domains need their register (ink-wash, crest, single-hue value ramp, etc.). Showcase packages must include at least one non-sports proof.

### Unreadable Names

Symptom: names only resolve at full size; melted/doubled glyphs; low-contrast type on busy portraits.

Fix: shorten to exact recognizable forms; high-contrast plates; one size/baseline; run text-fix edit or regenerate. See `text-strategy.md`.

### Wrong Order

Symptom: rendered Top-N or tier membership disagrees with the plan; two carousel pages disagree; before/after panels silently reshuffle unrelated names.

Fix: reject. Diff the rendered names against the exact-order contract character-for-character; regenerate. Covers may show a subset but must not contradict inner pages.

### AI Plastic Portraits

Symptom: waxy skin, identical smile templates, plastic sheen, mismatched identity, or "AI influencer" faces that break the routed register.

Fix: pull every subject through one portrait pipeline (`portrait-pipeline.md`); prefer illustrated/editorial unity over fake photo-real; regenerate with harder negatives against plastic skin / beauty-filter faces. Mixed photo+cartoon in one card is also a unity failure.

### Missing Basis / Scope

Symptom: the card looks authoritative but prints no criterion; fans cannot tell peak vs career, club vs country.

Fix: print a specific basis+scope line; run the credibility gate in `SKILL.md`. A basis that changes no placement is decoration.

### Collage / Pipeline Break

Symptom: one cell pops out by crop, tint, background, or edge; original photo rectangles remain.

Fix: blur-the-faces unity test; re-run five locks (crop / background / treatment / edge / register).

### Tier Sprawl / Mixed Vocabulary

Symptom: 7+ tiers, or `S` next to `天王` next to `二流` on one card; top tier overcrowded.

Fix: cut to 3–6 parallel-form tiers; keep apex scarce.

### Wrong Color Encoding

Symptom: warm→cool traffic light on 城市/专业/学校 quality bands; or no monotonic rank encoding at all.

Fix: use domain-correct ramp from `qa-checklist.md` / `style-routing.md`.

### Wrong Owner

Symptom: Rank Cards forced onto a single quote, a non-ranking cover, an org chart, or a cooperation process.

Fix: reroute — **quote-cards** / **cover-pop** / **lego-town** / **busy-town**. Say the better owner plainly.

### Text Overload

Symptom: title + subtitle + essay + legend + 12 chips on one cover.

Fix: `text-strategy.md` + `layout-handoff.md`; move debate copy outside; keep native ranking labels only.

### Default Tier-Maker Chrome

Symptom: bare gray rows, clip-art badges, amateur template look beside a real reference card.

Fix: next-to-a-real-card test; replace chrome; unify portraits; restore type hierarchy.

## Quick Triage

| If you see… | First open… |
| --- | --- |
| Invented / swapped order | `asset-routing-and-truth.md` |
| Sports look on non-sports | `style-routing.md` |
| Melted names | `text-strategy.md` |
| Cover too dense | `layout-handoff.md` |
| Plastic / collage faces | `portrait-pipeline.md` |
| Arbitrary tiers | `tier-and-criteria.md` |
