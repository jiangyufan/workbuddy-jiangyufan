---
title: "手把手教程：用 WorkBuddy 把一份政策文件\"蒸馏\"成 16 个可复用技能"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/744"
type: "skill"
chars: 3186
sections: 9
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 手把手教程：用 WorkBuddy 把一份政策文件"蒸馏"成 16 个可复用技能
好的分类不是按"文件有几章"来的，而是按"用户会问哪类问题"来的。

## 04 第二步：让技能自我进化（Darwin）。
技能"写出来"不代表"够好用"。这时候上达尔文，一行命令启动进化：进化命令：darwin evolve books/yanfafei-jiaji-2.0/。（books/yanfafei-jiaji-2.0/ 就是你上一步蒸馏出来的技能保存目录）。

达尔文会做三件事：先用 8 维评分卡给每个技能打分 → 找出最弱的那一环 → 只做一处低风险改进，改完重测，分涨了就保留、跌了就回滚（永远留退路）。

![](https://mmbiz.qpic.cn/mmbiz_png/xME3pneqdMDxcPNiaVDgTQR8dGPOEWrXTeh0wjibYxic6YVUg8D9EulQRkqfJJ8cyNOdVvGxBRB3ibrSciaiaJ2lUrB50dKTsdgNWulEicBAoa12c8/640?wx_fmt=png&amp;watermark=1#imgIndex=5)

本案例跑完的结果：指标。进化前。进化后。平均分。88.9。91.9。回滚数。（16/16 全保留）。优化的艺术在于：每次只动最弱那一环，而且永远留退路。

## 07 照着做一遍，你能得到什么。
回顾一下完整四步：

1. 装两个技能：book2skill（造）+ darwin（磨）
2. 一键蒸馏：一句话把文件变成一组技能
3. 进化打磨：一行命令把平均分从 86 磨到 91.9
4. 升级用户级：复制一下，全项目永久可用

这套方法不挑文件。高新企业认定指南、各省市科技项目申报指引、行业合规手册、公司内部 SOP……只要是有明确规则、需要"按场景查询"的知识，都能这么处理。

它替代不了专家，但能把专家的经验固化下来，让每一次咨询都站在同一个高质量起点上。工具只是拐杖，走路的人是你。但一副好的拐杖，确实能让路走得更稳、更快。

![①研发活动认定｜rnd-activity-judgment研发活动判定](https://mmbiz.qpic.cn/mmbiz_png/xME3pneqdMC3bcf3qbKfpbJ9dFfdUuUoQrVicfbksTh4qNha6DHlOf5vvKR52eSuyiakCVUu4ExSZjbRrX2tnkibC5L730h1hwL5n4kA8rIoB4/640?wx_fmt=png&amp;watermark=1#imgIndex=4)

*①研发活动认定｜rnd-activity-judgment研发活动判定*

## 05 第三步：实测——技能真的能用吗。
纸上谈兵没用，我拿 3 个真实的集团研发问题直接问技能：

![](https://mmbiz.qpic.cn/mmbiz_png/xME3pneqdMCzFpVOPOrEpkmQ6MQ3bOp1ZicAy2xCHAZwkT3cLXnEpp7qgySqffudktbSoLnE4HGv58HrFTibchc9Momjwb2OPt6rm3DFCnGY4/640?wx_fmt=png&amp;watermark=1#imgIndex=6)

Q：集团统一研发、各子公司怎么分摊加计扣除。

检验一个技能是否合格的唯一标准：拿真问题问它，看它能不能答对。

## 02 准备工作：在 WorkBuddy 里装好两个技能。
平台就用 WorkBuddy（其他支持安装 Skill 的 Agent 平台流程一样）。我们需要两个开源技能，分工很清晰：

- book2skill（仓颉 Skill） —— 负责"从零造出来"：把一本书 / 一份文档，蒸馏成一组可执行的 AI 技能。
- darwin-skill（达尔文 2.0） —— 负责"打磨到能用"：给每个技能打分、找薄弱点、自动优化、你确认，循环爬坡。

安装命令（直接在对话里让 Agent 帮你装，或按仓库地址安装）：安装 skill：kangarooking/cangjie-skill（book2skill）。

安装 skill：darwin-skill（达尔文 Skill 2.0 · GitHub: alchaincyf/darwin-skill）。

装好之后，你只要会"说人话下令"就行，两个技能的内部逻辑不用管。

![欢迎回来,｜准备好开工了!](https://mmbiz.qpic.cn/sz_mmbiz_png/xME3pneqdMCWxHqUQr58pyhajRZ0kibgj2MngFXEIsDhticKNHb1c7zt00R5ZJqOaT439N94xkfjGN7sHsTolycibFLsS7ic7VjhrjAmroFoDYI/640?wx_fmt=png&amp;watermark=1#imgIndex=1)

*欢迎回来,｜准备好开工了!*

工具不稀缺，稀缺的是知道"哪两个工具串起来，能解决我手头的问题"。

- 研发活动认定（3 个）

Skill。干嘛用的。rnd-activity-judgment。用"三要点"正向判定某项目/活动是否属于研发活动、能否享受加计扣除。excluded-activities。用 7 类不适用活动清单负向排除看似研发实为非研发的活动。negative-list-industry。

判企业是否落入行业负面清单/核定征收，过享受资格 gate。

- 费用归集（7 个）

deductible-expense-caliber。按 6 类正列举口径归集可加计研发费用，明确"正列举未列举不得加计"。other-expense-limit。用统一限额法计算"其他相关费用"10% 上限及资本化项目分摊。capitalize-vs-expense。

判定研发支出应费用化还是资本化（开发阶段 5 条件）。entrusted-rd-processing。委托研发境内外 80%/2/3 基数、合同登记、关联方明细处理。cooperative-rd。合作研发（多方共同投入），各合作方就自身承担费用分别加计、合同登记、知识产权归属约定优先。

group-centralized-rd。集团集中研发按"权利义务一致、收益配比"原则在成员企业间分摊、关联申报。special-income-offset。特殊收入/研发形成产品销售材料费/政府补助的基数冲减处理。

- 核算与申报（4 个）

aux-account-setup。按项目设研发支出辅助账，选样式、费用化与资本化分设。filing-timing。7 月 / 10 月预缴或汇缴。申报时点选择，无需事前鉴定/备案。retention-records。留存备查资料清单、10 年保存期限与企业担责。

retroactive-enjoyment。符合条件未享可追溯最长 3 年、税企异议鉴定、亏损/失败可享。

- 优惠组合（2 个）

accelerated-depreciation。专门研发设备可加速折旧并与加计叠加，基数按税收折旧额（2017 年 40 号口径）。

更妙的是，这些技能还会自动互相关联成知识网——你调一个，系统知道它可能还要联动哪几个。

## 06 第四步：从"项目级"升级到"用户级"。
到这儿，技能还躺在 books/yanfafei-jiaji-2.0/ 这个项目目录里——只有当前这个项目能调用。想让它变成你所有对话、所有项目都能用的"常驻专家"，最后一步是升级到用户级：

把技能目录复制到用户级技能文件夹即可：命令：把 16 个 skill 装进 ~/.workbuddy/skills/ 当可调用技能。

## 或在终端输入命令，从项目目录，复制到用户级（所有项目/对话都能调用）。

![升级:项目级→用户级，全项目可用](https://mmbiz.qpic.cn/mmbiz_png/xME3pneqdMC6BjlMsTSKJZvyq0m1tI4elJ5Eu5WLjicPDRujUJYajQzAnRhL1QUj9J2jFpmqsjt4t4H5ribsj6Uf9rxpNK83yaHuibezia86DuM/640?wx_fmt=png&amp;watermark=1#imgIndex=7)

*升级:项目级→用户级，全项目可用*

成后，这 16 个技能就常驻在 ~/.workbuddy/skills/ 下，以后任何对话直接喊名字就能用。

⚠️ 一个小提醒：复制过去的是"静态副本"，蒸馏稿 books/yanfafei-jiaji-2.0/ 仍是权威源。以后要改技能，记得两处同步（或用软链接），避免两边漂移。

让成果从"这次能用"变成"永远能用"，才是真的闭环。

## 手把手教程：用 WorkBuddy 把一份政策文件"蒸馏"成 16 个可复用技能。
导读：下次再拿到一份几十页、看两页就犯困的政策文件，你其实不用自己啃。这篇就带你用 WorkBuddy（任一支持安装 Skill 的 Agent 平台同理），把一份 2.4 万字的《研发费用加计扣除政策执行指引（2.0版）》，一步步变成 16 个"随时能问、张口就答"的 AI 技能——而且还能自我进化、跨项目复用。全程命令我都给全了，照抄就能跑。

![一本书到16个AI助手](https://mmbiz.qpic.cn/mmbiz_png/xME3pneqdMDtiaKokEfc2e4sYTvlXqxJ9uCtrCtxYQI3wNxXNVtianRSEQE3micvyzUSAnLJACXZrZkbSUDibBT3ic5wVpEu19frYCJ2hSYPSkxI/640?wx_fmt=png&amp;watermark=1#imgIndex=0)

*一本书到16个AI助手*

## 01 为什么值得你花 10 分钟学这个。
说个扎心的事实：这类政策文件有个通病——信息密度极高，但它是按"从头读到尾"设计的，不是按"遇到问题随手查"设计的。

比如研发费加计扣除 2.0 版，里面覆盖了：什么算研发、什么不算、哪些费用能加计、委托/合作/集团研发怎么处理、申报时点、留存备查、追溯享受……你让财务或项目主管通读，大概率第 10 页就晕了；真遇到具体问题，还得回去翻对应章节。

解法一句话：把文件"拆"成一组小而精的模块，每个模块只负责回答一类问题，AI 直接拿来用。

这次我拿一份真实文件跑通了全流程，最终得到 16 个原子技能，平均分从 86 磨到 91.9，3 个真问题实测全答对。下面就是完整步骤。

把大文件拆成小模块不难，难的是每个模块都能独立工作、边界清晰、经得起实测。

## 03 第一步：一键把政策文件蒸馏成技能。
这是最爽的一步——你不用拆解、不用归纳，直接下指令：蒸馏命令：

帮我把这个文件《科技部、税务总局联合发布《研发费加计扣除2.0版》（研发费核查标准）.docx》（这里需要添加文件地址，或添加文件到对话）用 @skill:book2skill 蒸馏成方法论。

把文件路径换成你自己的就行。剩下的，book2skill 会自动跑一套叫 RIA-TV++ 的五步流水线（整书理解 → 多路提取 → 三重验证 → 并行构造 → 卡片互链），你不用介入：

![](https://mmbiz.qpic.cn/mmbiz_png/xME3pneqdMBu5KADapKaNP7h10Vd72iabXw720725I7wuc8ezvo6xknymnnCyVHbnvibwSTB7atGnNG8vSddiaWrj4hqT1fBFLWHcAmFVic9rEI/640?wx_fmt=png&amp;watermark=1#imgIndex=2)
