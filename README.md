# shi-fu（师傅）

一个给小白用的工程引导层。基于 [Matt Pocock 的 Skills](https://github.com/mattpocock/skills) 设计。

## 这是什么

Matt Pocock 开源了一套专业的工程 skills（/grill-me、/tdd、/diagnose 等），但它们假设用户已经知道什么是 PRD、什么是 TDD、什么时候该调试。

shi-fu 是这套工具的**翻译层和路由层**——它先问几个问题，判断你处于哪个工程阶段，再推荐合适的 skill 给你，并用你能听懂的话解释为什么。

## 适用人群

- 想学工程但不知道从哪开始的人
- 有想法但不知道该用什么工具的人
- 被工程术语拦在门外的人

## 工作原理

```
你 → shi-fu（问问题 + 判断阶段 + 推荐skill）→ Matt Pocock Skill（执行）
```

shifu 不写代码，它只是一个**领路人**。

## 快速开始

### 第一步：安装 Matt Pocock Skills

```bash
npx skills@latest add mattpocock/skills
```

### 第二步：安装 shi-fu

复制 `SKILL.md` 到你的 skills 目录：

```bash
cp SKILL.md ~/.claude/skills/shi-fu/SKILL.md
```

### 第三步：使用

在 Claude Code 里直接打：

```
/shi-fu
```

然后回答问题，它会引导你走完整个工程流程。

## 工程阶段映射

| 你在哪个阶段 | 推荐 skill | 为什么 |
|---|---|---|
| 有模糊的想法，不确定要什么 | `/grill-me` | 先想清楚再动手 |
| 有清晰想法，还没开始 | `/grill-me` | 确保你想对了 |
| 在改现有代码 | `/grill-with-docs` | 建立共同语言 |
| 需要规划并拆解任务 | `/to-prd` + `/to-issues` | 先写计划，再拆任务 |
| 正在构建中 | `/zoom-out` | 从森林看树木 |
| 有东西坏了 | `/diagnose` | 系统化调试 |
| 想做得更好 | `/improve-codebase-architecture` | 整理你的代码 |
| 想写测试 | `/tdd` | 测试先行 |

## 相关项目

- [Matt Pocock Skills](https://github.com/mattpocock/skills) — 工程技能本体
- [mattpocock/skills](https://github.com/mattpocock/skills) — 课程
