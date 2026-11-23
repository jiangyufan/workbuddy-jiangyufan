---
title: "不想露脸也能做短视频？用 WorkBuddy 造一个口播数字人全流程"
source: "https://workbuddy.jiangyufan.com/index/hub/case/576"
type: "case"
chars: 2209
sections: 0
figures: 0
chapter: "05-我要做内容"
---

# 不想露脸也能做短视频？用 WorkBuddy 造一个口播数字人全流程
![关注狂想AI，让想象流动，学好AI不迷路](https://mmbiz.qpic.cn/mmbiz_gif/ZYIUeP9by5qm3kYHoSQc5uicGT6DLibHhMWuicibtGvLfnQdk0sU8zepFHDtjNzdcSD2yRXvbdo1uE9Npk7eUz7hibVxkeEg7noaUSYmnE4mDZLY/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

*关注狂想AI，让想象流动，学好AI不迷路*

很多人想做自媒体，但卡在两件事上：一怕镜头，二懒得录。 其实这两件事都能交给工具。这篇文章讲清楚一件事——用 WorkBuddy 当「总调度」，把「写文案 → 复刻声音 → 生成数字人 → 剪辑成片」串成一条自动化流水线。你只需要给个主题，或者一段想法，剩下的让 AI 工具一步步跑。看完你就能照着搭出自己的第一支数字人口播视频，不用自己出镜，也不用反复念稿。

为什么是「数字人」，而不是硬着头皮出镜。

做短视频最低的门槛，从来不是设备，是「我到底要不要露脸」。 镜头焦虑、没状态、声音不想被听见——这些都很正常，不是你一个人的问题。

退一步想：我们要的是「一个能稳定开口讲内容的人」，不一定是真人本尊。现在的技术已经能做到——用你的一张照片，生成一个长得像你、说话像你的数字人。再配上写好的文案和你自己的声音，一条口播视频就出来了。

关键不在于「数字人有多炫」，而在于：这件事能不能变成一个可重复的流水线，而不是每次都从零手忙脚乱。

文案：两套 skill，分别伺候两类人。整条流水线里，文案是地基。但不同的人，起点完全不一样，所以不能用同一套打法。@高要求人群 。

用 douyin-viral-script。它的逻辑是「拆解同行爆款 → 提炼公式 → 复刻脚本」。原版依赖 Gemini 做视频分析，但很多环境拿不到 Gemini 的 Key。我们改了一版：把分析环节交给宿主模型自己完成（WorkBuddy、豆包工作自带的模型都能干），下载视频的脚本保留，拆解的活儿用提示词驱动。结果一样，但零外部模型依赖。

@纯小白 。

用 douyin-script。它先帮你从「兴趣 / 资源 / 变现目标」三个方向梳理定位，再去抖音搜一圈验证「这个定位有没有人看」，最后给你一套能直接拍的选题框架和口播脚本。你不用懂什么叫「钩子」，它帮你把前 3 秒怎么开口都写好了。

两套 skill 分工明确：一个负责「打对标」，一个负责「找自己」。

![两套 skill，各司其职｜高要求人群ouyin-viral-script](https://mmbiz.qpic.cn/sz_mmbiz_png/ZYIUeP9by5oUH1hOtKN8odkeavQKiakibxuQQmQRFz2VeCH3fUHlSJMz1lnOIb2IUJWyGBnOzfq1JYeDIYribBXqBgwb3rQljYccYkHia3ibdVLU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*两套 skill，各司其职｜高要求人群ouyin-viral-script*

图 1 · 两套 skill 分工对比（本文自绘）。

语音：把「你的声音」克隆一份。

文案有了，如果还要自己录，那就不算全自动。️ 这一步用 minimax-voice-clone 解决。

流程很简单：去 MiniMax 开放平台注册、完成实名认证、做一下最低充值（语音克隆约 9.9 元一次性，之后合成很便宜，约 1 万字 2 元），然后发一段 30 秒左右的录音。技能会帮你把音色复刻成一个 voice_id，存进环境变量。首次克隆完，后面只要给文案，它就用你的声音把字念出来——克隆只收一次费，复用不花钱。

小提醒：音频 7 天内至少用一次，否则部分套餐会清理音色，养成「写完就生成一段」的习惯就好。

数字人：照片 + 音频 = 开口说话的视频。

声音有了，最后一步是把「人」请出来。 用数字人平台的接口（如 DIT Studio），你只需要交三样东西：API Key、一张你的照片、一段音频（录音，或上一步克隆出来的 mp3）。

技能 digital-human-video 只做它该做的事：提交任务 → 轮询进度 → 下载视频，不碰语音合成、不写文案。按平台计费，口播数字人大约 0.06 元/秒（60 秒约 3.6 元，以平台实时为准）。建议新手第一次先生成 20–30 秒短片看效果，再拉长时间。

把前面三步接起来，链路就是：文案 → 语音 → 数字人 → 剪辑，四步各有一个专门的 skill 守着，WorkBuddy 在中间做总调度。

![口播数字人·四步流水线](https://mmbiz.qpic.cn/sz_mmbiz_png/ZYIUeP9by5rVicjz3pIjz5O8nvPBicKnicHeqFm9qDzvAB1oLRSKGfYOMaEvR0hxMxJwiblAvIciayBDW5TWDBA63O2yvichTCHwyiaY9PfkZSs8PA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*口播数字人·四步流水线*

图 2 · 口播数字人四步流水线（本文自绘）。

一个真实的小白一天。

这不是科幻，是现在就能跑通的工作流。

工具真正的价值，不是替你「想」，而是替你「做那些重复到让人放弃的活」。 镜头、录音、剪辑、对齐——这些消耗意志力的环节，交给流水线；你只管判断「这条内容值不值得做、怎么说更打动人」。

![你只管做判断｜交给流水线](https://mmbiz.qpic.cn/mmbiz_png/ZYIUeP9by5qRbz0y5WY5mnoibhuEECsCvYPibhTPB2ycOqQZ8TSCHcLw8c09zO8WIdE91etS2UKAZc7OkJlZOaZgSkMyhiaxO5ZgsCOWGYUns0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*你只管做判断｜交给流水线*

图 3 · 你只管做判断（本文自绘）。以上，就是我用 WorkBuddy 搭口播数字人的全部思路。流程跑顺了，剩下的，就是多拍多试。

行动建议 / 延伸阅读。

- 想拆同行爆款：装 douyin-viral-script，丢 1–5 个对标视频链接 + 产品信息，让它出脚本和分镜。
- 完全没头绪：装 douyin-script，先让它帮你定定位、出选题框架。
- 想用自己的声音：装 minimax-voice-clone，记得先完成 MiniMax 实名认证 + 最低充值，再发录音克隆音色。
- 要数字人出镜：装 digital-human-video，备好平台 API Key 和一张正脸照片，把音频交给它。
- 合规提醒：口播内容避免绝对化用语和未经证实的功效承诺；数字人形象请使用你本人授权素材。

- 唐舰长《用 WorkBuddy 打造口播数字人，文案-语音-数字人-剪辑全流程》（微信公众号「杰克船长的AIGC」，2026-09-21）——数字人平台计费与 MiniMax 克隆费用参考。
- DIT Studio 数字人平台说明（changer.qcapi.top）——口播数字人计费约 0.06 元/秒。
- MiniMax 开放平台「语音克隆 / T2A v2」接口文档（platform.minimax.io）——音色复刻与语音合成接口依据。
- 开源项目 alchaincyf/huashu-skills 中的 huashu-douyin-script——douyin-viral-script 去 Gemini 化改编的源头。
