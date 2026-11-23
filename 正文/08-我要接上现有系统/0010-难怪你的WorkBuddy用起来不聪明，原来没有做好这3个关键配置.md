---
title: "难怪你的WorkBuddy用起来不聪明，原来没有做好这3个关键配置"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/436"
type: "tool"
chars: 2649
sections: 6
figures: 0
chapter: "08-我要接上现有系统"
---

# 难怪你的WorkBuddy用起来不聪明，原来没有做好这3个关键配置
![YouCore 思维力 / 学习力 / 人脉力](https://mmbiz.qpic.cn/sz_mmbiz_gif/oyz7rkNWZxeibyJMLLOIogvLt9rS0UlciaefD059uVQAiaCkP7UOfv0icYdynunHXjo7d3EOcYmCqrceicmeV5eNEePdYXq8rnPITziaPXnD4PJgA/640?from=appmsg#imgIndex=0)

*YouCore 思维力 / 学习力 / 人脉力*

你满怀期待地打开 WorkBuddy，输入了第一个任务：“帮我整理一下这个季度的项目资料，写一份汇报。”。

WorkBuddy 翻了翻你的文件，给了一份泛泛的模板，跟你想要的东西差了十万八千里。你不甘心，又问：“我是做运营的，给我一些提升用户留存率的建议。”。它给你列了五条教科书级别的答案，看完跟没看一样。你生气了：“这东西不是说很聪明吗。怎么跟个实习生似的。”。

别急着骂 WorkBuddy，你有没有想过一个问题：它连你是谁、做什么的、用什么工具都不知道，你指望它能聪明到哪去。

![](https://mmbiz.qpic.cn/mmbiz_jpg/QoGkF8SH7EvPCOo3CeG5yQpBqaY1M0Oj2eaGzKXquGia4FibcTCicbp0cajIB0kPILicJQEXCwuMGeLzwnnrSknSHGbDPsmlgx3Okv36kcCU6sQ/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=1)

WorkBuddy 的本质是一个 Agent，Agent 的聪明程度由三样东西决定：它对你的了解、它掌握的专业技能、它能触达的外部工具。

这三个东西，在 WorkBuddy 里分别对应三个关键配置：MEMORY.md 记忆系统、Skills 技能包、MCP 连接器。

大部分人这三个配置一个都没做，就指望着 WorkBuddy 天生聪明。今天把这三点配好，同一个 WorkBuddy，你会发现它像换了一个人。

## 01 第一个配置：MEMORY.md，给 WorkBuddy 一张“身份证”。
第一个配置：MEMORY.md，给 WorkBuddy 一张“身份证”。WorkBuddy 的记忆系统是三层架构。第一层是云端记忆。

WorkBuddy 会从你的对话中自动提取你的工作背景、个人偏好、近期动态，每晚定时在服务器上更新用户画像。这部分是只读的，你不能直接改，但每次新对话它都会自动注入。

第二层是用户级 MEMORY.md。

文件位置在 ~/.workbuddy/MEMORY.md。这是跨所有项目生效的，用来记录你长期稳定的偏好和规则。

- 你是做什么工作的，负责什么业务
- 你偏好什么风格的输出（简洁/详细，要不要数据支撑）
- 你常用的工具和平台
- 你的专业领域和工作习惯

第三层是项目级 MEMORY.md。放在当前项目的 .workbuddy/memory/ 目录下。

这里面有两类文件：项目长期记忆 MEMORY.md（记录技术选型、架构约定、项目规则），以及每日工作日志 YYYY-MM-DD.md（append-only，自动追加每天做了什么）。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/QoGkF8SH7EvsfpOL1XkicEYOz5NiaeVFmkoWDUVZPl5T1PibApoLyMaZkyjwBz7qvExcfY9ZnWqz6mpZdT2T2YT6Rhib76T9VXTdjvkTM9vfpQk/640?from=appmsg&amp;watermark=1#imgIndex=2)

很多人连用户级 MEMORY.md 都没手动更新过，WorkBuddy 每次对话都得从零理解你。就像你每天上班都要重新做一遍自我介绍，你的同事不疯才怪。

## 02 第二个配置：Skills，给 WorkBuddy 装上“专业工具箱”。
第二个配置：Skills，给 WorkBuddy 装上“专业工具箱”。MEMORY.md 解决了“了解你”的问题，但还有一个“够不够专业”的问题。通用大模型虽然上知天文下知地理，但在垂直领域往往差点意思。

处理 Excel 数据透视表时可能犯低级错误，做 PPT 时可能排版混乱，操作 Obsidian 笔记时可能不理解双链语法。

这就是 Skills 要解决的问题。

Skill 是可复用的专业工作流，本质上是给 WorkBuddy 注入某个垂直领域的 SOP 和专业知识。

腾讯的 SkillHub 上已经收录了约 7.5 万个 Skills，覆盖了几乎 90% 以上的办公场景。

你不用自己去写复杂的提示词，去 SkillHub 搜索，一键安装就行。五套必备的 Skills：

![](https://mmbiz.qpic.cn/mmbiz_png/QoGkF8SH7EuBicyia8pbFRfSZHnXuStRs1CxNQ22bbibKwCpZa8napOFLf4brgkiaYzerAIhxia0gjWKU6icLmJBT9Q8s8bPbGT4wFnVU9icS3a6v4/640?from=appmsg&amp;watermark=1#imgIndex=3)

对比一下：没有 Skill 的 WorkBuddy 做 Excel 报表，可能用 Python 脚本硬算，结果格式一团糟。装了 xlsx 套件之后，它直接用 Excel 的公式和透视表功能，生成的报表和资深财务做得差不多。

Skills 还有一个很聪明的机制：自我沉淀。

如果你用 WorkBuddy 完成了一个复杂任务，它发现这个流程可以复用，会主动把它总结成一个新的 Skill。也就是说，你用得越多，WorkBuddy 的专业能力越厚。

Skills 不是加分项，是基础标配。

## 03 第三个配置：连接器，帮 WorkBuddy 打通“任督二脉”。
第三个配置：连接器，帮 WorkBuddy 打通“任督二脉”。

前面的 MEMORY.md 和 Skills 让 WorkBuddy 更懂你、更专业，但它们都是在 WorkBuddy 自己的地盘上使劲。

真正让你抓狂的，可能是那些搬运的体力活。

你需要让 WorkBuddy 整理资料，但资料存在腾讯文档里，你得先下载到本地，上传给 WorkBuddy，它处理好了再下载，然后再上传回腾讯文档。

来回折腾三次，还不如自己手动做了。连接器就是解决这件事的。

它的技术名叫 MCP，WorkBuddy 叫它“连接器”，本质上是 WorkBuddy 和外部应用之间的通信桥梁。

装了腾讯文档的连接器之后，你只需要说一句：“帮我把上周的会议纪要整理成摘要，存到腾讯文档”，WorkBuddy 自己读取、自己整理、自己写回腾讯文档。全程不用你动手。

WorkBuddy 内置的连接器覆盖了主流办公工具：

- QQ邮箱（自动收发邮件）
- 腾讯文档（直接读写在线文档）
- 腾讯会议（读取会议记录和转写）
- 企业微信、飞书、钉钉（打通即时通讯）
- IMA知识库、乐享知识库（接入企业知识库）
- GitHub（代码仓库操作）

除了这些内置的，腾讯云的 MCP Hub 上还有上千个 MCP 服务，足以覆盖你的主要工作场景。

配置也很简单，WorkBuddy 会把 MCP 配置写在 ~/.workbuddy/mcp.json 里。你只需要在连接器管理页面点“添加”，授权，就好了。

安装连接器之后，过去需要你手动“下载-编辑-上传”的搬运流程，变成了一句话的事。

小结。三个配置都讲完了，现在用 10 分钟把它搞定。

## 第一步（3 分钟）：创建 MEMORY.md。
打开 ~/.workbuddy/MEMORY.md，写下三件事：

- 我是谁（职位、负责的业务）
- 我的工作习惯（偏好简洁/详细、常用什么工具）
- 我当前的关注重点

保存后，下次新开对话，WorkBuddy 不再从零开始。

## 第二步（3 分钟）：安装核心 Skills。
打开 WorkBuddy 左侧的“技能”入口，搜索并安装：

- xlsx 套件
- docx 套件
- pptx 套件
- obsidian-skills（如果你用 Obsidian）

## 第三步（4 分钟）：安装连接器。
进入连接器管理页面，按你日常最常用的外部工具，安装 2-3 个连接器。推荐从腾讯文档和邮箱开始。配完之后，找一件之前 WorkBuddy 做得不好的事，重新让它做一遍。比如“按照我的工作风格，帮我起草一份本周的项目进展汇报”。你会第一次感觉到，它不是实习生了。

WorkBuddy 的聪明程度，不取决于模型本身，取决于你给它配了多少“上下文”。配得越多，它越聪明。
