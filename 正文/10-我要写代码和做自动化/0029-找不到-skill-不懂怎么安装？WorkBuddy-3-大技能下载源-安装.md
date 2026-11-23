---
title: "找不到 skill 不懂怎么安装？WorkBuddy 3 大技能下载源 + 安装"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/745"
type: "skill"
chars: 2536
sections: 6
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 找不到 skill 不懂怎么安装？WorkBuddy 3 大技能下载源 + 安装
摘要：WorkBuddy找不到skill、不懂怎么安装。本文讲透3大技能下载源（技能市场/ClawHub中国镜像站/GitHub）和具体安装步骤，附常见问题排查，收藏防走丢。

![WorkBuddy上找不到 skill，不懂怎么安装，这一篇讲透。馆](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLV3kdpmFJIngZicibokexibkpfwEdCmsh7OhXdGIiaiaZOXYNVVHxEEE6ycWxdomCo7tP54U7ibn4z9eH0gg8icjb9WRD1LAuO9ORHSLI/640?wx_fmt=png&amp;watermark=1#imgIndex=0)

*WorkBuddy上找不到 skill，不懂怎么安装，这一篇讲透。馆*

WorkBuddy 的 skill 来源不止一处，很多人只盯着一个地方找，当然找不到。今天把 3 个来源和各自的装法一次讲清，建议先收藏。

## 一、先搞懂：skill 是啥，装哪。
说白了，skill 就是一份能力包。里面最关键的是一个 SKILL.md 文件，相当于说明书，外面可能还挂着脚本和参考资料。WorkBuddy 读到这个包，就知道遇到哪类任务该怎么做。

它装在两个地方，以 Windows 为例：

用户级：C:\Users\你的用户名\.workbuddy\skills\，装这里，你电脑上所有项目都能用。

项目级：你的项目文件夹\.workbuddy\skills\，只在这个项目里生效，适合团队共用一套。如果遇到技能不生效，重启一次 WorkBuddy就能看到了。

## 二、渠道一：技能市场（最省心，首选）。
腾讯自家的 skill，加上官方收录的，都在技能市场（BuiltinMarket）里。两种装法：

1. 对话框里一句话搞定 直接在对话框说"帮我安装 XX 技能"，WorkBuddy 会去推荐市场搜，找到就自动装好。不用管目录，不用解压，装完在「技能管理」面板里能看到，还能一键更新。

以安装腾讯ima技能为例，在对话框中输入“帮我安装腾讯ima技能”。

![连接器 自动化｜资料库·灵感](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLU5ib2EvIH71YzzRklUZ0zwI5NESkPVF6XlIHaR5CJIViaTH9RQsa1D8EmWsY9eiaEApw7frjmpQrTAkqE0TSaDmmjyKR5cmp19ibA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*连接器 自动化｜资料库·灵感*

显示已经安装完成，我们去「技能管理」面板看看是否安装成功。按照下图点击查看。

![连接器 搜索 搜索｜项目 项目](https://mmbiz.qpic.cn/sz_mmbiz_png/Iiczsyjb1aLVtaibC41ql9ZGTNHLXtmzzqk2bBk3Fbslg8sM1FAwIgw3ICj4OtKfqFpDuASlG5zu8sPjathiaD8U3As1hruGDX9QJMMSlicvzAI/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*连接器 搜索 搜索｜项目 项目*

![WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜+ 新建任务](https://mmbiz.qpic.cn/mmbiz_png/Iiczsyjb1aLULWo5XQ59HCWOibreokVP9157z4SotzGfhqHS6Ldzvp9KCSV6lleBt52C2TBOtdvqv23ialz2gIPv5XMibmibvYZslpQZBZbgIgu8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜+ 新建任务*

这是最省心的安装方式，因为WorkBuddy会自动解决一切。举个例子，你要安装一个skill，腾讯官方技能市场没有，怎么办。不用你操心，WorkBuddy会自动去其他技能市场搜索并下载好。

比如，我的公众号封面生成技能是baoyu-cover-image，这个技能在腾讯官方技能市场是没有的，当我给WorkBuddy下达下载baoyu-cover-image的指令后，WorkBuddy会优先到官方技能市场搜索，没有的话再去其他技能市场下载，看演示。

为了演示，我把之前装好的baoyu-cover-image删除了，然后给WorkBuddy下达了指令：帮我安装baoyu-cover-image技能。

WorkBuddy开始分析，腾讯官方技能市场BuiltinMarket没有这项技能，然后它去外部的skillhub和GitHub搜寻，最终从GitHub拉取而来。

![WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜专家·技能·连接器](https://mmbiz.qpic.cn/mmbiz_png/Iiczsyjb1aLXsibRRGSibcej3ib4BnB80MAQyfxRXPdo175gjs2HvfVSHd3tsB9Q6Xu8DbkvibicCKlKD7ZeVI8QTxUkUxuqPC9wXW1W6y47KHpNM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*WorkBuddy 编辑(E) 窗口(W) 帮助(H)｜专家·技能·连接器*

所以说，无论什么事，你只要能在WorkBuddy用普通的语言向他精准地下达指令，它就会尽力帮你解决好，而且越用越聪明。

1. 面板里手动安装。 打开「技能管理」面板，搜索需要下载的技能即可。按图中步骤操作。

![WorkBuddy 编辑(E 窗口(W) 帮助(H)｜SkillHub + 无信息图，分析内容，推荐布局 * 风格组合，并生成出版物。 5](https://mmbiz.qpic.cn/mmbiz_png/Iiczsyjb1aLWUaHPlZWszO4cC92Q18u1FWLgvByrSjtMaqlsnKVmFWc7hDNQTfNUaHOAD8QZIUH6RR2qE7ohdiaexE1DfDYNNMePbcaodZECk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*WorkBuddy 编辑(E 窗口(W) 帮助(H)｜SkillHub + 无信息图，分析内容，推荐布局 * 风格组合，并生成出版物。 5*

点击技能后，一般优先显示“推荐”的技能，这里的技能是腾讯官方整合的技能。优点就一个字：稳。官方维护、自动更新，安全有保障。如果“推荐”这里显示为0，说明腾讯官方没有这个技能，那就从外部的skillhub技能市场去下载。

## 三、渠道二：ClawHub 中国镜像站（社区好货，国内快）。
它是 ClawHub 社区高质量 skill 的国内镜像，访问速度比直连快很多。装法，手动最稳：进网站，搜你想要的技能。下载 zip 压缩包。解压，把整个文件夹丢进上面说的 skills 目录。重启 WorkBuddy。两点提醒：

1. 解压后目录别套娃，直接是「技能名/SKILL.md」，不要多包一层；放错文件夹等于没装。
2. 解压后把文件夹丢进skill目录中，有两个地方可以放。

C:\Users\你的用户名\.workbuddy\skills\。你的项目文件夹\.workbuddy\skills\。

## 四、渠道三：GitHub 下载（最灵活，开发者向）。
想要最新、最野的 skill，GitHub 上最多。找带 SKILL.md 的仓库，两种拿法：点 Code，Download ZIP，下完解压到 skills 目录。或者 git clone 到 skills 目录。或者GitHub上skill技能地址发给WorkBuddy,让WorkBuddy自动下载。

然后重启，完事。

下之前先看 README，有的 skill 要额外装依赖，比如 Python 包，有的对版本有要求，别闷头下完发现跑不起来。

## 五、三个渠道怎么选。
渠道。适合谁。难度。更新方式。例子。技能市场（含skillhub）。所有人，首选。最简单。一键更新。腾讯系技能。ClawHub 镜像站。想要社区好货。中等。重新下载。社区热门 skill。GitHub。开发者、追新。略高。重新 clone。

最新 / 小众 skill。

## 六、常见问题排查。
搜不到技能。大概率它不在推荐市场，去skillhub或镜像站或 GitHub 找。装完用不了。九成是没重启，或者文件夹套娃了，多包了一层。提示解压失败。把 skills 目录里那个临时文件清掉，重试。想更新。市场技能能一键更；手动装的，重新下载覆盖原文件夹。

三大来源讲完了。我的建议：日常用优先技能市场，找不到再去镜像站，再不行上 GitHub。收藏这篇，下次卡住直接翻。

下期我整理一份「我最常用的 10 个 skill 清单」，关注别错过。

能看到这里的，说明你对WorkBuddy是真感兴趣，想用WorkBuddy辅助自己做点事。那么我这个公众号或许对你有点用。

我的公众号在做什么。我一直在写WorkBuddy相关的教程，内容分三个方向：初级教程 — AI新手入门，基础操作一步步教。技能推荐 — 好用的Skills和AI工具推荐，看完就能用。实战应用 — 结合真实工作场景，教你用AI解决实际问题。

直接从合集点进去，按需翻阅。#WorkBuddy #AI办公 #Skill安装 #ClawHub #GitHub #技能市场。
