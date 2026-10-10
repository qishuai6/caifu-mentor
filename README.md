# caifu-mentor · 财富导师

> 把李笑来《财富自由之路》的 50 个概念，固化成一个随叫随到的 AI 校对员——你说出想法、行为或困惑，它用这本书的观点给出判决，并附上具体可执行的实施方法。

你手机里躺着无数篇「讲得都对、看完就忘」的成长干货。这个项目做的事不一样：**把一本书变成一个能持续审问你日常决策的对手。**

它不陪你聊人生。它的工作方式是每次校对都走完四段：

1. **结论** —— 一句话判决，先说，不和稀泥
2. **书怎么说** —— 逐字引用原文金句＋章节号（这是它的信誉来源，不编造、不改写）
3. **拆解你** —— 把你的陈述放上手术台：哪句话是证据，偏差在哪，锋利但不羞辱
4. **怎么办** —— 最多三条处方，每条都有动作、频率、检验标准，「保持耐心」这种废话禁止出现

## 一个例子

**你说**：我做了个副业账号，更新两个月没什么人看，我是不是不适合干这个？

**它答**：

> **结论**：「不适合」这个念头本身就是你此刻最大的敌人——它是全书点名的失败者墓志铭，而你的两个月，甚至还没走到能下任何结论的位置。
>
> **书怎么说**：「『也许我不适合干这事儿吧』绝对是一切失败者的墓志铭，甚至可以干脆改成『也许我不适合来到这个世界吧』」——第 4 章。「成长这个东西，只有突破了成本线才开始真正有意义，在那之前都是在挣扎……」——第 1 章。
>
> **拆解你**：你把「两个月没流量」当成了「我不行」的证据——这是用当下的反馈否定长期正确的方向。真正该检查的是三个事实问题：更新了多少篇？每篇有没有做「被看见」的动作？内容是「你以为的刚需」还是「读者以为的刚需」？
>
> **怎么办**：KPI 从阅读量改成发布量＋迭代次数，跑满 12 周再谈数据；每周做一次「被看见」动作；写下 12 周后的预测，封存到期对表。

## 安装

适用于 ZCode、Claude Code、Codex 及一切支持 SKILL.md 规范的 Agent：

```bash
git clone https://github.com/qishuai6/caifu-mentor.git ~/.agents/skills/caifu-mentor
```

或者手动复制本目录（SKILL.md＋references/）到你的 skills 目录（如 `~/.zcode/skills/`、`<project>/.agents/skills/`）。完全自包含，无任何外部依赖。

## 使用

对装了它的 Agent 说：

- 「校对我：我想辞职全职做自媒体」
- 「用财富自由之路看看这件事」
- 「李笑来会怎么看我的定投策略？」

内置 18 个高频场景剧本：想放弃、想梭哈、天天盯盘焦虑、纠结二选一、被人否定很委屈、坚持不下去、副业没起色很尴尬、眼红别人发财……也欢迎自由提问，它会从 20 张概念卡里选刀。

## 文件结构

```
caifu-mentor/
├── SKILL.md                 # 主入口：四段式校对流程与风格规则
└── references/
    ├── concepts.md          # 20 张概念卡片（定义／金句／常见误用／行动处方）
    ├── playbook.md          # 18 个高频场景诊断剧本
    └── chapters.md          # 50 章＋前言＋尾记速查表与引用纪律
```

## 来源与版权声明

- 本项目是 [《财富自由之路》](https://book.douban.com/subject/27011466/)（李笑来 著）一书的读者笔记与概念提炼，属于个人学习成果的非商业分享。
- 文中金句均为简短原文摘录并逐条注明章节，仅供学习与研究；原书完整版权归作者及出版方所有。
- **强烈建议购买原书，只字不差地阅读**——这也是书里第 25 章的原话：很多重要的观念会伪装成「和你没关系」的样子，使你生生错过且不自知。

## License

[MIT](./LICENSE)（适用于本项目的编排与原创文字；引用内容权利归原作者）

---

# caifu-mentor · Wealth Mentor (English)

> An AI skill that turns the 50 core concepts from Li Xiaolai's *The Road to Financial Freedom* (《财富自由之路》) into an on-demand life auditor: describe a thought, a decision, or a struggle — it delivers a verdict grounded in the book, plus a concrete action plan.

Plenty of self-improvement content tells you what's right and evaporates the moment you close the tab. This project does the opposite: **it turns one book into a persistent opponent that cross-examines your everyday decisions.**

It won't chat about life philosophies. Every audit runs the same four-part structure:

1. **Verdict** — one decisive sentence, stated upfront, no hedging
2. **What the book says** — verbatim quotes with chapter numbers (its source of credibility; nothing is paraphrased or invented)
3. **Your dissection** — your own words placed on the operating table: what counts as evidence, where the deviation is. Sharp, but never humiliating
4. **What to do** — at most three prescriptions, each with a concrete action, a frequency, and a pass/fail test. Vague advice like "be patient" is banned

## Example

**You say**: I've been running a side-project account for two months with almost no readers. Maybe I'm just not cut out for this?

**It answers**:

> **Verdict**: The thought "not cut out for this" is your biggest enemy right now — the book literally calls it the epitaph of all failures, and your two months haven't even reached the point where any conclusion is possible.
>
> **What the book says**: "'Maybe I'm just not suited for this' is the epitaph of all who fail — it might as well be rephrased as 'maybe I'm not suited for this world.'" (Ch. 4). "Growth only starts to truly matter after you break through the cost line; before that, it's all struggle..." (Ch. 1).
>
> **Your dissection**: You're treating "two months of low traffic" as proof of inadequacy — using present feedback to veto a long-term correct direction. The real questions are factual: how many pieces have you published? Did each one include a "get seen" action? Is your content what *you* think is essential, or what *readers* think is essential?
>
> **What to do**: Switch your KPI from view counts to publish count + iterations, and run 12 weeks before judging; do one "get seen" action per week; write down your prediction for 12 weeks out and check it when due.

## Install

Works with ZCode, Claude Code, Codex, and any agent that supports the SKILL.md convention:

```bash
git clone https://github.com/qishuai6/caifu-mentor.git ~/.agents/skills/caifu-mentor
```

Or manually copy this directory (SKILL.md + references/) into your skills folder (e.g. `~/.zcode/skills/`, `<project>/.agents/skills/`). Fully self-contained, zero external dependencies.

## Usage

Say to your agent:

- "Audit me: I'm thinking of quitting my job to do content full-time"
- "Check this against *The Road to Financial Freedom*"
- "What would Li Xiaolai say about my investment plan?"

18 built-in scenario playbooks cover the classics: wanting to quit, wanting to go all-in, doom-scrolling stock prices, agonizing over choices, feeling crushed by rejection, running out of steam, cringing at a stalled side project, envying someone else's windfall... Free-form questions work too — the skill picks the right scalpel from its 20 concept cards.

## File Structure

```
caifu-mentor/
├── SKILL.md                 # Entry point: the four-part audit workflow and style rules
└── references/
    ├── concepts.md          # 20 concept cards (definition / quotes / misuse / prescriptions)
    ├── playbook.md          # 18 high-frequency scenario playbooks
    └── chapters.md          # Quick-reference map of all 50 chapters + quoting discipline
```

## Attribution

- This project is a reader's study notes and concept distillation of *The Road to Financial Freedom* by Li Xiaolai, shared non-commercially for learning purposes.
- All quotes are brief verbatim excerpts, each attributed to its chapter. Full rights to the original text belong to the author and publisher.
- **Strongly recommended: buy the original book and read every word.** As Chapter 25 warns, important ideas love to disguise themselves as "irrelevant to you," so you miss them without ever knowing.

## License

[MIT](./LICENSE) (applies to the curation and original writing in this project; quoted material remains with its original author)
