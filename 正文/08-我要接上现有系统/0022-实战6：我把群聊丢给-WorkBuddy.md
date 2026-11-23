---
title: "实战6：我把群聊丢给 WorkBuddy"
source: "https://workbuddy.jiangyufan.com/index/hub/case/655"
type: "case"
chars: 2036
sections: 9
figures: 0
chapter: "08-我要接上现有系统"
---

# 实战6：我把群聊丢给 WorkBuddy
上一篇我们做了竞品调研，重点是让每个结论都能追溯来源。这一篇回到更日常的职场场景：群聊。

但如果只是让 AI 总结聊天记录，这件事很多工具都能做。更能体现 WorkBuddy 这类桌面龙虾工具优势的，是让它把群聊和本地项目资料放在一起对账。

## 01 群聊总结不等于项目进展。
群聊里有很多噪音：寒暄、确认收到、表情、重复催促。真正有用的是几类信息：任务、负责人、时间点、附件、风险、冲突。

如果只总结“大家讨论了上线进度”，价值不大；如果能整理成“产品明天给口径，运营周四交素材，客户评审时间存在冲突”，才真正能推进项目。

![普通 AI 总结群聊 vs 桌面 Agent 对账群聊｜差别不是总结得多顺，而是能不能和项目文件、纪要、表格互相核对。](https://mmbiz.qpic.cn/mmbiz_png/6UlmmlCwyI1dUk4aucs8f9ic95FcasHGfGL8FcibCkiccJSCbS7AmNMI7uQiaRHEu2r5y1q96cichYia5vQRrr6hyIEKu6ibpBQsuP7Yt5fqYWcJuU/640?wx_fmt=png&amp;watermark=1#imgIndex=0)

*普通 AI 总结群聊 vs 桌面 Agent 对账群聊｜差别不是总结得多顺，而是能不能和项目文件、纪要、表格互相核对。*

## 02 桌面 Agent 的优势：能和项目文件对账。
WorkBuddy 官方文档里提到，它可以选择工作目录、补充本地文件/图片/文字上下文，也能在右侧结果区查看生成的文档、表格等产物。Claw 远程控制还支持通过微信、企业微信、钉钉、飞书等渠道给电脑端 WorkBuddy 下发任务。

这些能力用在群聊整理上，就不是简单摘要，而是一个工作流：

- 读取群聊截图或导出的聊天文本。
- 对照会议纪要、进度表和项目文件夹。
- 找出已完成、进行中、延期、待确认和冲突信息。
- 生成项目进展清单、风险清单和群同步文案。

![这篇的目标:把群聊变成项目进展台账｜不是聊天摘要，而是进展、待办、风险、冲突信息。](https://mmbiz.qpic.cn/mmbiz_png/6UlmmlCwyI1Naia7xQka7N4XUZX2XScNNF3PoKp1IBkRCKqe1P0crp40wicMSgfpbibrenJkZCYian6icdXud5mOj4rlibFMXsSgwo5HW1wmczliag/640?wx_fmt=png&amp;watermark=1#imgIndex=1)

*这篇的目标:把群聊变成项目进展台账｜不是聊天摘要，而是进展、待办、风险、冲突信息。*

## 03 准备材料：别只扔聊天截图。
如果只给它一张截图，它能总结，但很难判断哪些话是真的更新、哪些只是重复。我建议准备这些材料：

- 群聊截图或导出文本：最好按日期整理。
- 上一次会议纪要：用于对照原计划。
- 项目进度表：用于核对状态和截止时间。
- 项目文件夹：看附件、方案、表格是否已经产出。
- 角色说明：谁是产品、运营、数据、客户、老板。

## 04 第一条指令这样写。
这条指令的重点是：不要只总结，要对账。

![第一条指令:不要只总结，要对账｜把群聊和项目资料放在一起看，才能体现桌面Agent的价值。](https://mmbiz.qpic.cn/mmbiz_png/6UlmmlCwyI3zfPtFdJwEKICS1COfdMleky1MYZHiaT1ibyic0qepENicQ5Nt1Rq4wwXtX4iaqZPU8ia4IhoOQicm5Hep9Odic6Kaf9qib4XUVxhUl5BE/640?wx_fmt=png&amp;watermark=1#imgIndex=2)

*第一条指令:不要只总结，要对账｜把群聊和项目资料放在一起看，才能体现桌面Agent的价值。*

请读取当前项目目录里的群聊记录/截图、会议纪要、项目进度表和相关文件。先不要直接写总结，请按顺序完成： 1. 从群聊里提取所有任务、承诺、时间点、负责人、附件信息； 2. 对照会议纪要和项目进度表，判断哪些已完成、进行中、延期、待确认； 3. 如果群聊和纪要/表格信息冲突，请单独列出； 4. 生成一份项目进展清单 xlsx； 5. 生成一份风险与待确认问题 md； 6. 生成一段适合发回项目群的 200 字以内同步文案。要求： - 不要凭空补负责人和截止时间；缺失就写“待确认”； - 每个结论都标注来源：群聊第几条、哪个截图、哪个文件； - 涉及发群前，先输出文案让我确认，不要直接发送。

## 05 好结果应该长什么样。
我判断结果好不好，不看它写得多顺，而看它有没有把项目状态拆清楚。

![](https://mmbiz.qpic.cn/mmbiz_png/6UlmmlCwyI2icXzGJJNZib6wIzVoDlCa3tC3Nlef1NmQ5ibw7xulkCtgBu6icicpbiakYBfDcYdoFmj8UL5NjvUo8LB4zego9icCuDLWCibLVbatG18/640?wx_fmt=png&amp;watermark=1#imgIndex=3)

尤其要看“冲突”和“待确认”。比如会议纪要写的是周四评审，群聊里客户又说周五前确认，这种就不能合并成一个确定时间，必须单独列出来。

## 06 最后交付物：别只要聊天摘要。
更好的做法，是让 WorkBuddy 输出一组项目文件。

![最后交付物:别只要聊天摘要｜让它生成一组项目文件，后面才方便追踪和复盘。](https://mmbiz.qpic.cn/mmbiz_png/6UlmmlCwyI1CZwO429DjPaXbFrNk0XjDQ4fXxX8aC4aaNpIc6cLSVm72ibtdP8FyaTYbUeWHncUNe0Qp9ZJbJLBjphPvCF3xxZgGPAhE534s/640?wx_fmt=png&amp;watermark=1#imgIndex=4)

*最后交付物:别只要聊天摘要｜让它生成一组项目文件，后面才方便追踪和复盘。*

这样你既能给项目群同步，也能留一份项目过程记录。下次老板问“上周谁说过这个”，你至少知道该去哪个截图或文件里找。

如果你已经配置了 Claw，就可以在手机上的微信、企业微信、飞书等平台给电脑端 WorkBuddy 下发任务。

这就很适合临时场景：会议刚结束、路上看到群聊炸了、老板突然问项目进度，你可以让 WorkBuddy 先在电脑端整理资料，回来直接看结果。

![更像桌面龙虾类的地方:可以从群里远程触发｜通过Claw，手机上的即时通讯软件可以给电脑上的WorkBuddy下发任务。](https://mmbiz.qpic.cn/mmbiz_png/6UlmmlCwyI2la9yvROBSFnEwvpX0IbWjWsGnuicC3FRs7Zpvl69VFYItsf49Oyoq4G6sRK4ibgsvwd9DtIzB6PYlcdPjbPibkWiapDR6jE6xQM0/640?wx_fmt=png&amp;watermark=1#imgIndex=5)

*更像桌面龙虾类的地方:可以从群里远程触发｜通过Claw，手机上的即时通讯软件可以给电脑上的WorkBuddy下发任务。*

请根据今天项目群的聊天记录和当前项目目录，整理一份项目进展清单： 1. 已完成事项； 2. 进行中事项； 3. 延期或风险； 4. 待确认问题； 5. 适合发回项目群的简短同步文案。先不要直接发群，把文案给我确认。

## 08 怎么验收。
群聊整理最容易出错的地方，是把“有人说过”当成“事情已确定”。我会按这几个问题验收：

- 有没有把玩笑、猜测、临时讨论写成正式结论？
- 有没有把群聊和会议纪要里的冲突单独列出？
- 有没有标注来源截图或聊天条目？
- 有没有明确下一步动作，而不是只写“继续跟进”？
- 发群文案是否会误 @ 人、误传未确认信息？

## 09 这类任务适合什么场景。
- 项目群消息太多，需要快速同步进展。
- 老板临时问“现在推进到哪了”。
- 客户群里出现新需求，需要整理成待办。
- 多个群里信息分散，需要合成一个项目台账。
- 项目复盘时，需要回看过程中的关键承诺。

这篇的关键不是 WorkBuddy 会不会总结聊天，而是它能不能把聊天记录和本地项目资料串起来，变成能推进项目的进展清单。

## 10 下一篇。
下一篇我会继续测试 PPT 大纲场景。

重点不是让 AI 直接生成一份花哨 PPT，而是看 WorkBuddy 能不能读取项目资料、提炼汇报对象关心的问题，先搭出一份能讲清楚业务的 PPT 大纲。
