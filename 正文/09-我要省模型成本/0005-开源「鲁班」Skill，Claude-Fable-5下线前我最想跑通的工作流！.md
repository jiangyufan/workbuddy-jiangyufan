---
title: "开源「鲁班」Skill，Claude Fable 5下线前我最想跑通的工作流！"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/346"
type: "skill"
chars: 4109
sections: 0
figures: 0
chapter: "09-我要省模型成本"
---

# 开源「鲁班」Skill，Claude Fable 5下线前我最想跑通的工作流！
来不及解释了，。

Claude Fable 5昨天上线，定位是Mythos的安全公开版。回忆一下4月份的Mythos当时就是称之为神话级模型，找出了1万多个零日漏洞，我刚拿到这个模型的时候，其实有点不知道该测什么。

这次开放得很突然，窗口也很短。从昨天到6月22日（就剩11天了），Pro，Max，Team都能在订阅里用到Fable 5。6月23日之后，它会先从订阅方案里移除，就开始烧API了，后面什么时候再回来，要看官方容量。

如果你是Claude订阅用户，我的建议很简单。这十几天，别拿Fable 5问日常问题。拿它做一件你一直想做，但平时觉得太麻烦很费脑子的事。

我是100刀的Claude Max会员，刚开始也学着想玩玩宝可梦，结果玩一半都不到额度就没了。所以我这24小时没有让它闲聊，也没有让它写文章看看写作是不是比Opus好很多。

我让它帮我做了一个Skill。更准确一点，是一个专门升级Skill的Skill。我给它起了个名字，叫鲁班Skill。

![把你的Skill拿到班门前，让祖师爷重新打磨一遍。｜安装·五个动作·实战战绩·它和同类有什么不同·安全边界·致谢](https://mmbiz.qpic.cn/sz_mmbiz_png/VNz1x8bH8FxB0Rlhx7jsw2d7uBiad3XPeFacjJRX2kw9q5PRdF7TZHz2B5D7gEliaxkPOjEjKsgqxPS0Eib3VtCaqR2YluIHQVlDdvUqFANtew/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*把你的Skill拿到班门前，让祖师爷重新打磨一遍。｜安装·五个动作·实战战绩·它和同类有什么不同·安全边界·致谢*

github. com/LearnPrompt/luban-skill。它在一轮打磨之后，把我的ai new rader升级到了v0.7版本，直接上GIF就知道了，。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/VNz1x8bH8FzPxAVaNicChA72hF0P2cwkKWvXpNqeNNicMIPm34LyUpNh7GmNTic08F1IsaWyS0NLibHvDu8adkatwss6jAibfkRHhuPSSxicygrNI/640?wx_fmt=gif&amp;from=appmsg#imgIndex=1)

为了让别人在第一时间，用10秒钟就能了解到这个ai news rader Skill能干嘛，。

Fable 5甚至用我电脑录制了一段完整的视频传到了Readme，这段视频我一秒钟都没剪它自己甚至把模型生成过程的多余的时间剪辑掉了，就离谱。

除此之外，他还把我这个项目里原本表达了思路但没讲透的优势，打包成了同一个项目另外一个 Skill，ai rader，这样，Agent通过安装这个Skill就可以直接读取聚合后的一手信息。

还不止，鲁班Skill是会通过横纵的方法吸收同类型Skill的优势的（后面会详细拆解），这些优势不是我跟Agent凭空讨论或者一拍脑袋就想去迭代的，而是同类型项目拉开差距的特有功能。

通过判断Github项目的Star数历史和Release记录。通过这些数据来判断它做了什么样的功能，从而导致它的Star有了一个非常快的提升。

所以一轮打磨之后还帮我追加了热点模式和时间轴模式。

![](https://mmbiz.qpic.cn/mmbiz_gif/VNz1x8bH8FxSdTZKDEqFJQQkSqEWqGFMNdHVdaU2KItT9MovdNuXYTicr0hlLwYEUwBibOtqBCxaDs5URSt65ASvvq2MJocUjbq0NZ4vfWlvw/640?wx_fmt=gif&amp;from=appmsg#imgIndex=2)

同时，它还提升了给消息打分的门槛。之前发现很多得分都在 100 分，是因为在信息源里面，如果AI信息源占比过多，分值权重就会很大。但对于聚合站来说，AI占比多并不代表完全的质量，。

所以Fable 5专门做了一个评分的回测工具，算法我也全部公开出来了，让大家来看看这个Fable 5的代码水平怎么样。

所以，这就是一次打磨后的效果，。

![v0.7:从时间线到热点雷达｜v0.6把分散的消息合并了故事线。v0.7回答的是下一个问题:](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FziaQ38KoGuNulmSJ1XueY1K9NMfyZdZ6Pejo5H9gzGfYiaY6YbsE9ib10XkxDric9Av7chyCzI0T3MhY0EEHJiaI4swj1taWiaeH9U8/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*v0.7:从时间线到热点雷达｜v0.6把分散的消息合并了故事线。v0.7回答的是下一个问题:*

更有意思的点是，我想给他开全量权限，让他连夜跑完的时候，Fable 5是会主动去预测，它改完这个项目后面的所有想要用的权限，只开放这方面的权限。

![早安总结:三件事都做完了，分支领先 master 5 个提交｜的失败清理把我的工作目录连同两个未推送提交删了。你刚写好的 radar](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FzBia7xTDCMc3ulibbDNxOVT6k64Ydic0BdicIyQ5AWJD0OD1dSXuqRnXzlsPeZ1xL7gHXEicmzabicZ4tcavYayEib0RW2o1wZAuIibtQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*早安总结:三件事都做完了，分支领先 master 5 个提交｜的失败清理把我的工作目录连同两个未推送提交删了。你刚写好的 radar*

那这个升级Skill的Skill为什么叫鲁班呢。

因为它干的是把一块已经能用、但还很粗糙的木料（本地给自己用的Skill），刨平、校准、开榫、打磨，最后变成一个别人真的愿意拿走、安装、复用的东西（能公开到Github上给所有人用的高水准Skill）。

这也是我最近越来越强烈的一个感受。

很多人以为Skill是一个很神秘的东西，好像里面一定要有复杂脚本，自动化流程，MCP，浏览器操作啥啥啥的。

但大量真正好用的Skill，主体其实就是提示语。一段写得足够清楚，边界足够明确，失败模式足够多的提示语。我常用的20万星的superpowers和1.5万星的pm-skills就是最好的例子。这次的鲁班Skill也是这个思路，。这段时间我看了很多Skill，有GitHub上的，有ClawHub上的，也有自己写着写着沉淀出来的。

然后我发现一个挺尴尬的问题。能用，和能发布，中间差着一大截。基本上所有的Agent都会有Skill Creator这个初始的Skill。

确实，你可以直接跟Agent说你的需求，让它打包成为一个可以在自己电脑上、在自己的 Agent 上能够顺利运行的 Skill。我Hermes給我打包的Skill都上百个了，但我也就打磨开源了10%不到。

![当前状态:活动｜当前状态:活动](https://mmbiz.qpic.cn/mmbiz_jpg/VNz1x8bH8FyhzHfUicUSVxMJGaTYnZmMibrcAh3SsbdpT6BeLiaIRSAazlGoVJ08EodTarVyZgLKUSDG4zIS4QrDgg7Jr0ta8V5SfGAphQ33Q0/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=5)

*当前状态:活动｜当前状态:活动*

一个Skill在自己电脑上能跑，不代表能看懂。别人看得懂，不代表愿意安装。愿意安装，不代表三分钟内能跑出一次工作流闭环。这就是很多Skill发布的时候卡住的地方。它像一个没有验收标准的手艺活，。你问Agent帮你改SKILL.md，它大概率会干什么。

加几个小标题，补一点触发词，写一段更漂亮的description，再把README整理得工整一点。有用吗。有但不大。

所以我给Claude Fable 5的任务，不是让它润色一个Skill，而是让它打磨我的ai new rader项目，完成一个完整的升级流程。

从这一次升级里面提取出来的这个鲁班 Skill，当然随着它改的项目越来越多，鲁班Skill肯定还会发布 2.0 甚至 3.0 版本的。但是留給Fable 5的时间不多了，我决定先把1.0版本开源。

第一步，先挑战前提，。会分出去一个掌柜的（产品经理），判断这件工具到底解决谁的什么问题，为什么值得安装。# skill.md 部分节选1。真实问题：这个Skill解决的真实用户问题是否成立。

独特角度：它的唯一性来自方法论、脚本资产、私有经验、数据、工作流还是展示效果。如果没有唯一性，直接指出同质化风险。

安装理由：用户为什么要安装它，而不是临时问Agent。公共传播性：它有没有一句话传播钩子。有没有可截图、可录屏、可展示的结果。这个Skill解决的问题真的成立吗。用户为什么要安装它。它有没有独特的方法论、脚本资产、数据、工作流、展示效果。它有没有一句话能讲出去的传播钩子。

这些问题先答上来再改。因为大部分Skill的问题是压根没想清楚为什么值得存在。第二步，去找同类。鲁班师爷会派几个行脚去找同类型的Skill，分析它们为什么被收藏，安装和传播。# skill.md 部分节选2。并行搜索策略。使用子Agent并行搜索提高效率。建议的分工：

子Agent 1 — GitHub同行：搜 skill、 agent skill、 SKILL.md、 Claude skill、 OpenClaw skill。

子Agent 2 — Skill市场：ClawHub、skills.sh、Tessl等目录里的同类分类、热门Skill、相近工作流。

子Agent 3（用户指定了对标时才需要）：深读用户指定的对标仓库或Skill，分析它的README、安装路径、showcase做法。

搜索词从当前Skill的name、description、README首屏、核心任务中提取，生成三组：功能词（它做什么）、人群词（谁会用）、形态词（skill/agent/runtime名）。

这也是我觉得Fable 5比普通模型更适合干这件事的地方。

它会去横向看GitHub、ClawHub、skills.sh、Tessl这些地方里相近的东西。哪些是直接竞品，哪些是间接竞品，哪些虽然不是同类，但README、命名、showcase做得特别好，值得借鉴。

![最后返回一个markdown表格](https://mmbiz.qpic.cn/sz_mmbiz_png/VNz1x8bH8FyzpQEOrUqjqvPMRRqVXHQngJdWq0MEUgaSvqvcrnxA8NTibOAHWfiboxoNLlRf5bgxz3qMibVKpIIhj0dsTaudl9dmoc311YicP1M/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*最后返回一个markdown表格*

第三步，是我从HV Analysis里借来的横纵分析。# skill.md 部分节选3。纵向：这个Skill从哪里来，要走向哪里。它最初是为了解决什么具体痛点。它现在是工具、方法论、工作流、风格迁移、还是自动化系统。它从"私用"变成"公开可用"还缺哪一步。

下一版最该从哪条路演进：更强功能、更好展示、更稳安装、更通用适配、更高验证。横向：行情里的同类凭什么立足。至少从以下维度判断：命名钩子：名字有没有记忆点。是否一听就知道解决什么。一句话定位：是否用人话说清楚用途。安装摩擦：是否一条命令能装。是否需要复杂前置条件。

首屏信任：README首屏有没有徽章、GIF、截图、结果样例、真实数据。可验证产物：跑完后有没有HTML、PDF、报告、卡片、diff、测试结果等"看得见"的东西。

安全边界：有没有说明不会乱删、不会泄露、不会擅自发外部请求。生态兼容：是否明确兼容多个Agent runtime。故事感：它是不是在讲"为什么现在需要这个Skill"，而不是只列功能。纵向看，这个Skill从哪个真实需求里长出来，现在解决什么，下一版应该往哪里走。

横向看，同类Skill为什么更容易被理解、更容易被收藏、更容易被安装。最后交叉出一个判断。

![类型:直接｜一句话定位:说句中文就出AI简报](https://mmbiz.qpic.cn/sz_mmbiz_jpg/VNz1x8bH8Fzy0RbL9hg66iagwWpGFia7CqRvdys4ZMTWYicRZm5YOibBOQNG0at1sMiaexCx125589gWPa7Re6pPAdSqxibCzYv5rzmMfR2qaqQJA/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=7)

*类型:直接｜一句话定位:说句中文就出AI简报*

我们真正要抢的生态位，到底是什么。Fable 5给我的一个判断就很有意思。它没有把重点放在「再做一个更好的AI日报网站」上。它反而指出，真正有差异的地方，是GitHub Pages上那份静态JSON。也就是，它天然就是一个不需要鉴权、不会被下线、可以fork、可以直接curl的开放数据接口。

我当时看到这个判断，确实愣了一下。因为这不是一个功能建议。这是生态位判断。按我以前的思路，大概率还会继续往页面、订阅、信息源、展示样式上加东西。但它把我从「做一个更好的新闻站」这条路，。拽到了「把自己的公开数据接口说清楚」这条路。第四步，是Darwin式评分。

鲁班师爷会派个量尺师傅来测出最先要打磨的面。

![第四步:过尺-活体检查+九维评分｜先量活体，再量文件](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FxfFBHuCTFgwArd2dZAuicLxCrAdOnwdjwjAARnmySpU3TpO6RbtMjvviboDq72Zc3BYwe31gldWZ3H2AHzLNjOsiaF7aia6oNiawjk/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*第四步:过尺-活体检查+九维评分｜先量活体，再量文件*

这里我让鲁班Skill固定用9个维度打分，Frontmatter与触发条件、工作流清晰度、失败模式、检查点、可执行具体性、资源整合度、整体架构、实测表现等等。

里面权重最高的是实测表现。

也就是说，一个Skill写得再漂亮，如果没有测试prompt，没有前后对比，没有真实输出样例，它也不能算升级成功。

这点我觉得很适合拿来给所有Skill当体检表。

![](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8Fz7FhBa0Vic7BadpEtGHHEQVcbA0lZN8mlTxhFh1icrBqsUrGyqg53eD2X0D4qYMNe01WAhOjFAibk8PNiaJ4eIMgOUJZ4kCmQw2vE/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)
