---
title: "白嫖！手把手教你 WorkBuddy 接入商汤模型，免费 token 随便用"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/441"
type: "tool"
chars: 2622
sections: 6
figures: 0
chapter: "09-我要省模型成本"
---

# 白嫖！手把手教你 WorkBuddy 接入商汤模型，免费 token 随便用
点击提供商，下拉至最底端，选择自定义。

![+ 新建任务｜+ 添加模型](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLW1icrwBPWtQf6eNmdB0MgjZz87rjGF7E5ZUvN331VjGlVU79TEs0QFMy3Eext8pNicod0A1jJ5o93JjtP6COFo5xGlyN6jGXUc4/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*+ 新建任务｜+ 添加模型*

1. 3 添加第一个模型：sensenova-6.7-flash-lite（多模态）

点「自定义」，照着我的图片填参数，要一模一样，一个字母都不能错。

![仅支持 OpenAI 兼容协议 API｜帮助与反馈](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLV4Klb4HhDJbtLNqExI0OSXUBCq89raFNBWA4t2Ziaara9hN2yVK5UM0dMYJRm5cK7cOhk8KGxXumvMTVsTfnBIJXk6ZGIrr5wc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*仅支持 OpenAI 兼容协议 API｜帮助与反馈*

特别强调一下，模型名称填sensenova-6.7-flash-lite，必须一模一样，不能错，否则后续使用会报错。

1. 2 WorkBuddy 里找到自定义模型入口

打开 WorkBuddy，点击左下角头像，找到并点击「设置」→选择「模型」，「添加模型」。

![Buddy 加油站 1期·5/31 结束｜本期:专家团能量包 每日可领 150 通用积分](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLXW18SQzqW3Ys7OAY1qjI956HyJiaIuSVKpTQUvicXDNtKqK8RWKqS8LZUoWhyyXhmz5z04VgBWkceLjnib9Vyh2kQWFYp3MHqOJU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*Buddy 加油站 1期·5/31 结束｜本期:专家团能量包 每日可领 150 通用积分*

![WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜+ 新建任务](https://mmbiz.qpic.cn/mmbiz_png/Iiczsyjb1aLUMq6BXnQRKJV1bJOnmD1TibHBOHjpAOCwvlqAqZIb3wls4TxdoOXfNeP5bFPcnxNG7xkE41fWSaPrOkGeicupGYLTHX8iaZ7gyicU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜+ 新建任务*

## 三、接入 WorkBuddy，一步步来。
流程不复杂，但我会把每一步写清楚。

1. 1 注册商汤账号，拿到 API Key

先去 platform.sensenova.cn注册账号。注册流程跟其他平台差不多，填邮箱设密码就行。

![原生多模态智能体模型已发布｜Token Plan 同步开启 免费公测](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLWcS6iarcKjd7RmSupBsPqFMZcQdojANlKDGvnVmZpYia9rkRgdGo1qaGoQKwFZqHpwnKFtMsClqCAWibrPPt0IQT3ZZNS720IHC8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*原生多模态智能体模型已发布｜Token Plan 同步开启 免费公测*

登录后进控制台，找到 API Keys，创建一个新的API Key。公测期间注册就有免费额度，不需要绑银行卡或支付方式，直接开整。复制好那串 API Key，后面要用。

8日新SensenoV 模型 Model Plan 中 商汤官网 问题反馈 公测 FREE H API Keys API Keys 创建API Key(2/20) 开发文档 创建、注销API密钥，用于应用接入SenseNova。最多可创建 20个 Keys。Key仅在创建时完整显示一次，请妥善保存到环境变量或密钥管理服务。名称 KEY(掩码) 创建时间 状态 操作 画图 sk-C*.*.*+*.*+*+| 2026/5/16 22:53:36 可用 查看 注销 可用 查看 享馆 api'202605161355 sk-N*.*.*+*+| 2026/5/16 21:55:08 可用 查看 享馆。

## 白嫖。手把手教你 WorkBuddy 接入商汤模型，免费 token 随便用。

![积分消耗快。｜免费额度随便用。](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLWARwHXEMZSSft2juHSwibZcyUe8oQvqotnMLXJOy2PkpPlh2hR0rDAPgHBJXP522XEPIviarIPlHN48RPWwNpeCWCerx9CJVrr0/640?wx_fmt=png&amp;watermark=1#imgIndex=0)

*积分消耗快。｜免费额度随便用。*

## 一、我也有 token 焦虑了。
WorkBuddy 我是真离不开。

从做公众号、管理 WordPress 站群、到写知乎带货回答，每天都要跟它打交道。这玩意儿确实好用，就是 token 不够用。

之前 WorkBuddy 有个签到领积分，每天签到能攒不少。但后来签到下线了，积分断供了。虽然后面上线了「加油站」，每天送 150 积分，但对于重度用户来说，150 积分远远不够，一种莫名的焦虑感油然而生。

付费也不是付不起，但能省则省。AI 工具这么多，每个月这里交一点那里交一点，加起来不是小数目。正愁的时候，发现商汤 SenseNova 平台公测免费。

## 二、商汤三款模型公测免费。
商汤科技大家不陌生，国内 AI 第一梯队。他们最近发了 SenseNova U1 系列，新一代原生多模态大模型，把理解、推理和生成统一到了一个架构里。

公测期间开放了三款模型，全部免费：优势。推理速度。公测免费额度。SenseNova 6.7 Flash-Lite。多模态办公、高频调用、OCR / 图表解读。极快。每模型 1500次/5小时。DeepSeek V4 Flash。长文本、Agent 工具调用、编程。

快。每模型 150次/5小时。SenseNova U1 Fast。图文生成、信息图创作、文字精度。三款模型各有用处，全免费接进 WorkBuddy，日常够用了。

1. 4 添加第二个模型：DeepSeek V4 Flash（推理分析）

同样的入口，再点一次「添加自定义模型」。接口地址和 Key 跟上面一样，只有模型名不同：

![WorkBuddy 编辑(E 窗口(W) 帮助(H)｜提供商 ④ 自定义 / Custom](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLVmAxpxnx1RqwicQM95ZaSMfQgn8QPiaG8XBzEjHKArQgia8RWXa9lFrvr30QY3nd2KCmS8IMf2pGQabMpumeQZjFjUWTxiaicaGBsk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*WorkBuddy 编辑(E 窗口(W) 帮助(H)｜提供商 ④ 自定义 / Custom*

同一串 Key。deepseek-v4-flash。

注意，模型名称要跟表格里的一致，最好直接复制过去。高级配置只要勾选工具调用，输入128k或者256K，输出16K。

1. 5 添加第三个模型：sensenova-u1-fast（文生图）

这是一个文生图模型，和前两种聊天模型的接入方式有所不同。我是这样操作的。

API Key：和之前的一样。模型名称：sensenova-u1-fast。

把上面接口地址、API Key和模型名称一并发给WorkBuddy，告诉他帮我配置好这个模型，剩下的WorkBuddy会自己跑，并且还会自己测试画图。这个模型我有些话要说，后面开个单独板块讲讲。

1. 6 怎么切换用

这三个模型怎么选。写文章、日常办公，切到「sensenova-6.7-flash-lite」；做复杂分析、写代码，切到「deepseek-v4-flash」；要生成封面图，调用「。

![WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜+已连接:微信](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLXmYpZDyDpP7GdaVZO6H9CvPo5sJcScdrakfOOThQxvIUQah1Qx52uGiaJDc8tkasUaJwjEU1jC4BpdEVibA4Y2S1fQxwjiaTz9dg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜+已连接:微信*

有一点要留意，deepseek-v4-flash目前不支持图片输入。

## 四、重点说说 U1 Fast 文生图。
三款里我最想推荐的是 sensenova-u1-fast。它能直接生成图片，其他对话模型干不了这事。

之前我做公众号封面，一直用火山方舟的 doubao-seedream。效果确实不错，但火山方舟按量计费，生成一张图几毛钱，一个月下来也是一笔开销。

U1 Fast 也是文生图模型，API 兼容 OpenAI 格式，调用方式和火山方舟一模一样。我拿它和火山方舟做了个对比：

对比项。火山方舟 doubao-seedream。商汤 U1 Fast。费用。按量计费。免费（公测）。最大尺寸。1280×544（2.35:1）。3072×1376（2.23:1）。中文渲染。稳定。准确也较高。画风。手绘漫画。API 格式。

我自己试下来，U1 Fast 的手绘漫画风格跟火山方舟差距不大。而且公测期间免费，每模型 1500 次调用额度，个人用户完全够用。

不过中文渲染时，复杂字体偶尔会出现乱码的现象，整体不错。我试下来，prompt 里用英文描述画面主体，中文标题让模型直接渲染，效果还行。多调几次就能找到门路。

## 五、三款模型怎么搭着用。
总结一个使用指南：场景。推荐模型。理由。日常聊天、办公。轻量省钱，够用。写文章、写代码、做分析。能力强，理解到位。生成公众号封面、配图。免费文生图，替代火山方舟。

token 焦虑这事其实有解。商汤公测期间免费开放，我们先用着，用好了帮他们反馈反馈问题，两边都不亏。

花五分钟把上面步骤走一遍，三款模型接进 WorkBuddy，每天省下的 token 额度，够你多写好几篇文章。
