---
title: "别养龙虾了：腾讯WorkBuddy可能是最适合大众的本地AI助手"
source: "https://workbuddy.jiangyufan.com/index/hub/case/667"
type: "case"
chars: 2857
sections: 10
figures: 0
chapter: "12-我看别人怎么用"
---

# 别养龙虾了：腾讯WorkBuddy可能是最适合大众的本地AI助手
## 本文为 WorkBuddy 入门指南。
从 3 月份龙虾热浪到现在，很多人都对个人 AI 助理或者AI agent有了新的认知。但养龙虾又贵又难，OpenClaw 要自己部署配置，Claude Code 门槛对很多人来说也非常高。如果你想体验但不想折腾，还想在2026年真正上到AI Agent的快车，腾讯的 WorkBuddy 或许是个不错的选择。

![腾讯版AI AI办公助手｜Claw 快捷接入指南](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkafyUzXhaPF0qYFyomZH4TCsXiaRwNqD4BgaIREe4MjHzsdaxC7UUM1gJuWY5MF89icibJeOvw4UItfqiacw3FxKBuWdQWTt6cy1b4A/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*腾讯版AI AI办公助手｜Claw 快捷接入指南*

## 为什么推荐 WorkBuddy。
大厂产品，省心安全。

腾讯云出品，通过了国家网络安全审查备案，下载即用。我觉得普通人别图新鲜去折腾开源项目，大厂封装好的产品更省心。这也是我们一贯的推荐原则，安全可靠稳定是最重要的。

## 内置模型够用，成本低。
WorkBuddy 内置 Kimi 2.5、GLM 5、ds 等主流模型，很多人养龙虾跑的也是这几个。反正我用了一个月，赠送的积分到现在还没消耗。如果有特殊需求，也支持自定义接入其他模型。

![输入消息...｜+配置自定义模型](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkaeUWic3YlcJuMRLBZg6cvex0ibfzCMIEKHo3d1MD9UdOsvvZ05Of9GU2S8yJQeSGNGPkJ7jicwMXu6yOpNLKzHkSAico35UopaOowo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*输入消息...｜+配置自定义模型*

## 安全机制完善。
OpenClaw 权限极高且无标准拦截，新手易踩坑。WorkBuddy 在安全上做得更完善：授权机制可以只开放指定文件夹，执行前会展示计划，高危操作会被拦截，数据全程本地处理不上云。

需要注意的是，任务记录默认存在 C 盘（Win 用户），建议做好工作空间管理（下文会讲）。

## 它能干什么。
一句话说需求，WorkBuddy 就能在你电脑上直接执行完交付结果。文件批量处理、多格式文档生成（Word/Excel/PPT）、数据分析报告、海报设计、本地知识库、定时任务自动化，这些都能做，还支持多 Agent 并行协作，做得都还挺好。

1. 下载安装

![展开更多(7)｜我正在写一个workbuddy的... 32分钟前](https://mmbiz.qpic.cn/mmbiz_png/bJGC6SphkafXicS9aF1ejJnicB3utDXarWAEriacxj1D05RmkfIjU7UNNmaAuo8PmpGxLRtL48aENJg4K3xQhS5LmEHgFyA77A0cqCMV3Kxy8I/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*展开更多(7)｜我正在写一个workbuddy的... 32分钟前*

1. Claw 配置（微信接入）

这是 WorkBuddy 最“龙虾”的配置，可以在手机微信里远程指挥电脑上的 AI 干活。

![注册微信客服号以接收和回复消息。｜注册微信客服号以接收和回复消息。](https://mmbiz.qpic.cn/mmbiz_png/bJGC6SphkafUoSHNcZMegJ3h4RDOx5eYDQT3ibLc8mibUNO86MbMZcuwTNIolr4RJIVwZQtIn6vbUqNxXZjwGibvuia48AZBvPviaXibjJOT8vhDU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*注册微信客服号以接收和回复消息。｜注册微信客服号以接收和回复消息。*

![WorkBuddy为你服务｜帮我看看桌面有一个2月发票文件夹，帮我整理文件夹里的发票，在桌面生成excel](https://mmbiz.qpic.cn/mmbiz_jpg/bJGC6SphkadP8NfibBbuavicpaCsicV1DqbAPDN1E2e8dRK7TSib6o89lRno0mqaQP9TiatojnaZn8icib6tNYPp2GClibiaWN9RUH3qeU8z9nKxsgJc/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*WorkBuddy为你服务｜帮我看看桌面有一个2月发票文件夹，帮我整理文件夹里的发票，在桌面生成excel*

你通过claw配置的输入端（比如微信）产生的任务将会形成一个独立的【claw】的工作空间。

Claw 有几个限制：工作目录固定、只有一个页面、无法清空上下文。所以更适合轻量级临时任务，比如出门在外让电脑帮你查个东西、整理个文件。

重要的项目型工作，我们还是比较建议在电脑端新建专门对话，可以自由选择工作目录，以便保持独立上下文。

1. 工作空间设置

每次新建对话时，WorkBuddy 会让你设置工作目录。建议按项目单独设定，不要开放整个硬盘。从桌面、文档等常用目录开始授权，敏感文件夹谨慎授权。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkafpKxuFSfEOE8gxRQv6UEq9cvqxAvoo8xPwvO1EvaKqTOgBZh03UYAJZFrhRdSJwPb227tbqIn9KDSzicfIEnHEEdRvEBhBcVmU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

## 上下文管理。
对话太长时，早期内容会被截断，AI 会“忘事”。我的建议是不同任务开不同对话，别在一个窗口里干所有事（claw任务除外）。如果 AI 开始答非所问，新开对话重新说需求。修改重要文档前记得让它先备份。反正和以前你用deepseek的逻辑一样，新主题新建任务。

针对claw的上下文，你可以看看设置里的会话管理，你在 WorkBuddy 里和 AI 的每一次对话，都会受这个设置控制。超过一定时间没用claw互动，它就会自动开新会话、清掉旧上下文。

![自动新起会话｜超过设定时间未对话，自动开启新对话](https://mmbiz.qpic.cn/mmbiz_png/bJGC6SphkacaejsKBrPbze2kywfVpRQQ3VUezgbw5tA309FLzTXLzUeme3JZd4yxIpTicApqibGwPPt0SBKLic8SIw5HnibMGftT2wFb8GOgfVo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*自动新起会话｜超过设定时间未对话，自动开启新对话*

1. 两种工作模式

WorkBuddy 有两种核心工作模式，根据你的需求选择：

## 日常办公模式。
面向所有人的通用办公场景。生成报告、分析数据、制作 PPT、批量处理文件、深度调研——这些全在这个模式下，是大多数人用得最多的模式。

## 代码开发模式。
面向开发者。代码审查、Bug 修复、项目理解、网站开发，功能上类似于命令行版的 CodeBuddy。如果你想尝试 vibe coding，也可以从这里开始。

## 执行策略（Craft / Plan / Ask）。
除了工作模式，WorkBuddy 还有三种执行策略可以切换。Craft 模式直接执行，效率最高，适合明确的任务。Plan 模式先列出执行计划，你确认后再动手，适合复杂任务。Ask 模式只问不动手，纯对话模式，适合咨询场景。

另外关于【召唤专家】在此不多加赘述，你可以根据任务来选择，复杂的任务可以先召唤一个对应的问问怎么搞，它有对应专业知识数据和回复设置来做回答支撑。但我觉得有时会比较模板化。

![按行业分类浏览专家，召唤他们为你服务｜▶ 搜索专家职称或描述...](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkaeSCLr3K2RNhJcicNROXiaiakibnUCgS0N8ficlX4cqFR37kWxKIo4secklTJb1rzH9NWKNBBic0lYG3WwHsuSYnIQWThUDawgw01r2o/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*按行业分类浏览专家，召唤他们为你服务｜▶ 搜索专家职称或描述...*

1. 模型选择

WorkBuddy 内置了 Kimi 2.5、GLM 5等主流模型，对话界面可以直接切换，日常使用完全够用。Auto应该是混元系列。如果有特殊需求，也支持自定义接入其他模型，具体配置方法可查阅官方文档。

1. Skill 技能

Skill 是 WorkBuddy 的能力扩展包，能让 AI 干原本干不了的事，很多人“养不好龙虾”也是卡在了没有合适的skills这一步。

我使用下来觉得大多数日常任务开箱即用，遇到“做不到”的情况，先看看有没有对应的 skill。然后可以在官方配置skillhub里去找，也可以自己描述需求用find skills帮你找找。

![+添加技能](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkaeCo6NX2f6gekiazCQBOTT3TtHoC1ZwsHZpQ06XQUPBCvXxQomfOxWAT4DATiar1TbRdHnmfLbb0xe45QzDhhhczoOeEAhMaGbnw/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

*+添加技能*

你也可以把重复性工作流程沉淀为自己的 skill，实现一键复用。至于怎么做skill，网上已经有很多教程，这个对用好AI非常重要，后边有空还是会单开一篇。

1. 记忆与人格定制

WorkBuddy 有比较完善灵活的记忆系统和定制化配置，会自动记录你的工作习惯、说话风格偏好、常用工具等，也可以自己触发它自己的人格修正。比如你总是让它用简洁的口语回答，用几次之后它就会记住。（初始看看设置里的记忆选项开启没有）。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkafchAulhaIpgvpdY1RUKTbc5WuathEmiamTX5vK98GsJcRBBKwtiaYvxn1XcINZVvSwXMiaiaJNFdIQISHhaaobvH1ehvGFtxojick0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=10)

![](https://mmbiz.qpic.cn/sz_mmbiz_png/bJGC6SphkacviaqcgP8fBHDbcd1nZRKZzsEZzrWfXG15Pb26HIEgYR7USLKXHJibTDhMOQxUsOnEc9hAM99HYzUqsN7mm70xkkk408wOSAyBo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=11)

WorkBuddy 通过 ~/.workbuddy/[SOUL.md] 记录回应风格，通过 ~/.workbuddy/memory/[MEMORY.md] 记录你的背景偏好。你可以直接告诉它需求，或手动编辑这些文件，修改后即时生效。

装好 WorkBuddy，绑定微信，选个工作目录，然后直接开始对话就行。

当然它也不是万能的。上下文太长会截断，多步复杂任务偶尔会绕弯子，Claw 那边还有几个小限制我前文也写了。但整体用下来，这些都在可以接受的范围内。

真正有意思的是用久了之后，它开始记住你那些乱七八糟的偏好，你说话中英文夹杂，它也跟着混着说；你们讨厌的那种"这不是...而是..."的句式，说几次它也很少用了。这种感觉怎么说呢，真的像有个好buddy了。

推荐试试，反正还不要钱。

![](https://mmbiz.qpic.cn/mmbiz_png/bJGC6SphkafaOCHRnRf4JmibEdTm7IxXuQWgBkibGxESPwaR8tJo1X1t6FAUacxGmfJ9YvGOzTH6saaRgbxKpNicUZqiaccxEmoJZXmarHWhFibY/640?wx_fmt=png&amp;watermark=1#imgIndex=12)

牧云之野（MUY AI Solutions）成立于2024年11月，由来自国内外顶尖学府的人工智能行业专家组建，核心成员包括前上市国企总工程师、计算机科学博士等。作为国内AI应用先锋机构，专注为政企提供定制化AI 应用指导、全链路数智解决方案、以及AIGC创作服务。依托国内顶尖研究院技术资源支持，紧跟政策和行业趋势，服务众多政企单位与院校，已为数十家大中型政企及 7000 + 员工提供优质服务获赞誉。团队坚持技术实用主义和长期价值创作，秉持科技向善初心，深度赋能客户发展，扎根行业挖掘更多AI应用价值。

## 让AI为我所用。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/bJGC6SphkadbIM60ncERU7TkCFcibcATyE5bpZeS26hemHxEh6l84LFYq1Qa0yXqHTvGSUsbkZ5dC8lQdQggYG1icxHJQ0t8aia0DYgItibbU0Q/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=13)
