# skill-forge

把你脑子里的方法论，锻造成一台别人装上就能用的 Skill 机器。

90% 的人想"做个 skill"都卡在两件事：①不知道哪些经验值得封装，写出来全是正确的废话；②写出来的 SKILL.md agent 根本不触发。skill-forge 把这两件事变成一条可检查的产线：立项拷问 → 挖矿 → 定名 → 锻造 → 反模式拦截 → 触发自检 → 发布包。

## 背景

2026 年 10 月，GitHub trending 前 8 有 5 个是 Agent Skills 项目，Google 宣布 11 月起 Gemini 的 "Gems" 全面更名为 "Skills"、接入 SKILL 开放标准。Skill 正在成为 AI 时代的"个人配置文件"（the new dotfiles）——而大多数人还不知道怎么把自己那份写出来。

## 安装

把这句话发给任何支持 SKILL 标准的 agent（Claude Code / Codex / Cursor / Gemini CLI / WorkBuddy）：

```
请帮我安装这个 Skill：https://github.com/Halloran444/skill-forge
```

或手动：

```bash
git clone https://github.com/Halloran444/skill-forge ~/.claude/skills/skill-forge
```

## Quick Start

对 agent 说：

> 用 skill-forge 帮我把"我每周写周报的流程"做成一个可发布的 skill

它会先拷问三个问题（谁的痛 / 差在哪 / 凭什么信），答不上来会直接拦下你——这是特性，不是 bug。

## 工作流

```
立项拷问 → 挖矿(口述/文件/笔记) → 定名(查重) → 写 SKILL.md
   ↓ 拦截：三问答不上来                        ↓
← 退回重谈                            反模式拦截(4 条自查)
                                              ↓
归档 v0.1.0 ← 组装发布包(README/LICENSE/CHANGELOG) ← 触发自检(3+3 对照)
```

## 设计立场

- **一个 skill 解决一个痛**，塞了三个能力的就是三个 skill
- **description 是触发器**：写不清"什么时候用"，skill 就等于不存在
- **没有实战背书不开工**：作者自己没用过的流程，锻不成机器
- 发布是对外动作，永远等用户确认

## Roadmap

- v0.2：references/ 模板库（周报/复盘/选题三类骨架）
- v0.3：脚本化自检（触发词测试自动化）

## License

MIT
