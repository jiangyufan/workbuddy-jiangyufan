---
title: "腾讯司内实践：手把手教你如何用 Skill 与 AI 协作"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/341"
type: "skill"
chars: 2590
sections: 6
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 腾讯司内实践：手把手教你如何用 Skill 与 AI 协作
![](https://mmbiz.qpic.cn/mmbiz_gif/u0lmmJTuFHgZaOfHW6VwNe0UDbXdibVVJ40XrYFe81kUQ8vghddibjRg9cVHQWjMmibQqpict4WjPI284e6cL9ibgwzQuaI8y488dV5uO0G4Zdc8/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

AI 时代，我们如何面对海量信息，真正用 AI 能力帮助自我迭代。这位腾讯员工给出了他的答案，他把日常学习、设计和构建项目的方法，做成了三个 Skill，帮助个人成为超级个体。

![](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHjQMIhZtelwB782dvUl2HXria8YcCFj6Hbz2g0XBniapUBWKVxeTCChI2HRXQPBxcBNlKQHo9hYmCy9rXuvRicg5A0j4grgT8FwCk/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

Balance Li，腾讯产品经理。

这篇文章重点介绍其中的 Learning skill，为大家介绍怎样用 WorkBuddy 演示生成专属学习 Skill，再用它制定计划、练习、复盘和保存笔记。

以下是 Balance 的自述，你也可以换成自己的主题，跟着步骤尝试。

## 01 从工作出发 工作不断变化，好的方法值得留下。
工作不断变化，好的方法值得留下。

我做产品工作，负责法务 AI 建设。日常主要做三类事：学习一个新领域、设计产品方案，以及制作 Skill 或系统 Demo。

以知识库为例，做方案前，我需要弄清楚相关技术能解决哪些问题；设计时，要想清楚谁会用、怎么用，以及哪些需求暂时不做；之后，再做出 Demo，检查方案是否可行。任务各不相同，做事的方法却有不少共通之处。

用 AI 学习时，可能会遇到这样的情况：聊了很多，也看懂了不少解释，却越来越不清楚自己究竟要学到什么程度。等到工作中需要做判断，才发现自己记住了术语，却不知该怎么用。换个对话，之前学到哪儿、还有什么没弄懂，又要重新交代。

于是，我想把学习中几件容易漏掉的事固定下来：先说清目标，再按步骤学习，学完做练习，最后记下进度和收获。能不能让 AI 持续按这套方法帮我。

另外，我也将我自己的三个高频工作场景需要固定下来的内容做成了 skill 生成器，按任务需要选用，三个场景可以单独使用，也可以按项目需要接着做。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHjpamNsOuhb6Tea34JNFIqxwl1icfB9SFSL0BacUdNbqJCszazqcbBhibHkxhpD0iakFUQsFzlxBIPwZkWF4onBt1KYDxzqYfqmSg/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

01 系统学习。LEARNING。理解陌生领域，学会作出有依据的判断。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHjMKsKgLf0Vfj6828Jtvd2rmvjPY6DqGkNQleiaVjj4qtUqaE8DxdlDvZLSn7xlj7hEOpRFxib6GBmhGzkwsJYMpbdJQ9Eez94Go/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

02产品设计。DESIGN。想清目标和限制，形成可供评审的方案。

![](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHjZ8TxhFicICa5hIzkm8IqjNsUo7tNPy1QTL5jScG1NfyQgPWzHrVa2IKDNiaNvd8T0Y9UHUdKyIpribHibaeibYJVNt2oR6VROSNQM/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

03构建与验证。BUILD。实现 Skill 或 Demo，检查结果是否满足目标。

## 02 把方法做成工具 三个生成器，为不同任务准备专属 Skill。
三个生成器，为不同任务准备专属 Skill。

围绕这三类工作，我开发了 Learning、Design、Build 三个 Skill 生成器，都已上线公司内部市场。你可以把 Skill 理解为一份给 AI 助手的工作说明：该按什么步骤做、遇到什么情况要追问、怎样检查结果，以及哪些内容需要保存。

我把它们设计成生成器，是希望同一套方法能适应不同任务：先了解你的需求，再生成一个专属的子 Skill。例如，同样用 Learning 生成器，学 SQL 和学英语时，目标、学习内容和练习方式都会有所不同。

![](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHgXYVwLmprpWOX271X66keq6NE9G60hYNmm4OREibYrbRz366vFczEHhC4XCiciaBwib0Uw1CbnSkHJ9fiav1vcXMibarglyRVZ6WiaQI/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

这些生成器产出的子 Skill，会根据项目进展引导下一步。比如，做设计时发现新信息与原先的判断矛盾，就会建议重新检查需求或方案；做开发时测试发现问题，就会回头检查设计或技术选择。进度和重要决定会保存在项目文件里。

WorkBuddy·学习流程示意·分两步使用，先生成学习项目子 Skill，再用它制定计划、安排练习和保存笔记。

- 你的需求

主题 / 目标 / 基础 / 条件。

- 生成器

澄清需求，生成并预览。

- 专属子 Skill

项目背景，流程与保存规则。

- WorkBuddy 引导学习

讲解 / 练习 / 记录 / 继续。

## 第一步·生成专属 Skill。
生成器交付 SKILL.md 和配套指南。

## 第二步·使用子 Skill。
在 WorkBuddy 中调用它，开始学习。

Build 生成器先交付一份指导构建工作的 Skill。接下来，还要按它的引导制作、测试业务 Skill 或 Demo。三个生成器可以配合使用，但需要你按任务选择，并不会自动依次运行。

我选择 Learning 来展开介绍，是因为几乎每个人都有学习需求。用它做例子，更容易看清一套方法怎样落实到与 AI 的每一步对话中。

## 03 Learning 怎样引导学习 把“学完能做什么”，放进每一步。
把“学完能做什么”，放进每一步。

我给 Learning 安排的第一步，是帮你明确学习目标。“了解 RAG”太笼统，不容易判断是否学会。换成“能画出基本流程、分析可能出错的环节、提出方案评审问题”，就能据此决定学什么、学多深。

目标确定后，AI 助手会把内容分成几个模块，再把每个模块拆成较小的学习点。每个学习点按下面五步进行，合起来就是一次学习闭环：

一个学习点的五个步骤·你 × WorkBuddy。01 输入 — 讲清概念，明确本次目标。02 学习 — 讨论与追问，逐步展开。03 确认 — 发现盲区，纠正理解。04 验收 — 练习或案例，检验会不会用。05 沉淀 — 保存笔记，更新进度。

理解有偏差就补讲，验收未通过，就补练后再次检验。完成一个学习点，再学下一个。

这里的“验收”，就是用一个任务检查自己是否学会了：可以写一段查询、分析一个案例，或模拟一次工作讨论。我保留了跳过某次验收的选择，但建议第一次尝试时先做一次练习，因为实际做过，往往才能发现哪些地方还不会。

学完一个模块，还要回头想一想：这些知识点有什么关系。之前没懂的地方解决了吗。遇到一个复杂问题，能不能一起用上。整个项目结束时，再整理成框架或总结，也记下还需要继续学的内容。

AI 可以帮助解释、出题和整理。是否真的学会，要看自己能否解释清楚、实际用上。

为了让学习能持续下去，我也把保存记录的规则写进了子 Skill：计划里记进度，笔记里记收获和疑问，模块总结里梳理知识之间的关系。下次对话时，AI 助手重新读取这些文件，就能知道接下来该学什么。它靠项目文件记住进度。

## 04 完整实操 跟着一个 RAG 学习项目走一遍。
跟着一个 RAG 学习项目走一遍。

下面，我选一个贴近自己工作的主题——RAG（检索增强生成），用 WorkBuddy 演示具体用法。简单说，RAG 就是先找相关资料，再让模型参考这些资料回答问题。

![本次学习任务｜教学演示案例](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHia4L2yNOSaS1ZibqGCePKiczpETEcViaotia0iaGHX0L5A1d90VaxQYPL7v5NTFiaA2Qrdc6Fv25tK4iatfxFgZvRtn84qicImhZlbagyc/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*本次学习任务｜教学演示案例*

为方便大家照着操作，我把下面的学习计划、WorkBuddy 对话和成果都写成了示例，重点展示每一步怎么做。

01｜在 WorkBuddy 中准备好学习环境。

开始前，确认 WorkBuddy 已识别 skill-creator-learning，并能在当前工作空间保存文件。学习涉及技术版本、工具参数等容易变化的信息时，还需要能检索外部资料。

我用 WorkBuddy 展示这套用法，配图是流程和对话示意。具体安装入口和操作界面，以你使用的版本为准。

02｜一次提供四项信息，减少来回补问。

安装后，在 WorkBuddy 中输入下面这段话。说清主题、目标、基础和时间即可；如果对讲解或练习方式有偏好，也可以一起说明。
