---
title: "WorkBuddy 实战教程--玩转skill：我的第一个skill-数学金牌教"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/400"
type: "skill"
chars: 3157
sections: 5
figures: 0
chapter: "10-我要写代码和做自动化"
---

# WorkBuddy 实战教程--玩转skill：我的第一个skill-数学金牌教
![创建你的第一个 Skill｜创建你的第一个 Skill](https://mmbiz.qpic.cn/sz_mmbiz_png/E864uqzGa0NPqxVYKBQzuzeJ9IgicfNBBp1FpM5hwcIkZutiaiamf02snTPsUaZVkrk1IEQ3Nro4CvssSUDHcjFuUI3vWNnolK3NEqnVyTInXA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*创建你的第一个 Skill｜创建你的第一个 Skill*

![专家中心我的专家｜将数学降维成交互HTML的学院派教练。画图解讲、方程确认、错题深度诊断···](https://mmbiz.qpic.cn/sz_mmbiz_jpg/E864uqzGa0PjkPAAicbbT7YO9rHib8tzbuEqI6ZCoPLAbExZaKsIoskAbozDVLCCNA4dGcQvY4959r9KDjaLsnsky4bD9UOkicKKkG0XaicbbK4/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=1)

*专家中心我的专家｜将数学降维成交互HTML的学院派教练。画图解讲、方程确认、错题深度诊断···*

我的私人专家库，还在增加中。

## 一、先搞懂：什么是 Skill。
如果说 WorkBuddy 是一部智能手机，那么 Skill 就是装在里面的“王牌 App”。

作为官方的“专业工具包”，WorkBuddy 哪怕自带了 20 多种涵盖文档、表格、PPT 的原生技能，也依然有一个无法解决的硬伤：官方再懂 AI，也不可能懂你的具体业务。

你的独特场景、大厂 SOP、死磕出来的输出标准，只有你自己最清楚。所以新瓶装新酒，自定义 Skill，就是把你的个人经验，打包固化为 AI 的“专属超能力”。

它死死掐住了我们在日常办公中的 4 个痛点：【告别低效】 解决重复输入 Prompt 耗时易错一句话触发，一劳永逸。【沉淀资产】 解决个人经验难以传承 技能即资产，永久沉淀。【稳定输出】解决 AI 盲盒式输出质量不稳定固化 SOP，严控质量标准。

【团队赋能】 解决好工具无法团队共享 一键分发，全员生产力升级。

## 二、创建你的第一个 Skill：四步走。

![](https://mmbiz.qpic.cn/mmbiz_png/E864uqzGa0MX51ToGza4dQ9D8h1sMfQ9y3kbibzkdcAIe3xibxebOe91XbAKmjo8ZFhB6tAz2RgWf9ZeRsPxzBZteoZkswZ4K9KWKwnNVB6xE/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

上图是我把文章扔给我的生图助手生成的。创建一个自定义 Skill 并不需要任何编程基础，核心流程其实只有简单的四步：第 1 步：梳理你的 SOP（标准作业程序）。把你平时重复在做的工作流程抽象出来，闭上眼睛回答这四个问题：

- 场景描述：你想把什么工作流程自动化？描述得越具体、越细节越好。
- 触发条件：在什么情况下，你会需要用到这个技能？
- 输出要求：你期望 AI 最终吐出什么格式、什么内容的结果？
- 专业背景：你的行业或专业领域是什么？需要补充哪些背景知识？

建议：刚开始玩，先从你每天/每周都要做的高频重复任务入手。不要贪多，聚焦 1-2 个最痛的场景，跑通闭环最重要。

第 2 步：创建并填写 SKILL.md 文件。

SKILL.md 是这个技能的“灵魂配置文件”，AI 就是通过它来理解「我是谁、我该做什么、我什么时候该出来干活」的。

送你一个偷懒秘籍： 别被 .md 后缀吓到了。你完全可以把上面第 1 步整理好的需求直接扔给 DeepSeek / ChatGPT，对它说：“帮我把这段需求转成标准的 SKILL.md 格式”。我的第一个技能就是这么调教出来的。如果出来效果不完美，就倒逼它迭代修改，在不断微调中自然就熟悉了。

一个标准的 SKILL.md 模板结构如下：

--- title: "你的技能名称" summary: "一句话描述这个技能是干嘛的" read_when: - 触发条件1 - 触发条件2 - 用户说 “xxx” 时触发 --- # 技能标题 你是一位【硬核角色定义 / 专家身份】。收到任务后，请严格按照以下流程执行： 1. 第一步：xxxxx 2. 第二步：xxxxx 3. 第三步：xxxxx ## 输出格式要求 * 必须包含：xxx * 整体排版格式为：xxx。

文件保存路径： .workbuddy/skills/[你的技能名]/SKILL.md。第 3 步：精准设定“触发词”。

触发词（即配置文件中的 read_when）决定了 AI 能不能在正确的时间“秒懂”并自动调用你的技能。设定时请遵循以下三条原则：

- 自然且具体：用你平时大白话会说的话，拒绝抽象生硬的指令。
- 避免歧义：确保它具有排他性，不要和你的其他技能撞车。
- 多留几个入口：列出 2-3 个同义的表达方式，提高 AI 的识别容错率。

✅ 好的触发词示例。❌ 差的触发词示例。

- 用户需要评估选题 - 用户要优化标题
- 分析 (太笼统，日常聊天极易误触发)
- 用户说"帮我看看这个选题"
- 用户需要帮助 (太宽泛，AI 根本不知道该掏出哪个工具)

第 4 步：测试与闭环迭代。

保存好 SKILL.md 文件后，请务必重新开始一轮新对话（这很重要。旧的对话缓存不会加载新技能）。接下来，用你设定的触发词去调教它。

标准的测试流程：

- 1. 唤醒测试：说出触发词，观察 AI 是否成功联动、触发了你的自定义技能。
- 2. 质量检查：检查 AI 吐出的内容和排版，是否完全符合你在配置里定义的格式。
- 3. 丝滑微调：不满意？直接回去修改 SKILL.md 里的流程或角色定义。
- 4. 循环往复：重复测试，直到输出效果稳定达标。

⚠️ 避坑指南：如果发现技能没有被正确调用，优先检查两点：一是 read_when 里的句子跟你的聊天输入匹配度高不高；二是检查技能文件是不是乖乖躺在正确的文件夹路径下。

## 三、我的实战示例：数学金牌教练专家 兼 Skill。

![鸡兔同笼错题精讲｜阿几教练·画图法讲解·适合小学低年级](https://mmbiz.qpic.cn/sz_mmbiz_jpg/E864uqzGa0PjEf4dRR1LrbbhtDbvNB51zsdn2eqvrCr8M3pH0lic5pxsORQDSC5d09Z4YcwcnuToYxq6l3pgsEINrluibRsWzuyBqQmYYzvQ0/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=3)

*鸡兔同笼错题精讲｜阿几教练·画图法讲解·适合小学低年级*

![画图讲解(正确答案)｜第1步:画10个脑袋(圆。)](https://mmbiz.qpic.cn/sz_mmbiz_jpg/E864uqzGa0MXzu1LLNj68pAtUdJtrkh4njlmLrzxKQy3VFwtu6iaRgO5Ed7ia2pce762DrJe88bXiaBKDflJxibVPCWJ5GLh8rZetGib5yXPlFec/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=4)

*画图讲解(正确答案)｜第1步:画10个脑袋(圆。)*

然后我是怎么做的呢。看下面详解：1，点击workbuddy左边栏的专家，然后选我的专家，点击创建专家。

![专家中心我的专家｜嗨扯写作专家](https://mmbiz.qpic.cn/mmbiz_jpg/E864uqzGa0MxTBlSYelN7s2g4v1Nshafcm6Z8Mf6GSrCCuJGhI3d7CbRtXCSsDMRPrDXzialZlfjnxCZNnIXaoCeg05VkxlWw0ibtMXyGygIk/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=5)

*专家中心我的专家｜嗨扯写作专家*

2，然后选把要创建的专家的要求发他（我的专家提示词是DeepSeek写的），你可以再加一句，有什么不去清楚的可以先向我提问，确认后再执行。

![expert-manager帮我创建一个极简几何学派·数学金牌教练｜当接收到用户上传的错题时，你必须首先严格执行【题目诊断】:](https://mmbiz.qpic.cn/sz_mmbiz_jpg/E864uqzGa0ORR6sBaQ7UhM0TOCmf8YKs6wKiaClj2cmteoHogicvxjndgqOnIwQooMqTX9310rV9jNmG0IgQtWK4d9f2WuLPVtRpsnQNXzYibw/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=6)

*expert-manager帮我创建一个极简几何学派·数学金牌教练｜当接收到用户上传的错题时，你必须首先严格执行【题目诊断】:*

3，接着等他和你沟通完后，就等他执行完，然后你就点击测试。

![创建结果总览｜极简几何学派·数学金牌教练](https://mmbiz.qpic.cn/mmbiz_jpg/E864uqzGa0P6zqMBswKlBkd9hCAe5CCZNVlg4Mlw2YeJ318WUSyw5u3GQBLXqAPRdwqxlxibeiaUOFOnw0jpXqWLuKHgSP9wWTdQicetvZ1evs/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=7)

*创建结果总览｜极简几何学派·数学金牌教练*

4，下图是我开始测试，我家娃的一题错题，成果前面放了，这个我后面也调试了几次，也增加了一些内容，等这些结束后，你可以在“我的专家”下面找到你刚创建的专家，恭喜你。你拥有自己的专家了。

![a8b8cfe5515dfad0d9089168fbd2c77d.png 帮我讲解一下｜好的!我看到这是一道小学数学的鸡兔同笼经典题目,而且有学生的解题过程。让我来仔细分析一下。](https://mmbiz.qpic.cn/mmbiz_jpg/E864uqzGa0OaAGqv2Hutww7FtNe1Z4w2BGhayNIJo7laYlBYibjSnrtYqrFE3Ta7zhByHDPzHADj3HgvoCklbndW5b52d6WzQrNILYczNwEk/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=8)

*a8b8cfe5515dfad0d9089168fbd2c77d.png 帮我讲解一下｜好的!我看到这是一道小学数学的鸡兔同笼经典题目,而且有学生的解题过程。让我来仔细分析一下。*

我现在已经创建了3个专家，一个是写作专家团，一个数学辅导专家，还有一个生图专家。

![专家中心我的专家｜覆盖创作全流程的写作专家团，从需求挖掘、框架搭建到执笔校审，多位专…](https://mmbiz.qpic.cn/mmbiz_jpg/E864uqzGa0MVFDoly9XnNOGeBAFhTkl0WgB5C5Ix4RgHibImUqV3PVPGLB4ib3r3MVU1mH7YkuY8htO0SxCyclNZjZ8iaRRhjzsSOeOniaWH6Vc/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=9)

*专家中心我的专家｜覆盖创作全流程的写作专家团，从需求挖掘、框架搭建到执笔校审，多位专…*

## 四、发布你的 Skill。
怎么把专家转成skill，一句话，只要和workbuddy说：帮我把这个专家做成skill。

![热榜 全部技能｜new大赛大赛](https://mmbiz.qpic.cn/sz_mmbiz_jpg/E864uqzGa0NKkDyyZ6R36xs1nFEciaicO7YAwFuL9A2gXHChyiamaNSgfPbo0FOyq1QpZt6VdC6wCl5kgUMvBnchgBx36yh2JxyicZ61jVKYvjI/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=10)

*热榜 全部技能｜new大赛大赛*

## 五、写在最后。
从「用工具」到「造工具」，这是质的变化。你不需要是专业程序员，只需要：

- 清晰地描述你的需求
- 理解问题的本质
- 善用 AI 的能力

你的第一个skill会是什么。每天都要生成的重复性报表。每次都要手动处理的邮件分类。每周都要整理的项目文档。把这些重复劳动变成一个 Skill，一句话搞定，彻底解放双手。

我第一个专家团，其实也有在我的文章中使用过降本还是增效。AI落地正在迎来最残酷的分水岭。现在就打开 WorkBuddy，创建你的第一个 Skill 吧。

#workbuddy#腾讯#qclaw#智能体#agent#skill#专家#技能#skillhub#github#clawhub。

WorkBuddy 迎来史诗级更新。打通 ima，亲手打造你的全自动 AI 助理。WorkBuddy 入门指南。WorkBuddy、QClaw、Marvis 到底怎么选。这篇终于讲明白了。OpenHuman 智能体又一搅局者 深度解读。Obsidian 插件的正确打开方式。

Obsidian 帮我终结信息过载，搭建“终身知识复利”系统。Hermes Agent 必装五款提升 AI Agent 生产力的开源神器。Hermes装一个大脑，它好像变聪明了。Hermes Codex等用户必看：一个软件搞定大模型切换，再也不用改配置文件了。

Hermes Agent 相关网站及资源汇总。

强烈推荐-skill大比拼-Evolver vs OpenSpace：谁才是AIAgent的"记忆大师"。

强烈推荐skill-gstack ：从单一Agent到多角色协作。强烈推荐skill-CLI-Anything：让所有软件都能被 AI 代理驱动。Gdplay玩AI草图 · 让 AI 成为你的生产力，部分图片由AI辅助。
