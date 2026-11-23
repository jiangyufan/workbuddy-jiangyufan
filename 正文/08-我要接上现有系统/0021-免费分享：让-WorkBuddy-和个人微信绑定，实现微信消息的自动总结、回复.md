---
title: "免费分享：让 WorkBuddy 和个人微信绑定，实现微信消息的自动总结、回复"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/596"
type: "tool"
chars: 2090
sections: 0
figures: 0
chapter: "08-我要接上现有系统"
---

# 免费分享：让 WorkBuddy 和个人微信绑定，实现微信消息的自动总结、回复
我看了看，很多方法都是先在电脑上选中需要总结的消息，再转发给微信里的 WorkBuddy，让它帮忙总结。

![转发到其他应用｜群聊的聊天记录](https://mmbiz.qpic.cn/sz_mmbiz_png/lqqnHrRVBQGBxpLwPjJT2Zyn5xFaUeZ7JkKQQDTwWVCC7uCwMNoW7G5sxICg8JjFYzxmLtHCmIWiakoy4CKGm35fU2kNVud79icO7OKOibU4Qk/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*转发到其他应用｜群聊的聊天记录*

AI 辅助总结消息流程。你说有没有用。那肯定有，最起码不用自己一条一条看了。但是吧，我还是得先去选消息，选完再转发。这个过程，我觉得多少还是有点麻烦。能不能连这一步也省掉，让它自己去找。

这个就有意思了。想看哪个群、哪段聊天，直接告诉它，让它去查就行。我这里跑通之后，在 WorkBuddy 上，或者直接在微信里，都可以让它调取消息、做分析。先给大家看一下效果。

![— YESTERDAY IN TATALAB · 昨日群聊｜模型在进化，工具在开源，群友把梗聊成了方法](https://mmbiz.qpic.cn/mmbiz_gif/lqqnHrRVBQGqnQqDqibGMJQhreNJKaQDCeT9k230hs6rsd17xsv49NFAwNLOu2dLh3Qw3ZJuCjSHJVVY7djeZO7vOq6HUW7ADKd7gGtaVyQQ/640?wx_fmt=gif&amp;from=appmsg#imgIndex=1)

*— YESTERDAY IN TATALAB · 昨日群聊｜模型在进化，工具在开源，群友把梗聊成了方法*

说到这不得不佩服这些人，凌晨 0:18 ——晚上 23:56 一直在讨论 AI，说明什么。说明几乎一天 24 小时都不带停的，怪不得这些大佬们懂这么多，都是用时间换出来了。

这也是我见过的最活跃的群（之一）。下面就说说，这套东西怎么弄。先打开 WorkBuddy，找到左侧的专家、技能、连接器入口，进去以后选中「技能」。

在右边的输入框里搜索「WeChat CLI」。这里记得再点一下「Skill Hub」按钮，找到这个技能，直接安装。

![专家技能-连接器｜通过 wechat-cli 读取和...](https://mmbiz.qpic.cn/mmbiz_png/lqqnHrRVBQG5XArmkYKXXPzp3IfVo7iboReicVGQyzEaIejB7uBiaazzHVr0umXa4VUGTgqiaKj2aSoGd3NrneFMrIxmdUgYB6ia6Gr4pOXkibBKQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*专家技能-连接器｜通过 wechat-cli 读取和...*

安装 WeChat CLI 技能。安装好以后，点击和它对话。我先问了一句：你有哪些能力。

![日常办公 代码开发 设计创意｜数据分析及可视化](https://mmbiz.qpic.cn/mmbiz_png/lqqnHrRVBQGw0hdZL9WmkbfzwRdic0AUUpbBNyDND1FvVpdPkfO3f6Lwej0iaglLgDVtuI15OnianTH8C9euoWH9OuralZCsySEl6mEsNvYJDM/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*日常办公 代码开发 设计创意｜数据分析及可视化*

询问技能能力。

结果一问才发现，光把这个技能装上还不够，本机还得先有一个叫 WeChat CLI 的工具，它才能干活。

但按它给的 GitHub 地址去找，我又没找到对应的项目。

![通过 wechat-cli 读取和分析微信聊天记录 你有哪些能力｜这个技能让我能直接读你本机微信已登录账号的聊天数据。这是我刚查到的本机状态：](https://mmbiz.qpic.cn/sz_mmbiz_png/lqqnHrRVBQGpb68CLj55Ciavz9Nm1wsvx6eGnmyjiaTCVRLDSsS1yuPqXZkneVomX87vms5N9d0jpyTJRvq1yA9F62gZHR0MvVbGlL7rR8FibI/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*通过 wechat-cli 读取和分析微信聊天记录 你有哪些能力｜这个技能让我能直接读你本机微信已登录账号的聊天数据。这是我刚查到的本机状态：*

方法就是让 WorkBuddy、Codex 这些智能体帮你找一找，找到还能用的 WeChat CLI 项目，再让它帮你安装。

如果你实在找不到，直接把本文链接发给你的智能体，告诉它：别人的 AI 能找到，你为什么找不到。你要是不能干有的是 AI 能干。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/lqqnHrRVBQG0otkHRYw8M0Bolj08Mwo4MmDzyCI5cXVys5TmicibiavnMmnwO9n14EWjfd7tVAkaQ8cLre6nvELqIIWonOhTsskPajIyxncLTw/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

指令示范。这样，等它告诉你安装好了，就可以拿几个问题试试了。我先问了一个：我这边有多少个微信好友。它很快就把结果发过来了。但是我一核对，哎，这个数好像不太对啊。

![](https://mmbiz.qpic.cn/mmbiz_png/lqqnHrRVBQHS4aB8KLlYXAwwIS6icm0tUySYcqYyNV2bCVljwlHwBOLFicyDv50uXZ1dXXpxWd0FLNNibsU6CSj1hpWpIE0yUjibOQNg1JJxlTw/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

AI 反馈的结果对比。所以，AI 给的结果还是得自己看一下，不能它报个数，咱们就直接信了。

发现不对也没什么，直接告诉它，让它继续改呗。它后来把查询用的 SQL 调整了一下，改完以后，结果看起来就没问题了。

![](https://mmbiz.qpic.cn/mmbiz_png/lqqnHrRVBQELGPK64vfIyuRRCnk2knTwMPWrmzCDCSk6A69FBFHkKAV16GLbPuIpORiaRnoR8sGrryMB00bXfkB0PSFsYVkvn1AicE1icMbvzM/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

修正后的查询结果。

而且，这个查询速度确实挺快。快到什么程度呢。我这边测试，几百条、上千条聊天记录，读取出来不到一秒。

不过这里要分清楚，不到一秒说的是把消息查出来。查询走的是本地脚本，后面让 AI 总结、分析这些内容，才是比较消耗积分或者 Token 的部分。

用到这里，我又觉得还有一个地方不太方便。查消息是省事了，但我总不能每次都打开电脑，再去 WorkBuddy 里问它吧。我们平时最常用的就是微信，那干脆直接在微信里问，能不能行。可以，接着往下弄。

打开 WorkBuddy，点击「助理」，再进入「设置」。这里可以绑定其他通讯平台，微信客服、飞书、钉钉这些都有。

![](https://mmbiz.qpic.cn/mmbiz_png/lqqnHrRVBQF9XFC2h1ic8PuFas627KnRS1D4xoKPNdQqUBhZhgoeibjyqmlo6OaDLhUb3S86Pb8jrib5nNohMUMZAmfvWsbRyNx5dmbQRQfyf0/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

![将 OpenClaw 连接到微信｜连接后将启用 微信ClawBot 插件，可通过聊天的方式连接 OpenClaw。](https://mmbiz.qpic.cn/sz_mmbiz_png/lqqnHrRVBQEiakfqARjxzVmZcndMfUAibcgMtFThzFMagwAuBwPmzzZRmSJwz0zfXUWMaOkyNM0WwrSDaLcT4u92K0o2yuVAPEgibO7beoFB08/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

*将 OpenClaw 连接到微信｜连接后将启用 微信ClawBot 插件，可通过聊天的方式连接 OpenClaw。*

直接在微信对话效果。这个就舒服多了。群名没说全，它也能帮我找到，我还想干什么，在微信里接着问就行。

![TATALAB 一起早起(220)｜TATALAB 一起早睡(500)](https://mmbiz.qpic.cn/mmbiz_png/lqqnHrRVBQFaibskgO0AnoUqnJU5mOjuKjhmjWGuSPlQ45CYtu7fGC6qsekmLb3jDRb4vy5GMUWEDWXsdt2Us1hCJvnEia6tmSxicYDRS03MKs/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*TATALAB 一起早起(220)｜TATALAB 一起早睡(500)*

其实，没有晚睡，只有早起。到这里，从微信里提问，再到查询、分析聊天记录，整个流程就通了。说到这里，我想肯定有大聪明要问了：既然 AI 都能读到微信消息了，那能不能顺便替我回一下。我也顺着这个思路，又做了一个自动回复的测试。不过，这次用的是一个新注册的微信。这样玩有没有风险，我也说不准，所以先拿新微信试了一下。

大家看下面这个演示。

![](https://mmbiz.qpic.cn/mmbiz_gif/lqqnHrRVBQGOC7BDb3FicSZCFBnYIqdyM53UlOPSWbvlu7w3G389K1ZrY3yBjNuBj7t7JxQxHx5G8bxOiaxmibianJ4UtmLpZ7ibNcuAqfteNsqA/640?wx_fmt=gif&amp;from=appmsg#imgIndex=11)

自动回复测试演示。我测试的这个微信，现在接的模型是：deepseek-v4-flash-vision-exp。这个模型收到消息后，可以识别文字、图片，再根据上下文内容，自动回复。而且，回复时的人设、逻辑，包括自己的知识库，也都可以给它设置进去。

你想让它用什么口吻说话、按什么逻辑回答，就往这个方向去调。

![AI原生微信｜AI、联网研究与上下文](https://mmbiz.qpic.cn/sz_mmbiz_png/lqqnHrRVBQHhITRj474c53GBkr3qJg5xyRv4IibiaiccRpfGfIGciciaF6icSXRfYND9RQLIRFqkw71UWUKRFG4mrdPpzwkOES3QNbt286QzJqHias/640?wx_fmt=png&amp;from=appmsg#imgIndex=12)

*AI原生微信｜AI、联网研究与上下文*

回复设置逻辑。所以这里面能玩的东西，还真挺多的。你看，我最开始只是觉得，每次选消息、转发给 AI 有点麻烦。顺着这个想法往下试，就弄出了直接查聊天记录、在微信里问的用法，后面又另外试了自动回复。我觉得，这也是现在 AI 特别好玩的地方。以前你可能只有某一方面的能力，有了一个想法，其他部分却不一定能做。

现在就可以把自己的能力和想法结合起来，缺哪一块，再让 AI 帮你补上。这样一来，就能做出很多好看、好玩的应用。这也许就是 AI 最大的魅力，让看不懂一行代码的我，也可以做一些好玩的应用。写在最后。案例只是一种思路和方法的传递。更多无限的可能还在路上。
