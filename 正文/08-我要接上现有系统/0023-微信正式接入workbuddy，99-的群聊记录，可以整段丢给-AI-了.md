---
title: "微信正式接入workbuddy，99+ 的群聊记录，可以整段丢给 AI 了"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/434"
type: "tool"
chars: 1935
sections: 8
figures: 0
chapter: "08-我要接上现有系统"
---

# 微信正式接入workbuddy，99+ 的群聊记录，可以整段丢给 AI 了
大家好，我是星途，前大厂产品经理，一人公司实战派，专注于AI前沿科普。上周开始，微信电脑端的转发面板里多了一个选项。点开「转发到其他应用」，里面躺着 WorkBuddy 和元宝。

![最近聊天 创建聊天 转发到其他应用](https://mmbiz.qpic.cn/sz_mmbiz_png/pZKINIeAItBXhLnDAfyL4pIFJks81n8OwaR6AianjlrGFJ1dHUs6lBeV8H5c0cXnYyCPptFrUPibKfKJmibI3UuzBDuID7lEwsSpLp31RBeeOY/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*最近聊天 创建聊天 转发到其他应用*

## 版本对不上，后面全是白搭。
先说前提，卡在这一步的人最多。

微信电脑端要 4.1.13 以上。Windows 现在是 4.1.13.12，Mac 是 4.1.13。

WorkBuddy 要 5.5.0 以上，我这边跑的是 5.5.3。手机端暂时不支持，只能从电脑端发起。

## 第一步：框选，别一条条点。
打开目标群，鼠标左键按住任意一条消息往下拉，会拉出一个透明方框。比一条条打勾快得多。左下角还有个「选择到这里」，想一次性选到某一条就用它。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/pZKINIeAItD4gtgiboJL7gsicCqmh1iaRicEXB12w80SicYwialAictUqWyJspVhakq3vCIzSL7vYUaRibgEJk9u68gRictn1ZjMOCkzQffvOWzlONwg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

## 第二步：合并转发，切到最右边那个标签。

![转发到其他应用](https://mmbiz.qpic.cn/mmbiz_png/pZKINIeAItAcuSagHjZgOLe5Tcia7DG0nsQCOic3ZKrrnLkG5e77UMkQ7G8jTH9SGJNHcmrDfuJT8ibUJYakkK4jkoicshDzkc8qTficMyuxPXeI/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*转发到其他应用*

## 第三步：弹窗点确定，然后别急着发送。
点完会弹一次「即将离开微信，打开 WorkBuddy」，确定。WorkBuddy 被唤起，对话框里多出一个压缩包，重点来了：它不会自动发送。你可以在输入框补一句你要它干什么，再点发送。很多人直接回车，等于让它自己看着办，出来的东西就很随机。

![致敬好老师，送你 Buddy 好搭档，认证老师尊享积分好礼｜@代码开发](https://mmbiz.qpic.cn/mmbiz_png/pZKINIeAItCkmpZ1O9atkFZrrFibMrhncMa9VOBIYzE4adP66mN4YHH8FuuZYIcw8Tiac8DDRMkS4L5WrCAdtWLU2X68gk3t7v3dWNiaYqMIFc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*致敬好老师，送你 Buddy 好搭档，认证老师尊享积分好礼｜@代码开发*

## 四条边界限制。
这次踩了几个坑，总结一些心得和能力限制。一次最多 100 条。这是微信侧转发本身的上限，跟 WorkBuddy 没关系。群消息多的，建议分几批转过去，最后再一次性下指令让它统一处理。一次最多 9 个会话。想一次导入多个群或者多个联系人的记录，会撞上这个限制。

图片能读，视频基本没戏。图片它读得懂，做群日报的时候甚至能把图配回输出里。视频是靠抽帧读的，HEVC 编码大概率抽帧失败。语音、公众号链接、小程序、名片，现在都转不过去。是你推给它，不是它去拿。WorkBuddy 不会主动读你的微信，每次都是你手动选、手动发。

这条决定了隐私边界：你勾选了什么，AI 才知道什么，它自己拿不到别的。这里，我让他帮我做了一个可视化的报告，也非常清晰可观。

## 这几句指令可以直接抄。
出纪要：把这段群聊整理成会议纪要，标出决议事项和待办，待办写清责任人。

提需求：从这段聊天记录提取所有需求，按「需求—提出人—日期—紧急度」整理成表格，还没定论的单独列一栏。

做统计：统计这段聊天，消息总量、发言人数、活跃度前 5 位、主要话题分布，输出成一份日报。挖遗漏：从这段记录里找出所有被提到但没有被回答的问题。再往上一步，加一句「保存到」。比如「把今天所有客户需求提取出来，分类保存到 /客户管理/需求库/ 文件夹」。

加了这句，聊天记录就从一次性消耗品，变成了能攒起来的资产。

判断一段对话值不值得转，我给自己定了三条：信息密度高不高、手动整理会不会超过 30 分钟、能不能文件化。

占两条，就值得转。

说实话，这个功能本身技术含量不高，难的是微信肯开这个口子。我一直没想明白：微信自己做一个能进群的机器人，到底有多难。技术上我觉得一点都不难，国外早有同类产品了。卡点应该在隐私和合规——群聊是多人数据，你一个人点了转发，其他人的消息算谁的。所以现在这个形态是个妥协：微信不出面，让 WorkBuddy 接，数据全程在腾讯自家院子里转。

它跟真正的微信 Agent 是两回事。真正的 Agent 是常驻的、自动的、会主动提醒你；现在这个是手动的、一次性的、你不推它就不动。但话又说回来，能用上就先用着。爬楼两小时变几十秒，这笔账怎么算都划算。至于小微以后会不会真的进群，我赌它会，但不会太快。

我是星途，感谢您的阅读。

WorkBuddy 被唤起，对话框里多出一个压缩包，名字类似「聊天记录_20260907_094206.zip」。

重点来了：它不会自动发送。

## 四条边界，网上说法挺乱。
这块我专门对了好几个来源，加上自己试的，结论如下。群消息多的，分几批转过去，最后再一次性下指令让它统一处理。顺带说一句，有博主说视频号链接能提取口播文案，我这边没复现出来，这块存疑，别当定论。这里我让他帮我做了一条可视化的分析报告，大概长这样也是非常清晰明了的。

![群聊记录报告-财税风控智能体知识库踩坑.html｜《财税一体化风控智能体》本地搭建踩坑复盘](https://mmbiz.qpic.cn/sz_mmbiz_png/pZKINIeAItAEf549XZwznABEw5FUxuTDhVJP16kgeYHJlbJouGDlGFzpgef1g1rPSnQ5lnbGQnm3cxick5coicBpzsKaQcUGKghPfQJw5vx14/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*群聊记录报告-财税风控智能体知识库踩坑.html｜《财税一体化风控智能体》本地搭建踩坑复盘*

所以真正值钱的不是「能转发」，是你下指令的颗粒度。加了这句，聊天记录就从一次性消耗品，变成了能攒起来的资产了。判断一段对话值不值得转，我给自己定了三条：信息密度高不高、手动整理会不会超过10分钟、能不能文件化。我一直没想明白：微信明明作为一个流量最大，也最容易做出国民级应用的平台，为什么把自己封闭得那么死。

要实现技术上的对接，其实一点都不难，国外早有同类产品可以参考。但话又说回来，能用上就先用着。毕竟也是一个好消息。

![](https://mmbiz.qpic.cn/mmbiz_png/2aXcqmnP9tGnyyMv5iarRJoOWjYhI3F8lADwT7cZky0wQ02DXMzTywFlqt4pUEaEvFAofxYVY2Pyu1C4xh9a17w/640?wxfrom=5&amp;wx_lazy=1&amp;wx_fmt=other&amp;tp=webp#imgIndex=19)
