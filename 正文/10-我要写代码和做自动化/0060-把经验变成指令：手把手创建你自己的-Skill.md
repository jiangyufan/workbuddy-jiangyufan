---
title: "把经验变成指令：手把手创建你自己的 Skill"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/1113"
type: "tool"
chars: 869
sections: 5
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 把经验变成指令：手把手创建你自己的 Skill
## Skill 的本质是什么
无论你用 Claw、Claude Code 还是 Codex，都可以通过类似 Skill 的方式来封装重复性任务。Skill 的本质是：把「如何做某件事」的经验，封装成可复用的结构化指令。这个核心知识是通用的——学会之后，可以迁移到任何支持自定义指令的工具里。

## Skill 的核心价值
Skill 火起来之后，无论蒸馏还是自创，它的价值都在于把行业知识、业务逻辑与 AI 能力深度融合，实现「任务拆解—自主执行—结果闭环—自我进化」的全流程提效。常见用法包括：写公众号按固定格式生成内容；格式转换（转 Markdown / PDF）；质量检查（检查项目信息一致性、准确性）；数据处理（按规则整理数据）；对接 API（让 Agent 通过 API 成功调用工具）。

## Skill 文件放在哪里
以 Claude Code 为例，Skill 文件有两个存放位置。方式一：项目级 Skill（推荐），放在当前项目目录下，只对当前项目生效——项目目录/.claude/skills/你的skill.md。方式二：用户级 Skill（全局），放在用户配置目录，对所有项目生效——Windows 在 %USERPROFILE%/.claude/skills。对于 Codex，路径是 .codex/skills；对于 openclaw，用 .openclaw/skills。

## 实战：用 Skill-creator 创建 Skill（蒸馏你的写作风格）
最高效的方式不是从零手写 Skill，而是让 AI 帮你分析和封装。例如要自动提炼你的公众号写作风格并生成专属写作 Skill：第一步，用 Skill-creator 创建 Skill。虽然可以直接和 AI 自然语言对话创建，但更推荐借助专门的创建器来自动拆解你的范例、提取风格参数，生成结构化的 Skill 文件。

## 把 Skill 用起来
装好之后，直接以自然语言召唤即可——告诉 AI 你要达成的目标，它按 Skill 里封装的流程执行。重点是：Skill 把「你会但每次都要重复说一遍的做法」固化成了规则，装上它，即使换了人或过段时间，结果依然稳定。
