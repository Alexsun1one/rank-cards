# Asset Routing And Truth / 资产路由与事实约束

Use this reference before final prompt writing when the source is more than a vague "做个排名卡": a named list, published ranking, debate thread, stats table, before/after claim, carousel brief, or social-card package.

Rank Cards is a **ranking / tier judgment** system, not only a sports-card style. The first question is not "what should the chrome look like?" but "what job must this ranking image do in the final artifact?"

## Core Rule

Keep Rank Cards only when **ordered comparison** (rank, tier, GOAT scarcity, or before/after placement) is the meaning.

If the final need is a single quote, a clickbait cover without a ranking claim, an org/system structure diagram, or a multi-role cooperation story, do not force Rank Cards to own the whole job. Use Rank Cards for the ranking surface; let quote-cards, cover-pop, lego-town, or busy-town do their own work.

## Asset Roles

Pick one role before choosing layout archetype or style register.

### GOAT Pyramid

Use for scarcity-at-the-top claims: GOAT, 历史地位金字塔, 神品→能品 apex.

- Visual job: make the apex scarce and the drop-off obvious.
- Best form: pyramid archetype (`layout-archetypes.md`).
- Truth rule: exact apex names and exact band membership; never invent a GOAT to fill the tip.

### Top-N List

Use for ordered Top-5 / Top-10 / Top-20 where position matters more than tier bands.

- Visual job: make #1–#N order readable at a glance.
- Best form: ranked grid or podium (Top-3 cover); dense grids stay in carousel.
- Truth rule: exact names in exact order; scores/stats only if supplied.

### Tier List

Use for S/A/B/C, 神品/逸品, 一线/二线, or any banded judgment.

- Visual job: bucket many subjects into parallel-form tiers with a printed basis.
- Best form: tier-row list; cover only if ≤3 rows and ≤4 per row.
- Truth rule: exact tier vocabulary + exact subject→tier map; basis must govern placement.

### Before / After Rank

Use for "升了 / 掉了 / 重排后" claims — same subjects, changed order or tier.

- Visual job: make the single delta (who moved) obvious.
- Best form: two-panel or two-page spread sharing one template; only order/tier changes.
- Truth rule: both sides use the same subject set and the same printed basis unless the user explicitly changes the criterion.

### Carousel Page

Use when the ranking is a multi-page short-video / 小红书 carousel: cover hook + inner detail pages.

- Visual job: one focal claim per page (cover = winner/pyramid; inner = tier-row / grid / single-hero).
- Best form: cover archetype on page 1; denser layouts only after.
- Truth rule: every page that shows names/order must match the same locked ranking table — no page invents extras.

### Ranking Data Status (thin note)

Ranks are data. When scores, rates, trophy counts, or published list positions appear on the card, treat them like a data-status contract:

- Visual job: encode the ranking claim; numbers support it, they do not decorate it.
- Truth rule: list every score/order that appears; do not invent ranks, ties, or decimals.
- If the whole artifact is a rigorous chart with axes, use a native chart; Rank Cards can still own the portrait/tier surface around it.

Keep the **exact order contract** explicit in every plan:

```text
exact order contract:
1. {name} — {tier or #} — {score if any}
2. ...
Do not invent, swap, or drop any row.
```

## Routing Questions

Answer these before prompt writing:

```text
asset role: goat-pyramid / top-n / tier-list / before-after / carousel-page
final container: short-video cover / carousel / README / article / slide / other
display well or ratio:
text ownership: native-in-image / outer-layout / both
truth constraints: exact names / exact order / exact scores / printed basis / none
style register (from style-routing):
layout archetype:
if not Rank Cards, better owner:
```

## Truth Handling

### Must Be Exact — NEVER invent rankings

- subject names specified by the user or a cited source
- order (#1…#N) and tier membership
- scores, rates, trophy counts, or list positions that appear on the card
- the printed basis + scope line when the card claims a criterion
- before/after deltas (who moved where)

Put exact requirements in the final prompt:

```text
Exact text: title "{…}"; basis "{…}"; tiers "{…}"; names in this exact order: "A", "B", "C".
Exact order: do not swap, insert, or drop any subject.
Exact scores: only these values: ….
Do not invent rankings, ties, extra names, or fake stats.
```

### Can Be Symbolic

- portrait treatment inside the routed register (duotone, ink-wash, oil, etc.)
- warm→cool or single-hue ramp encoding (must still match domain rules)
- decorative chrome, medals, seals, crest motifs that do not change order
- era/jersey/prop choice when the user did not lock a specific photo

## What To Refuse Or Reroute

Reroute away from Rank Cards when:

- the user only needs a **single quote / number / feeling** → **quote-cards**
- the user needs a **clickbait cover** without a ranking claim → **cover-pop**
- the topic is **org / system / module structure** (who snaps to whom) → **lego-town**
- the topic is **multi-role cooperation / handoff process** → **busy-town**
- the asset is a strict chart with exact axes and the ranking surface is irrelevant
- the user needs a logo, sticker pack, or editable diagram only

In these cases, say the better owner plainly. Rank Cards may still supply a supporting ranking inset if the outer job stays with another skill.

## QA Additions

Before delivery, check:

- The chosen asset role is visible (pyramid scarcity / Top-N order / tier bands / before-after delta / carousel page job).
- Exact names, order, and scores were not invented, swapped, or misspelled.
- The exact order contract in the plan matches the rendered card character-for-character.
- Text ownership is respected (`text-strategy.md` / `layout-handoff.md`).
- Wrong-owner jobs were rerouted instead of forced into a sports tier template.
- Style register still follows `style-routing.md` (no sports-only lock on non-sports subjects).
