---
title: "【巽哥说】用ima知识库“蒸馏”出一个项目式学习教学设计的skill"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/350"
type: "skill"
chars: 1201
sections: 6
figures: 0
chapter: "04-我要管知识库"
---

# 【巽哥说】用ima知识库“蒸馏”出一个项目式学习教学设计的skill
![广东省郑巽名教师工作室(初中综合实践活动)](https://mmbiz.qpic.cn/mmbiz_png/VKoHDXNKAvEQmNFKPsZUHnicKlfxuYKXj4Gb3x6qMRBiatjuDMorsJJib0HngDsnZZow1QbayzaOXavs9gh1icA3Mw/640?wx_fmt=png#imgIndex=0)

*广东省郑巽名教师工作室(初中综合实践活动)*

## 00 蒸馏，蒸馏。
蒸馏，蒸馏。

![巽哥的PBL知识库](https://mmbiz.qpic.cn/sz_mmbiz_png/hNRklJ0o9FYboWyoQhFlLON1KLLepicYuU6pibGmia3QV2O6Xich5OEiaeJkXUmZXPgJI4OhEl1h6O8LABLXBOAY22XjficUvNB6YYbACNnTa5J8M/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*巽哥的PBL知识库*

既然已经在ima里建了一个“巽哥的PBL知识库”，数百篇关于项目式学习的文章在里边，那就不能浪费。

最近ima出了copilot的功能模块，用上ima-skill-creator，就可以开始定向“蒸馏”知识库了：先让大模型充分读取ima知识库里的信息，知道怎么一步步引导教师设计课程 → 我们把这个推理过程"蒸馏"成了一个可复用的Skill → 下次不需要再读那些文章，加载Skill就能直接干活。

## 01 让AI"吃透"知识库。
让AI"吃透"知识库。

![犹哥的小伙伴](https://mmbiz.qpic.cn/sz_mmbiz_png/hNRklJ0o9Fb5H4w7e89RaaxhJghroW5B9rnzy18WHGAhXibAticIKiaiayp3aQkXkxjblIaGJeicwJgbWiajczAwmSZAfDAPhv4pTKMzgaO7VQlibI/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*犹哥的小伙伴*

首先，我没有让AI凭空编造，而是要求它只从我的PBL知识库中获取信息。它在知识库里读取到——PBL教师支架工具包、DESIGN六步法、以证据为中心的评价设计模型、常规课堂实施策略、案例设计流程……，提炼出了PBL设计的底层逻辑。

这里其实做了两次，一次在ima-copilot，另一次在workbuddy中部署ima skill，获取我自己ima账号的API Key。

## 02 搭建初版技能。
搭建初版技能。

基于知识库内容，AI搭建了一个七步法的PBL课程设计技能——从确定主题、设计驱动问题、设定学习目标，到规划任务链、设计评价方案、实施准备与反思。每一步都配有"引导教师思考"的问题和知识库中的参考示例，还按需加载了驱动问题设计指南、评价量规等参考文档。

初版出来后，我觉得还行——方法论扎实，交互设计清晰，但总觉得还不够。

## 03 两个初版的交叉PK。
两个初版的交叉PK。

![我还从别的地方创建了一个类似的skill，我要怎么才能让你比较两个skill的优劣之处呢｜有两个方式可以让我帮你比较两个 skill的优劣，你选哪种方便:](https://mmbiz.qpic.cn/mmbiz_png/hNRklJ0o9FZWrNAThArHAxjkKicqIcRenP9ib7wJ5agKUfJamo9twQ0BcKcSYZbKia8fI5CCsP8Qd5WCIMUCynmuj62zTMB0SHZZiaRHZKlHGzo/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*我还从别的地方创建了一个类似的skill，我要怎么才能让你比较两个skill的优劣之处呢｜有两个方式可以让我帮你比较两个 skill的优劣，你选哪种方便:*

同样在ima-copilot和workbuddy中，上传另外一个skill的各个.md文件，让AI充分理解和判断两个版本的优劣。

此时觉得我真坏，但有时我们确实可以用这样的互质、互鉴、互搏的方式来提高质量。

## 04 互融合并，迭代升级。
互融合并，迭代升级。

![PBL课程设计助手｜该技能数据来源于 SkillHub，作者是巽哥](https://mmbiz.qpic.cn/sz_mmbiz_png/hNRklJ0o9FaKRagRtoSbGgjzzIx2TOqlhGgW4Dym0Z9mR5RRMR9Q5UULMwlsyRzJWfFAibS3MeEeibYgLE7cL2C43hjlicd6sOCYibWQ45I7HI0/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*PBL课程设计助手｜该技能数据来源于 SkillHub，作者是巽哥*

## 05 人机协同的真正价值。
人机协同的真正价值。这个过程给我最大的启发是：AI不是替我们思考，而是帮我们把已有的思考结构化。

知识库是我积累的，AI只是从中提取和整理；两个版本的优劣判断，需要我提供对比素材，AI才能做出分析；合并方向需要我确认"可以"，AI才动手整合。

如果没有人的知识积累和判断，AI只能产出"正确但平庸"的东西。而当人的专业积累遇上AI的结构化能力，产出的才是真正有用的工具。

同样，当加载、调用这个skill后，AI不会一次性帮我们生成一个项目式教学设计，需要我们在人机协同下，一步一步生成。

![广东省郑巽名教师工作室｜在思考的世界里,学以成人](https://mmbiz.qpic.cn/mmbiz_png/hNRklJ0o9FaO2IArnoAcZHnLCic7Mpa0AjgibYAQxDLiavTxicPHwfc7KL5sicyyOIgo1yWVuf13azXRGQgMQv8nA6YosvomllstlZ8sHl4pl4ag/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*广东省郑巽名教师工作室｜在思考的世界里,学以成人*
