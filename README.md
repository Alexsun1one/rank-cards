# Rank Cards / 排名卡片

> 生成适合中文社交媒体传播的 Top 榜、分档榜、球星榜、产品榜和观点排名卡。

排名卡不是把列表贴到图上，而是要有明确口径、强层级、可争论的立场和手机上能读的视觉秩序。这个 skill 适合做体育、产品、AI 工具、创作者、书单、城市、公司、观点等排名内容。

## 示例图

<p><img src="examples/images/spring-tea-snacks-top7.png" alt="春日茶点人气榜" width="100%"><br><sub>生活方式榜单：排名卡不只适合球星，也适合食物、城市、书单和文化内容。</sub></p>
<p><img src="examples/images/world-football-forwards-ranking-cr7-first.png" alt="世界足坛前锋历史排名卡" width="100%"><br><sub>世界足坛前锋历史排名卡</sub></p>

## 它能做什么

- 把 Top-N 榜单做成 3:4、方图或横版排名卡。
- 突出第一名、分组层级、理由标签和排名依据。
- 为争议型排名写清“个人向 / 数据向 / 荣誉向 / 体验向”等口径。
- 生成适合短视频封面、公众号插图、小红书/朋友圈传播的排名视觉。

## 安装

把这个仓库克隆到本机 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/Alexsun1one/rank-cards.git ~/.codex/skills/rank-cards
```

如果你的 Agent 使用其它 skills 目录，也可以把包含 `SKILL.md` 的这个仓库复制过去。

## 怎么用

示例请求：

```text
用 rank-cards 做一张 3:4 中文排名卡：世界足坛前锋历史排名，C罗排第一。请写出排名依据线，并让手机缩略图也能看懂。
```

Skill 入口是 [`SKILL.md`](SKILL.md)。细则在 [`references/`](references/)；如果这个仓库带脚本，脚本在 [`scripts/`](scripts/)。

## 质量要求

- 先服务内容，再服务风格；图必须解释一个具体想法。
- 中文默认要可读，标题、caption、标签不能只当装饰纹理。
- 同一组图要风格统一，但每张图要贴合自己的段落/用途。
- 示例图是工作流参考，不是唯一模板。

## 公众号

更完整的拆解、提示词、案例复盘、AI 写作和产品实践，我会继续写在公众号里。下面是我的真实公众号二维码/搜一搜卡片，不是仿造的装饰二维码。

<p align="center">
  <img src="assets/wechat-official-account.png" alt="微信搜一搜：正在逐渐AI化" width="720">
</p>

## 开源协议

MIT。见 [`LICENSE`](LICENSE)。

## 声明

这是 Sun Wuyuan / Alexsun1one 的原创开源 Skill 包。它不隶属于 OpenAI、GitHub、微信或任何被提及的平台。请不要用它去复制受保护 IP、仿冒在世艺术家，或暗示不存在的品牌背书。
