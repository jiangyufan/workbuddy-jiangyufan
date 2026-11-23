---
title: "WorkBuddy × 微信：构建属于自己的自动回复Agent"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/648"
type: "tool"
chars: 821
sections: 0
figures: 0
chapter: "08-我要接上现有系统"
---

# WorkBuddy × 微信：构建属于自己的自动回复Agent
腾讯的WorkBuddy，爆了。因为极其优秀的适配国内办公环境出圈，所以我也充满希望看看能不能实现我的一个日常小场景——自动回复微信好友消息。因为好多博文似乎都讲述了如何用微信去远程控制WorkBuddy为我们干活，但是很少说明自动回复消息这个场景，所以今天就试一下构建自己的自动回复Agent。

1. 简单安装

![AI专家团 全场景办公｜API·小白部署不输](https://mmbiz.qpic.cn/mmbiz_png/DVnh2ViaFsALI6vQAXATylnJ5NIUKs6zLxo55RRz2xMPtXNbDxGsiaW5yTfVpniayibpf07DiceiaWJ9ibpypuubspGff7M0Bj3plPr5mK7DdUDvek/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*AI专家团 全场景办公｜API·小白部署不输*

在登录后就能使用，左下角可以赠送100灵感积分，可以小领一下。可以够我们的测试。

1. 配置可以自动回复的技能

在WorkBuddy界面找到技能选项，选择搜索微信，找到对应的微信自动回复技能“微信QQ自动发消息”并下载安装。

![专家·技能·连接器｜项目新手指引](https://mmbiz.qpic.cn/sz_mmbiz_png/DVnh2ViaFsALxQXXyDW4KMTpWp1F0BcPKYc095cbchuNzjy7ffyrXkpBVsUmV296k2Uicx4GjY1Vz8tC7EiaMdIRgG8xoKtJrNFlSDKEL3BAgM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*专家·技能·连接器｜项目新手指引*

1. 一键对话设置设置自动回复

在安装好我们的技能，。

只需要用一句话对他说：使用微信qq自动回复技能，给我微信好友（备注的名称）发xx消息，他便可以对你所说的对象发你想要的信息。

使用微信qq自动回复技能，给我微信好友xx发消息:我是ai。注意在此期间，鼠标不要移动。

![哈哈哈测试了一下可以用](https://mmbiz.qpic.cn/sz_mmbiz_png/DVnh2ViaFsALIaoRCrjZeBXWQia3stSKg81CwmicScsUF24nCnKBZXnQAVTDLTsS6gdEWEA1eZ4QZWiaTO3ibYHFsoJ2k5IZIuctcrBujRibkmFds/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*哈哈哈测试了一下可以用*

为了让它能够帮我自动发送我文件夹里的内容，我还对他说：帮我发C:\Data\1.png,然后用一段话向我的朋友xxx介绍一下你。在WorkBuddy一通操作后，我朋友也顺利收到了消息。

![您的工作方式了吗?｜AIAgent 这个概念很火](https://mmbiz.qpic.cn/mmbiz_png/DVnh2ViaFsAJQiawt4uKxgbp2Gn3ffomsLzobtBXlia7hsBIK7DTA4luCKyVtxw1l4pGL7VZHVicMzvCHXOsGNiba3kEQSHGiato6yI3dthF4cWOQ/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*您的工作方式了吗?｜AIAgent 这个概念很火*

所以可以验证出它是可以发送我们电脑的文件。甚至还可以设置一个定时任务，让他定时向我们的微信好友发送，那它就可以帮我们去发一些固定在办公场景中需要发的通知，可以大量地节省我们每日的工作负担。

1. 写在最后

或许就是一个 Agent 互联办公的开始，我们可以用最简单的方式去感受它。我相信后面如果接入更多有意思的技能 skills，就能让它发挥出更强的能力。当然也可以喂给它专门的知识库，那它就是是个有内容的自动化回复Agent。

“Agent为我们解放更多时间，或许是为了走得更远”。
