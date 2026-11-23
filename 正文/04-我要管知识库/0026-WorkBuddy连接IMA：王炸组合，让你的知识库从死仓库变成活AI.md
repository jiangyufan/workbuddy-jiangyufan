---
title: "WorkBuddy连接IMA：王炸组合，让你的知识库从死仓库变成活AI"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/656"
type: "skill"
chars: 2632
sections: 11
figures: 0
chapter: "04-我要管知识库"
---

# WorkBuddy连接IMA：王炸组合，让你的知识库从死仓库变成活AI
你在微信里收藏了多少篇文章。大多数人早就数不清了。收藏夹999+，书签栏塞满了"以后再看"的链接。但有两件事最扎心：第一，你真正回头看过的，可能一只手数得过来。第二，就算你找到了，你还得从头读一遍才能回想起重点。这些"收藏"本质上就是一堆占着存储空间的字节。它们从来没有真正变成你的知识。

今天这篇文章，教你用两个免费工具，把你的收藏变成能帮你干活的AI大脑。

## 一、先搞清楚为什么是这两个东西。
WorkBuddy上一节内容已经介绍过了。WorkBuddy是腾讯出的AI Agent，一个能直接操作你电脑的AI助手。它不是那种只会聊天的AI。它能：读你的文件。写你的文件。帮你搜集信息。帮你整理资料。帮你跑自动化流程。打个比方：普通的AI是给你出主意的顾问，WorkBuddy是直接帮你干活的员工。

IMA：你的专属AI知识库。IMA也是腾讯出的，是一个AI知识库工具。你发给AI的问题，AI基于什么回答。有两种情况：没有知识库：AI基于自己训练时学到的通用知识回答。回答会比较泛，跟你想要的可能有偏差。有知识库：AI优先从你给它的资料里找答案。回答更精准、更符合你的实际需求。

IMA做的就是这个事——你给它喂资料，它帮你存着，以后你问什么它从你的资料里找答案。它俩连在一起，会发生什么。简单说：WorkBuddy负责干活，IMA负责存东西。WorkBuddy。IMA。角色。执行者（干活的）。存储者（记东西的）。做什么。

写文章、搜资料、跑流程。存储内容、提供检索。产出去哪。

- 一键存入IMA

← 从知识库调取。WorkBuddy写完的文章、做好的PPT、整理的资料，一键存入IMA。反过来，WorkBuddy干活的时候，也可以从IMA知识库里调取资料。它俩一配合，你的知识库就从一个"死仓库"，变成了一个能自己成长的"活系统"。

![WorkBuddy + IMA 协作示意图｜## 文档知识库](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrzujNMh1qibXFsx3MMss17LLQpYWrpTuAGKXuk3u2OuticxXpicNnPoDDXia9rCfu81icW0r0GW3FlcyZzHKgXsnxiaC8xd2YUju7bO4/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*WorkBuddy + IMA 协作示意图｜## 文档知识库*

## 二、3分钟配置教程。
配置其实非常简单，三步搞定。我带着你做一遍。

## 第一步：装技能。
打开WorkBuddy，在技能市场里搜索并安装这个技能：「腾讯ima」。

![ⅠmIOKX X+添加技能｜Excel 文件创建与分析](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrykYSEV70fTticLkdC8Q2ibjJM4HGEDsvkMHY48sT67LkZfFEbB0UnFXNcHic9pVMmuibq6TU7RH19J4ibYwhjBlwlWwEqoG9k2Q3YQ/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*ⅠmIOKX X+添加技能｜Excel 文件创建与分析*

再连接器中接入「ima知识库」。

![连接器管理｜连接外部服务，扩展 AI 能力](https://mmbiz.qpic.cn/sz_mmbiz_png/tYNTib1MTTrwgIwDpaZ9VOfonuHZ36QAyWLjtZgib8GS1ncSu3uf8ibiclpuAokAcg99ibgcRPyjHE8JeRo27BeFictmcfFaicX6ouyTFZSysWTmQM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*连接器管理｜连接外部服务，扩展 AI 能力*

## 第二步：获取API Key。
1. 用浏览器打开：https://ima.qq.com/agent-interface
2. 点击「获取API Key」
3. 弹出一个窗口，显示Client ID和API Key把这两个内容复制下来。

![▶第1步:复制提示词，发给小龙虾以部署ima skill｜请安装 ima 技能](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrxPyoKDr7Xz0icDuuibwc7nyqoSfxdflfWEe9fNOLgpicHnZRgIQrCbMDwofKo1ZUfBgIbjzA7NBYZQq36MERicsOJB18Bl6exxG34/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*▶第1步:复制提示词，发给小龙虾以部署ima skill｜请安装 ima 技能*

1. 配置凭证 回到WorkBuddy，在对话框输入：「配置IMA凭证，我的Client ID是XXXX，API Key是XXXX」 把"XXXX"换成你刚才复制的内容。

等它回复「凭证配置成功」，就说明搞定了。

## 第三步：测试一下。
输入：「我的IMA中有多少个知识库。」。如果它返回了你的知识库名称和笔记本列表，说明连接成功。如果报错，检查：微信账号和IMA账号是不是同一个。网络是不是正常。API是否配对正确。

![「我的IMA中有多少个知识库?」｜IMA知识库连接器已连接,我来帮你查询所有知识库。](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrxnUACQF77Y2IiavWicib5z6AWaB8Kp5zS1u82PwfibAibPA6PZgOvLt86YDAiaVONaSuOZUWicboTj0nfLDhB77RHmNmnLia2SvfRd2t0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*「我的IMA中有多少个知识库?」｜IMA知识库连接器已连接,我来帮你查询所有知识库。*

## 三、实战案例：把微信公号文章自动收进你的知识库。
配置好了，光能读不够。真正爽的是自动化。我教你一个最实用的场景：让AI每天自动帮你搜索公众号文章，自动存入知识库。你就不用每天刷公众号了，相关的文章AI帮你找，帮你存，你什么时候想看就去知识库里搜。

## 第一步：建一个知识库。
在IMA里建一个共享知识库，比如叫「AI最新资讯」或「自媒体干货」。

![+ 共享知识库｜超级AI之路](https://mmbiz.qpic.cn/sz_mmbiz_png/tYNTib1MTTrw2I8E3ZQH89yl3gh07QxiarRHDXwTEVAJctJcALqeLcxxF8ibVZYu0ctnBzXEle5xEOoiaxsVx8oydPiawGvujsDGqANQxE9duFLI/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*+ 共享知识库｜超级AI之路*

## 第二步：装一个搜索技能。
在WorkBuddy的技能商店里安装「wechat-article-search」技能。这个技能能搜索微信公众号文章，覆盖科技、AI、商业、职场等各种领域。

![赋予 WorkBuddy更强大的能力｜技能市场 已安装0](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrxYAh88mIkf2Oup9TfFfe0rHSA4yIl2F2iaZC0ibnUzyXiczUNceSk26A7iaSnLhs6LGp08EKqqH5kTaya33MTQfSVZRsnxibicqYcag/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*赋予 WorkBuddy更强大的能力｜技能市场 已安装0*

## 第三步：设置自动化任务。
在WorkBuddy里添加一个自动化任务，把「wechat-article-search」和「腾讯ima」两个技能都勾选上，然后写一句提示词，比如：

![+新建任务｜资料库·灵感](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrzwnXBCjiaSgd9dvfJk87rGBibBURrfZEyK3pLjTrxJcuffPeRe7Ziby6nV2j4PV8mZS5HrcygQwXTVPyfiaFFuZ9eplOq3L62uic4c/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*+新建任务｜资料库·灵感*

「每天搜索AI工具使用技巧相关的公众号文章，将搜索结果存入IMA知识库」。

![「每天搜索AI工具使用技巧相关的公众号文章，将搜索结果存入IMA知识库」。腾讯ima｜客户号·詹锅AI创富](https://mmbiz.qpic.cn/sz_mmbiz_png/tYNTib1MTTrxvWkzPHGE3TcFiaKJtuOUcWC4mfLMWYWJiahsiaRuvKceIsg831a3HlaH0mtFmRtZM6Wsiaszibuv20zoMWtphrUvPf4n77RiaYticJM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*「每天搜索AI工具使用技巧相关的公众号文章，将搜索结果存入IMA知识库」。腾讯ima｜客户号·詹锅AI创富*

![添加自动化｜] 搜索技能](https://mmbiz.qpic.cn/mmbiz_png/tYNTib1MTTrwb3suWqbrB2fllKCJrFekNlAsNhVEmHWnTPibYag09ZdnS0j2UQT26FaTvH1ic3ZiclabhzoR4ftqqkonlTVvasYib7QPXudw0VaU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

*添加自动化｜] 搜索技能*

保存之后，AI每天会自动帮你搜文章、存进知识库。你每天打开IMA，最新的相关内容已经静静地躺在那里等你看了。

## 四、这个组合还能干什么。
上面只是其中一个场景。实际上，WorkBuddy + IMA能做的事多了：场景。怎么用。写文章。WorkBuddy参考你的IMA知识库写初稿，写完一键存入IMA。做研究。把相关资料全导入IMA，让WorkBuddy帮你分析、总结、写报告。学课程。

把课程资料、直播逐字稿导入IMA，WorkBuddy随时帮你复习重点。做PPT。告诉WorkBuddy主题，它从IMA知识库调取内容，自动生成PPT。管理客户。把客户资料、沟通记录存进IMA，WorkBuddy帮你整理、写跟进方案。核心逻辑就一个：你只管往IMA里存，WorkBuddy帮你用。

## 五、常见问题。
WorkBuddy和IMA都要付费吗。WorkBuddy有免费额度，日常够用。IMA注册就送免费存储空间，基础功能不花钱。配置复杂吗。三步，三分钟。跟着上面的教程走就行。我只有手机能用吗。IMA有APP和小程序，但WorkBuddy主要在电脑上用。建议电脑端配置好，手机端用IMA查资料。

知识库里的内容会丢吗。

不会。IMA里的图片、文档存的是文件本身，不会失效。但公众号文章原文链接失效后，建议让AI转存为笔记备份。

写在最后。以前搭知识库是技术活，要配命令行、要写脚本。现在不用了。WorkBuddy干活的，IMA存东西的。你只需要说一句话，AI就帮你搞定。剩下的不是技术问题，是你愿不愿意开始往里存。别让收藏继续吃灰了。给你的知识一个能帮你干活的AI大脑。

一个建议动作：日常手机浏览到优质公众号文章，顺手就保存到ima知识库中。这就是微信生态牛的地方，在公众号的文章一键就可以存到ima知识库中，丝滑的不行。

我是詹锅，关注我，一起通往AI之路。

![用电脑打开 在浏览器中打开 ima打开 用豆包打开 用飞书打开 更多打开方式｜保存为图片](https://mmbiz.qpic.cn/sz_mmbiz_jpg/tYNTib1MTTrzMnRO4NkS9CeKQtKLDdIz6muGAo0h9LWsWbQgIaOrickWBotWLudFgpCC2u30hKicgaiaVv3so98yecBePRRWBeGL3lsRMyPlzj8/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=10)

*用电脑打开 在浏览器中打开 ima打开 用豆包打开 用飞书打开 更多打开方式｜保存为图片*
