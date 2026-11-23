---
title: "WorkBuddy无限算力实战指南2"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/670"
type: "tool"
chars: 2178
sections: 5
figures: 0
chapter: "09-我要省模型成本"
---

# WorkBuddy无限算力实战指南2
挂了的直接删，还能用的留下继续调，还自动加了几个模型。

1. 2 参数修正

接下来把参数修正过来。直接丢这句话：对我已配置的模型，修正一下这些模型的参数。

- maxInputTokens
- maxOutputTokens
- supportsToolCall
- supportsImages
- supportsReasoning

WorkBuddy 会自己跑去查官方文档，把参数补上。改完之后大概这样：模型。上下文。输出上限。图像。推理。LongCat-Flash-Lite。256k。4096。Minimax M2.5。196k。8192。supportsReasoning": true。

移动这条线我现在当 NVIDIA 的备胎在用。额度就 45000 次，看着不多，但救急够了。主力挂了的时候切过来，至少不至于对着屏幕发呆。

## 三、怎么选模型。
模型一多就容易犯选择困难症，每次提问前都要纠结半天"这次用谁"。我懒得自己想了，直接丢给 WorkBuddy 处理。

查看一下我配置的模型，给出他们各擅长什么。它会帮你整理出一张表。我自己是这么用的：场景。首选模型。原因。日常问答、快速响应。Nemotron Mini 4B。

1. 2 秒，轻量够用

长文档分析。Minimax M2.5 / Kimi K2.6。196k~256k 上下文。需要看图/分析图像。Kimi K2.6 / Qwen 3.6-35B。能读图。复杂推理、代码任务。Minimax M2.5 / Mistral Nemotron。

会推理。超长输出（写长文）。Kimi K2.6。32768 token 输出。额度充裕随便造。每天 5000 万 token。模型列表里按优先级排好，WorkBuddy 会自己从上到下试，前面的挂了自动切下一个，不用我管。

## 四、我现在的完整配置。
supportsReasoning": false。最后说两句。

说到底，token 焦虑就一个字：穷。要么额度太抠搜，要么参数没调好白白浪费。我的做法也就两点——先把手里这几条线的配置整明白，省着点花；再挖两条新的免费渠道进来，多条路多个 backup。

现在我的配置大概这么分工：NVIDIA 那条线平时当主力；龙猫额度多，随便折腾也不心疼；移动的拿来应急，关键时刻顶一下。三条线互相 backup，基本不会再出现那种"额度用完只能干瞪眼"的尴尬了。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/a0NvtlohtC8FTHdvcicIN361a7UONKN32DRPOicibERWj48zHy5YuuoMibxv3QhqApnSmv27mN37oyAZvrhrcD6Keb9mliaPDI6XyyOaO7mOnFmU/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1#imgIndex=9)

关注我，跟着我来实践。

## WorkBuddy无限算力实战指南2。
之前写过一篇《WorkBuddy 配置 NVIDIA 免费算力实战指南》，说实话那时候研究得不是很深，只是把 NVIDIA 的免费模型接进来，能用就行，继续优化后，理顺了，终于把token焦虑解决了。

## 一、先把手头这批模型整明白（以确定免费的NVIDIA为算力基础）。
之前配置模型的时候，参数基本都是瞎填的——maxInputTokens 填个 128000，maxOutputTokens 填个 4096，完事。反正能用就行。

但 WorkBuddy 会根据这些参数来决定怎么处理上下文、要不要截断、选哪个模型干活。参数填错了，轻的多花不少 token，重的直接把对话干崩。

1. 1 看看谁还能用，谁更好用

最简单的办法：直接问 WorkBuddy。测试一下我已配置的各个自定义模型的响应速度。查找一下更多模型。把有问题的模型配置去掉。配置地址：C:\User\admin\.workbuddy\models.json。

它会一个个测过去，告诉你谁还活着、谁挂了、谁快谁慢。我跑完的结果：Nemotron Mini 4B 最快（2.2 秒），然后是 Minimax M2.5 和 Mistral Nemotron（2.5 秒），Kimi K2.6 也差不多（2.6 秒），最慢的是 Llama 3.3 70B（5.2 秒）。

龙猫这几个型号里，我基本只接 Flash-Lite。原因很简单——每天 5000 万 token，这额度听着就踏实。日常问答、写点小脚本、改改代码什么的，用它完全够了。速度也还行，反正不卡。

1. 2 广东移动智算

这个是意外发现的。中国移动 App 里有个"我的卡券"，能领 30 天试用，45000 次 token 包。

![可使用(12)卡券历史｜【45000次】移动token 包优惠体验](https://mmbiz.qpic.cn/sz_mmbiz_png/a0NvtlohtC8niaMIvZz7wna8Wb9j1sRv2kPshibceps5icEqLzHIlkFMczSMwvdWK3qbHvnze2JJygsF2DRibHWbwmiaH6Jg9AoicF6A2sfsB5tg0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*可使用(12)卡券历史｜【45000次】移动token 包优惠体验*

选"标准版本"→立即办理。

订单信息页能看到 API Key和接入地址。目前只有两个模型能用：Minimax M2.5 和 Qwen 3.6-35B。

## 二、加两条"免费管线"。
NVIDIA网络一慢，我就有点慌了。手头不能只有这一条线，得赶紧找替补。前前后后试了五六个渠道，最后留下两条比较稳的。

1. 1 美团龙猫 LongCat

美团那边搞了个 LongCat 系列，最近把 API 放出来了，额度给得还算实在。

每个账号每天自动获得 500,000 Tokens 免费额度，可用于LongCat-Flash-Chat、LongCat-Flash-Thinking、LongCat-Flash-Thinking-2601、LongCat-Flash-Omni-2603 和 LongCat-Flash-Chat-2602-Exp。

每个账号每天自动获得 50,000,000 Tokens 免费额度，可用于LongCat-Flash-Lite 模型。

LongCat-2.0-Preview 初始额度5,000,000 Tokens/天，提交模型使用反馈，每次有效的反馈都将有机会获得额度刷新，每日最多可获得120,000,000 Tokens。
