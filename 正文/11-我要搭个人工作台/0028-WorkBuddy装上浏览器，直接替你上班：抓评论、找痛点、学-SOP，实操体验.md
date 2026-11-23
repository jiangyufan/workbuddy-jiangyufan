---
title: "WorkBuddy装上浏览器，直接替你上班：抓评论、找痛点、学 SOP，实操体验"
source: "https://workbuddy.jiangyufan.com/index/hub/case/616"
type: "case"
chars: 2477
sections: 4
figures: 0
chapter: "11-我要搭个人工作台"
---

# WorkBuddy装上浏览器，直接替你上班：抓评论、找痛点、学 SOP，实操体验
毕竟现在桌面端的 AI 技能工具，无论是哪一款工具，基本上都是一个吞金兽，根本不够用。看似 deepseek 发布的模型价格特别低，但关我 hy3 什么关系，我免费。

![Hy3 模型限时免费｜延长至8月31日](https://mmbiz.qpic.cn/sz_mmbiz_png/k1k6dPQU2PsnZicEeQBs43B7kZ3Rs92CBEtJAKmco32j8SVh1DRibwI6M4VhMUazyibnESOiacntibDBGVK1UhkYZjPnfkZhhXuiaznbOv9F9qQGc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*Hy3 模型限时免费｜延长至8月31日*

之前我跟大家Codex怎么操控浏览器，今天换一个同样能打的——腾讯开源的 BrowserSkill。

电脑浏览器操控这个功能，很久之前就有对应的 skill；但这次不同的是这是腾讯自己开源的 BrowserSkill，一一句话怎么说呢：小作坊出品固然高质量、但大厂出品，稳定性最高。

它干的事一句话就能说清：

你给 WorkBuddy 装上这个技能，它就能直接操作你电脑上已经登录的浏览器，自己打开网页、点按钮、搜内容、抓数据，甚至把结果整理成 Excel 表格。

说实话咱们每天大量时间，都耗在浏览器里——登录后台、翻数据、复制粘贴、填表单。这些活不累，但特别烦。很多人可能就是冲着这一点才去用 Codex 的，门槛高的很，所以又只能花时间学习。

而现在，你居然告诉我三分钟就能配置完成，还免费用的 Workbuddy 也能替我把这些活干。

今天这篇文章，我把 BrowserSkill 是啥、能干啥、怎么装、我实测了哪些神仙场景，外加一份你可以直接抄的实操案例清单，一次讲透。

如果你也在用 WorkBuddy，或者正好被"每天重复的网页操作"折磨，这篇建议先收藏～。

## 01｜BrowserSkill 到底是啥。
别被"浏览器自动化"这几个字吓到，真不难理解。一句话：

BrowserSkill 是腾讯开源的一套浏览器自动化工具，装上之后，AI 能进入你已经登录的 Chrome 或 Edge，在一个单独的 Agent 窗口里替你操作网页。

它不是一个新开的、空白的浏览器，这是最关键的差别。

BrowserSkill 用的是你已经在用的、已经登录的浏览器。所以像小红书、公众号后台、淘宝、猎聘这种要账号的网站，它可以接着你的登录态直接干。

而且整个过程你都能看见：它打开了哪个页面、正在点什么、表格填到哪一项，浏览器上都会有"Agent 正在控制"的提示。碰到验证码、异常，或者你不想让它继续了，随时可以中断。

那它和别的浏览器工具比，强在哪。我列个表你们对比一下：

![](https://mmbiz.qpic.cn/sz_mmbiz_png/k1k6dPQU2PsQh02jUqE7am0FTGymsk1j9bVJiavY0uibZMcgFkqrg1E89MlALsEy8lBlP3XgmrsoYRmg0VR5ncxS8uQNf4eHPpEfT2gOnOESQ/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

看明白了吧。BrowserSkill 适合的是另一个场景：我不想重新登录，也不想把整个浏览器交出去，我只想让 AI 临时用一下我的登录状态，把眼前这件事干。

## 02｜怎么装。真正需要手动的只有一步。
安装比我想象中简单，而且大部分 Agent 能自己搞定。我一开始直接问 WorkBuddy：你知道 BrowserSkill 吗。网址在哪。发我看看。

![专家/技能/连接器｜资料库-宽感](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PsnNnaia5cg35rhZKsVIeOUEtvbz8GbJAm6NERrVliacph2ibZNILqiaDKpxyj5BkubOpd6FmicZPyjIHvzgrIKdtjdPwaXc5fh4nEk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*专家/技能/连接器｜资料库-宽感*

确实能看到是腾讯官方的 github 仓库，源码仓库、浏览器插件都具备。感兴趣的可以点进去看一下，当然我们想要用上就很简单了。

帮我直接安装一下，并告诉我怎么用。

然后 WorkBuddy 自动跑完了安装流程。真正需要我们手动处理的，只有安装 Chrome 扩展那一步。

![](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PuoujEcAsKzbftapFvPRCBqOiciau65Oichg9H2Sa4vwME9Jk97mkNXphUUln3oTwEobeFZS5WWcEoQ8whZt0CZ583gUBq0vIib0sM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

安装浏览器插件有几种情况：直接帮你打开本地浏览器，给你显示页面；另一种是给网址（给网址就把网址复制到浏览器中，打开也能显示界面。）。

在这之前，确保你电脑上有 edge 浏览器和谷歌浏览器，就是这两：

![](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PvFA5ibxO6ehkK4aZFiaAzfjpAb5tATJwm0pL4n43vwjNlzUsva2EiaJgTdjME9wGHDic7szb38lo6UcY6xy0Yz20AL0LO12vPQh6A/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

正常状态下，Workbuddy 会自动帮你打开浏览器，并显示出安装商店的窗口界面，你只需要点一下获取，或者点一下安装即可。

![单击“获取扩展”进行安装｜chrome 应用商店](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2Ps8sjzOfddVYjDYnp0c4R48US0xDfnSqic2zL2icyFvRo2gR7YFGgQqiaKdNVaYb4HKibR9Q17YmnDkmXl6MeOicxZbjtLjic4Z8IYkc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*单击“获取扩展”进行安装｜chrome 应用商店*

![扩展程序 工具 6,000 用户](https://mmbiz.qpic.cn/sz_mmbiz_png/k1k6dPQU2PslxNjVpM0tcia1uiadQ9MmgO729060wlFFC7gGnsVW1BIPofN3lbRxHWjgm7aDk1PEczmQVKuicJ8e0MUqOh48MEZsAVqDJzQuXE/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*扩展程序 工具 6,000 用户*

当你看到"已连接 / 运行正常"的提示，才是真的装好了。

![开发者模式](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PvCLtRL0hM0bBeTT6X7quDLttFElw6A6gkHCvRKoe6OMu488UarvcFsPHv4qMsR9n7Lq7xuZhpJFfq2MOPricTZ0qDO0s8pV12U/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*开发者模式*

以后要用的时候，在 WorkBuddy 对话框里选中 这个技能，再输入任务就行browser-skill。

![了解BrowserSkill及其网址｜专家、技能、连接器](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PvUXOdoLmxJCibV66FO47BmoenicznQicouEw7Lq44QzPiciaD6AcX6icEx5ZCicmWGv21Sv4m9vibtqqkFglzJspwOicCMRhWybRQkDe8M/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*了解BrowserSkill及其网址｜专家、技能、连接器*

说真的，别被"安装"两个字劝退，我自己第一次也就弄了 3 分钟。

## 03｜我实测的神仙场景。
光说能力没意思，我直接上三个我最想让你们抄走的场景。这几个都是"步骤明确、重复发生、结果能核对"的典型，最适合交给 AI。

我给 WorkBuddy 下了这条指令：

![了解BrowserSkill及其网址｜专家·技能·连接器](https://mmbiz.qpic.cn/sz_mmbiz_png/k1k6dPQU2PsAtnrGZKXVeNtEibeK3gdfIWPicLU0UlZibJJUoy50JMN96BiaUDK1UMcRhLLE6JsqPXickQWLlD9XLfV00rVhq9eL31Lqp7hfujpU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

*了解BrowserSkill及其网址｜专家·技能·连接器*

任务开始后，BrowserSkill 单独开了一个浏览器窗口，顶上提示"正在调试"，底部显示"Agent 正在控制"。

![WorkBuddy 教程 - 小环节搜索 × +](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PuaIOW7z31Kwfz81TPd9yiaJoCCG8Uag7tcuvtlhXvEEVMd5eEr6sTWAMChibzaa4Ny1fFOthoVe477CCJWsLY40ytOCic3DAZFA8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=10)

*WorkBuddy 教程 - 小环节搜索 × +*

它先搜索、再进不同笔记看数据和评论，最后把几百条评论里的"问题"归类成了痛点清单，甚至直接给我整理成了一份"用户痛点洞察报告"。

![☑ 一期视频带你高效玩转WorkBu.](https://mmbiz.qpic.cn/sz_mmbiz_png/k1k6dPQU2PtP3MZCohXfz2RXLzNiaKglusYruMz0m3g7nOQFjx5c22NVG442QFq37g3TmRoU05zHSyxzXYoGuOLnjZb8hQ4hLIGVEXibesfQc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=11)

*☑ 一期视频带你高效玩转WorkBu.*

这一步才是我觉得最有价值的地方：

如果只是帮我搜 5 篇笔记，它算个自动化工具；但它把几百条评论变成了"用户痛点"，又把"用户痛点"变成了"可以继续写的选题"——这条链路，已经进我的内容生产系统了。

![WorkBuddy用户头疼问题选题参考.md｜WorkBuddy 用户头疼问题 & 选题参考](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PtM7DFQiaBUcFTN4zDdJCia7MmhCglCusOEK9MsKIjkiadVVZ4j4ib7YpHSc12g3vGzh8TXmiawZOtVHTWt4eaYcVBS6lpxyCmgajNc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=12)

*WorkBuddy用户头疼问题选题参考.md｜WorkBuddy 用户头疼问题 & 选题参考*

![](https://mmbiz.qpic.cn/sz_mmbiz_png/k1k6dPQU2PuXw0eiavwB90nYiaWx3DPzb2ZFeuAfNekCKSPXibFH03XW9I09rP6xN41yOn4gDVuSMVu7bVnu3iaUReqYwxuoreGxnQEAkWOHhb8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=13)

你可以把这套提示词换成自己的行业：

做产品的人用它找需求，做电商的人找购买顾虑，做课程的人找学员卡点。同一套思路，换个行业就能用。场景二：商务拓客——去平台找合作对象。内容跑通以后，我又试了一件更接近商务的事：找合作。

人工去淘宝/抖音找 20 家店，要不停搜索、翻页、判断是不是旗舰店，再复制店铺、链接、价格、销量。头都大了。

我直接给了它这条指令：

打开我已登录的淘宝，帮我找卖【品类】的新品。要品牌旗舰店、销量不太高的产品，方便我去谈合作。整理成表格，字段要有：店铺名称、商品链接、价格、对应销量。先收集 20 家。

![了解BrowserSkill及其网址｜专家、技能、连接器](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PspYPICINoVsH5OV0ZsOfIEHxBex05GMeKAQAcjyafkZBVyewgnkPVZ6qA766RAvPkZa3SqQvWAqibtPDUq7MR3pMxYTyeeibvIs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=14)

*了解BrowserSkill及其网址｜专家、技能、连接器*

BrowserSkill 进淘宝后，按关键词搜索，再根据店铺类型和销量筛选，最后生成的 Excel 比我要求的字段还多。

![](https://mmbiz.qpic.cn/mmbiz_png/k1k6dPQU2PuqXRaevAMCXAzmGWYIjf7ZLbE93ZxMnz7jblDwMSthhAuDEuqOiaLXWbNAuWnYGQ5l1qibPfc6cic81S9XjpdRowh8nJoFlZVLPE/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=15)

这一套做下来，它完成了：搜索商品 → 判断店铺 → 筛选销量 → 提取数据 → 生成 Excel → 给出合作优先级。

原本最耗时间的前期筛选，它已经帮我做掉了。当然，最终要不要合作、品牌适不适合、联系方式真实不真实，还是得人工复核。

## 04｜进阶玩法：操作录制，你做一遍它学会你的工作流。
