# Rank Cards

> A skill for generating opinionated, readable ranking cards for sports, products, creators, tools, and ideas.

Rank Cards turns a ranked list into a publishable social card with hierarchy, badges, reasons, and a clear ranking logic. It is built for Chinese content where the image must be instantly scannable.

## Examples

<p><img src="examples/images/world-football-forwards-ranking-cr7-first.png" alt="World football forwards ranking" width="100%"><br><sub>World football forwards ranking</sub></p>

## What It Does

- Design top-N ranking cards with clear winner hierarchy and supporting rationale.
- Choose layouts for sports cards, tier lists, product comparisons, and creator/tool rankings.
- Keep names, numbers, badges, and reason lines readable on mobile.
- Make the ranking stance explicit instead of pretending to be neutral data.

## Install

Clone this repository into your local Codex skills folder:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/Alexsun1one/rank-cards.git ~/.codex/skills/rank-cards
```

If your agent expects a nested skill directory instead of a direct clone, copy the folder that contains `SKILL.md` into its skills directory.

## Use

Example request:

```text
Use rank-cards to make a 3:4 Chinese Top 10 ranking card. Topic: 世界足坛前锋历史排名. Put C罗 at #1 and include the ranking basis line.
```

The skill entry point is [`SKILL.md`](SKILL.md). Supporting rules live in [`references/`](references/) when this repo includes them; helper scripts live in [`scripts/`](scripts/) when available.

## Quality Bar

- The image must explain a concrete idea, not merely decorate the page.
- Chinese text should be readable at the actual publishing size.
- The output should keep a stable style system across a set while letting each image fit its topic.
- Generated examples are prompts and visual references, not fixed templates.

## WeChat

More writeups, examples, and AI workflow notes are published on my WeChat official account. This is the real QR/search card used for the account, included as a normal bitmap asset rather than a stylized fake code.

<p align="center">
  <img src="assets/wechat-official-account.png" alt="微信搜一搜：正在逐渐AI化" width="720">
</p>

## License

MIT. See [`LICENSE`](LICENSE).

## Notice

This is an original open-source skill package by Sun Wuyuan / Alexsun1one. It is not affiliated with OpenAI, GitHub, WeChat, or any referenced platform. Avoid using it to imitate protected characters, living artists, or third-party brand assets without permission.
