---
title: "Gemini 4 Neon 发布：第 10 号元素「氖」"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/913"
type: "tool"
chars: 2422
sections: 1
figures: 0
chapter: "09-我要省模型成本"
---

# Gemini 4 Neon 发布：第 10 号元素「氖」
刚刚，谷歌发布了 Gemini 4 Neon...也就是元素氖（氦氖氩氪氙氡里的氖）。

价格方面（百万 token），输入 3，缓存0.15，输出 $15，比 Carbon 便宜一些 模型可在 Google AI Studio 进行调用，订阅用户也可在 Gemini App 和 Google Antigravity 使用。

![示意图](https://mmbiz.qpic.cn/mmbiz_jpg/jXSGuwJvpdiaVpZXv6wrhdbTRwy94uJd9mUx4vQuibibOZtGD0EqHicujEqmvbibxHuChR7QErbRCU12qk6RqPR4vqgxiaMriah7oyyUfa1bT4hQss/640?from=appmsg#imgIndex=0)

*示意图*

然后你会突然发现，谷歌这几天发布了一堆元素....先是 Argon（氩，18 号元素），然后 Carbon（碳，6 号），紧接着是 Hydrogen（氢，1 号），今天是 Neon（氖，10 号），咱也没看出个规律，除了说「科技与狠活，它是打算放半个元素周期表进去」。

啊对....在 Google AI Studio 里，模型选择确实是一个元素周期表....非常恶趣味。

**说一下分工吧：**Argon（氩，18 号）： 是最早的基模。

Carbon（碳，6 号）：基于 Argon 后训练而来，目前谷歌家的最强模型，对标 Fable/Astra。

Hydrogen（氢，1 号）：主打便宜大碗，还有免费额度，对标 Sonnet/Terra。Neon（氖，10 号）：新发布的这一个，对标 Opus/Sol。价格信息汇总如下。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_jpg/jXSGuwJvpdjA3gDpibJzq9BfiacRR2WESdCIIYnu7VRLddRBs3Hud5R0abRzib0uRSCicPkWGqO4Q84iaFfSDY8oYkzarYpSSXI3wmDg9nEINNZs/640?from=appmsg#imgIndex=2)

*示意图*

跟着模型一起放出的几段演示（顺便也安利了下其自家的 Google Antigravity）。

首先在多代理协同的数据任务里，一群 Neon agent 把一张图片拆进了 10 万 格的 Google 表格，在未嵌入图片和 Apps Script 的前提下，单靠 50 多万 个实时公式做出了边缘检测、3D 深度计算和重新打光。

从零写大型前端项目时，它独立写出了一个第一人称 WebGL2 自由滑雪模拟器，采用勃朗峰与霞慕尼的真实地形高程，包揽了 10,200 行自写着色器、120Hz 滑雪物理和板状雪崩效果。

## 调度子代理跑完长任务
现在的复杂 Agent 编程，主流架构是一个主模型在上面拆解规划，底下调度一群轻量级 subagent 并行执行。

谷歌把 Neon 设计成上层的 Orchestrator，专门在 Antigravity 里调度成群并行的 Hydrogen 子代理。

这里有两段官方演示，展示的就是这套 /swarm 子代理集群的跑法。一段是调用 Blender MCP 搭出一座照片级的 3D 元素实验台，按化学元素给 Carbon 和 Hydrogen 配上本生灯火焰，给 Argon 和 Neon 配上高压气体放电管。

谷歌 CEO Sundar Pichai 随后转发了这段实验台演示，顺手引用了自己早些时候发的一句“Happy WedNEsday!”，特意把周三里的元素符号大写。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_png/jXSGuwJvpdhxfXSy04iba5mapnLFhJwUA2QGGrUliaNAvWBu4aSChGEdxYv3j05EDicAjIpmNDvxbmrvylkeNicS9iclich4gE0Nib7iaFb11Ipf8Gg/640?from=appmsg#imgIndex=3)

*示意图*

另一段同样动用 /swarm 去翻找历史档案照片，在交互式 3D 场景里复原了 1936 年图灵在剑桥国王学院的书房，从礼拜堂外景一路走进 X.8 房间，桌上的那台通用图灵机真的可以运行。

官方演示之外，提前一天拿到模型的试用者 Chubby（@kimmonismus）在 Antigravity 里测了一整天，让 Neon 做出了 17 个可交互演示，涵盖带海边天际线与 24 小时日照的“港湾都市”、带引力透镜调节的黑洞飞掠，以及浏览器稳定 60 帧的可破坏体素场景。做体素场景时他只提了“能破坏、能重置”，Neon 自己加上了三种建筑，还配了手感各异的大炮和凿子。

![翻译自 英语 显示原文｜一个线程：](https://mmbiz.qpic.cn/sz_mmbiz_jpg/jXSGuwJvpdjJvwcgEazGEaPriay6oAp5l848BibG0vgAe1yLwnzlv06iaxz024ibN7Uzy31ibbeaQMdZYCrmTZQkibCbLRu5r6MDB5zWQTFtbTwac/640?from=appmsg#imgIndex=4)

*翻译自 英语 显示原文｜一个线程：*

落到修代码和审查上，他拿三个带 bug 的程序去测，预订检查器（5 项测试原本只过 1 项）、任务调度器（14 过 8）和异步加载器（16 过 10）修完后全部通过；代码审查里故意埋下的 4 个 bug 也被悉数找出，Neon 甚至主动指出了两个剩下的缺口：预订检查器会拒掉合法的闰秒 23:59:60，文件检查在恰好的时刻换掉文件夹仍能绕过。

![翻译自 英语 显示原文｜在代码审查中，它发现了所有四个我故意植入的bug。](https://mmbiz.qpic.cn/sz_mmbiz_png/jXSGuwJvpdhzpA1YTmmqUyN0XMNia9UJlTmUCbYpuqPN9ibOibd3JhEUanufHuIZGJRY4ibEoXkF9l5HAv2Vxx1W5vsZqHCzwcd1o7GQeu7UW1o/640?from=appmsg#imgIndex=5)

*翻译自 英语 显示原文｜在代码审查中，它发现了所有四个我故意植入的bug。*

他翻看 Antigravity 日志发现，xhigh 档跑完 13 个会话一共触发了 762 次工具调用（读文件 313 次、编辑 266 次、新建文件 104 次、shell 43 次、子代理 13 次、网页搜索 2 次）。为了撑住这么长的链路，Neon 减少了重复读文件的动作，干活过程中会主动汇报进度，长会话里的上下文压缩也保持稳定。Quadrillion 首席科学家 Trenton Chang 评价说，新手研究员是你给什么实验就跑什么，好的研究员会一直问为什么，Neon 是第一个让人感觉像后者的模型。

这个模型并没有去挑战 Fable 一类的（确实打不过 hhhh），而是选了新近发布的 Opus 5.5 和 GPT-6.2 Sol。面对同样开到最高思考档的 Claude Opus 5.5 和 GPT-6.2 Sol，Neon 在 18 项测试里赢下了 15 项。

然后这里有个有趣的事情，各家模型在使用自己的 harness 时，性能获得了显著提升，如下图：

![示意图](https://mmbiz.qpic.cn/mmbiz_jpg/jXSGuwJvpdiavhsLjZMRoefkVBFaKiaP7COdGQIQmGZYb5Gxbm1Ft2Pjoe8Uprer5MtKnQ0X2rNCejNyVW818JVCMv13rr5S8uRKJksX8p1NQ/640?from=appmsg#imgIndex=7)

*示意图*

外部编程工具的实测也印证了这个定位。当天接入 Neon 的 Cursor 测出，默认档在 CursorBench 4.1 上拿到 63.7%（高于 Hydrogen 的 57.3%），单任务平均花费 $6.54，处在性价比曲线的最前沿。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_png/jXSGuwJvpdhIa0qqBQZXFcCNpIDhib6fXXDKWBEx85rSGDYLWy5TOF9CNtevK0veMlibJRl0EAd2Y1EhJbgXUjo2eUQVqy5HXHHoQDGTiaNUKc/640?from=appmsg#imgIndex=8)

*示意图*

编程之外，Neon 的 Artificial Analysis（AA）综合指数拿到 61（Opus 5.5 为 59，Sol 为 57），排在总榜第 3，仅次于规模更大、速度更慢的模型。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_jpg/jXSGuwJvpdgVztvKPXRbCHz8Wto4haAf8TlJXHfAfguUR3TqjGaljNP7WHBEG0XibicLLB6WOfyM52t8WJz9DGp0PkT7dc8gNzISoaOMuodog/640?from=appmsg#imgIndex=9)

*示意图*

放到真实交互榜单上看，Neon 在模拟长期经营生意的 Vending-Bench 2（$16,843）和 AA Coding Agent Index（58.6）上拿到了第 1。

![翻译自 英语 显示原文｜凭借基于 Arena 全球社区 4.2k 个真实世界代理会话的 1336 分，它超越了：](https://mmbiz.qpic.cn/mmbiz_png/jXSGuwJvpdjNsD9yx5CqGcGS1l39GUmvvw662icTMxbZIU9M2Z28SrXMlyh6eQBG4H2ibNUfjsEFPuMuC08hBibyfQQ5IhWfgtLhtDs5y7UfhQ/640?from=appmsg#imgIndex=10)

*翻译自 英语 显示原文｜凭借基于 Arena 全球社区 4.2k 个真实世界代理会话的 1336 分，它超越了：*

除了常规的模型之外，面向安全领域谷歌还准备了专门的 Gemini 4 Neon for cyber，未来几天会通过 Fairwind 计划逐步开放给受信任的用户。

以及...信息插播。

Anthropic 的 IPO 发行价定为 每股 83 美元（高于此前 70 至 78 美元的指导区间），预计于当地时间 2026 年 11 月 19 日在纳斯达克开始交易，股票代码为 ANT。
