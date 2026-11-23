---
title: "你的workbuddy该有个独立邮箱了，每天省下40分钟"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/647"
type: "tool"
chars: 2132
sections: 1
figures: 0
chapter: "08-我要接上现有系统"
---

# 你的workbuddy该有个独立邮箱了，每天省下40分钟
下午，我刷到一条关于QQ邮箱团队推出“Agent Mail”的消息。初看时没太在意，以为不过是又一款邮箱服务。但细读之下，发现事情并不简单——这个邮箱不是给人用的，而是给AI用的。更准确地说，是给AI Agent配备一个专属邮箱地址，让AI拥有独立的“数字身份”，可以自主收发邮件，且与你个人的QQ邮箱完全隔离。当时我脑子里冒出的第一个念头是：这玩意儿能绑定WorkBuddy吗。翻完文档，答案是可以。于是花了大约3分钟，把WorkBuddy和Agent Mail接上了。跑完几个场景后，我在笔记本上写下了一句话——「这可能是2026年最被低估的AI效率工具。」。

（workbuddy企业版，私信了解折扣）。

![腾讯刚出的Agent邮箱｜我花3分钟绑定了WorkBuddy邮件从此不用自己管](https://mmbiz.qpic.cn/mmbiz_png/ZfPRvecBtLS15NWU1hK1ALfnibI9nuXx59oXcy8L3wycGickfKFGVRSlBSqs4UCGh6ehn9BtAZiaPCGxbsNu03ADMptR8o7PFqHobdr8eKnZYg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*腾讯刚出的Agent邮箱｜我花3分钟绑定了WorkBuddy邮件从此不用自己管*

（一）为什么AI需要一个自己的邮箱。在聊Agent Mail之前，得先说说过去让AI处理邮件有多别扭。

我曾试过让WorkBuddy帮我打理邮件——方法很简单：用我的个人邮箱，把SMTP授权码交给它，让它能登录、能发信。但问题随之而来：它收到的每一封邮件、发出的每一封回复，全都混在我的个人邮箱里。想区分哪些是AI发的、哪些是我自己处理的，根本无从下手。更麻烦的是，WorkBuddy的权限和我完全一样，万一它误删了一封重要邮件，我连补救的机会都没有。如果你同时运行多个AI，每个AI共用一个邮箱，那更是一团乱麻——谁发了什么、谁收了什么，完全理不清。

Agent Mail恰恰解决了这三个痛点。一个AI一个邮箱，物理隔离。你的AI用一个，另一个AI用另一个，你个人的QQ邮箱纹丝不动。每一封邮件从哪儿来、到哪儿去，清清楚楚，可追溯、可审计。这个理念说来简单，但此前从未有人付诸实践。QQ邮箱团队是第一个把“给AI办个独立邮箱”这件事做出来的。

（二）3分钟绑定流程。我亲自走了一遍绑定流程，最快的路径是这样的。

## 第一步：装一个CLI工具。
打开WorkBuddy对话框，输入一句话：

WorkBuddy会自动读取文档，并在后台执行安装命令。整个过程完全自动，你只需旁观。关键在于，WorkBuddy的技能库里已经预置了agently-mail这个skill，文档读完，它便会自动装上。

![授权命令已启动，成功获取到授权链接。请点击或复制以下链接在浏览器中完成授权:](https://mmbiz.qpic.cn/mmbiz_png/ZfPRvecBtLQV7s8y44Yf12deZibVITLejplOR5mhuckQEUfHD77Nm8cAdJccsRvvHQUD9BCp3JtM3amHib5HZMib3lBOhT2V41Ria8Xdk9BPREY/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*授权命令已启动，成功获取到授权链接。请点击或复制以下链接在浏览器中完成授权:*

![](https://mmbiz.qpic.cn/mmbiz_png/ZfPRvecBtLRSGCcvPFV82uJdr6LdlXHDVVNU9qwCA6VkgZAtSEnEPVtMv7CyxzHPXK5hARg1GCoRJ8iaBogkactv7g9n2R6iaiaL1jXKR8qbd0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

第三步：验证 授权完成后，WorkBuddy会自动执行验证指令。一切顺利的话，它会返回你的Agent邮箱地址。看到这个地址，即表示绑定成功。

![](https://mmbiz.qpic.cn/mmbiz_png/ZfPRvecBtLS16BDU8xbMPkjWtJHT191ENfcCdUOI86qZyV2nqc3kHGujlNgDpEVlXrNKYwWaAl9vrianWSsRuBnibv64ddayTYU0icMuibJibibiaM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

（三）绑完之后能做什么。场景一：让AI自己收发邮件。

这是最直接的用法。你只需对WorkBuddy说一句话，比如“帮我给客户发一封邮件，告诉他方案已经做好了，附件在桌面文件夹里。”WorkBuddy会自动起草邮件、检查内容、确认收件人、发出。全程你只需一句话。

收件也一样。你说“看看我最近收到了哪些邮件”，它便自动拉取最近的邮件列表，按时间排序展示；你说“帮我整理最近一周的重要邮件”，它会自动分类、标注优先级、生成摘要。

对每天要处理几十封邮件的人来说，这意味着原本花在“筛选→阅读→分类→回复”链条上的时间，现在被压缩成一句话。

![USR: 帮我整理最近一周的重要邮件｜WorkBuddy正在拉取 Agent Mail 收件箱](https://mmbiz.qpic.cn/sz_mmbiz_png/ZfPRvecBtLR48ODRPPF7lByyDSJsNnG5wsbXdp15mzUPgrYMSzac7OsT1iaia5f8c66mTiboiaicfZzB78IZcoTME8wRY78Qt2j7rdbbO21J2ge4/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*USR: 帮我整理最近一周的重要邮件｜WorkBuddy正在拉取 Agent Mail 收件箱*

场景二：自动回复客户的常见问题。

你只需在WorkBuddy里设定规则：哪些类型的问题AI可以自行回复，哪些需要先经你过目。设定好后，每天打开邮箱，AI已经帮你处理掉一大半。

我试了一下，设置了一条简单规则：含“报价”和“合作”关键词的邮件，AI起草回复后等我确认再发；含“你好”“咨询”之类的一般问询，AI直接回复。两天下来，大约60%的邮件由AI直接处理，我每天省下近40分钟的邮件时间。

场景三：定时自动发送简报。

这个场景对自媒体创作者尤其实用。在WorkBuddy里设一条定时任务：每天早上9点，搜集昨天的行业热点，生成一份简报，通过Agent Mail发送到你的读者邮箱列表。WorkBuddy会自动执行：抓取资讯→整理内容→生成简报→通过Agent Mail发送。全程无需你动手。

以前你得手动写简报、手动复制粘贴邮箱地址、手动一封一封发。现在设定好后，它每天自动运行。

场景四：邮件内容的二次创作 这是我觉得最有意思的场景，对自媒体创作者价值很大。将Agent Mail收到的邮件作为内容来源，WorkBuddy自动分析邮件中的信息，提炼出可用的选题或素材。比如你做行业分析类自媒体，订阅了几个行业资讯邮件——以前你得自己看邮件、找选题、整理素材。现在Agent Mail收到邮件后，WorkBuddy自动读取内容，分析哪些信息有传播价值，生成选题建议和素材摘要，直接喂到你的内容生产流水线里。

当你的WorkBuddy拥有自己的邮箱后，它能做的事就不再仅仅是“帮你读邮件、帮你写邮件”。它变成了一个能独立处理邮件往来的AI员工——客户问报价，它回；合作方发来合同，它收；每天简报，它发。你剩下的唯一工作，就是看结果、做决策。

![群聊: workbuddy经验交流 2群｜该二维码7天内(7月14日前)有效，重新让公焱勇新鱼香龙虾](https://mmbiz.qpic.cn/mmbiz_png/ZfPRvecBtLQQ0zaKAexcHOFS9pXiaLYskpicRXVaJswXUJFYxsP5XHn4fSL60mgWrVuYGyPf9cg6VicmJicowROARCN4B9gWjey0HsOtASsicibrU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*群聊: workbuddy经验交流 2群｜该二维码7天内(7月14日前)有效，重新让公焱勇新鱼香龙虾*
