---
title: "WorkBuddy又解锁一个王炸Skill，直接操作你已登录的浏览器！自己上网干"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/384"
type: "skill"
chars: 2451
sections: 5
figures: 0
chapter: "10-我要写代码和做自动化"
---

# WorkBuddy又解锁一个王炸Skill，直接操作你已登录的浏览器！自己上网干
最近我一直在深度使用 WorkBuddy，也写了不少相关的实测文章。

就在前两天，我又发现了一个挺有意思的东西，腾讯开源了一款叫 BrowserSkill的浏览器自动化 Skill。

它能干啥呢。

就是你装上它以后，WorkBuddy就可以操作你电脑上已经登录的浏览器，帮你打开网页、点击按钮、搜索内容、抓取数据，甚至把最后的结果整理成 Excel表格。

它是真的会打开浏览器，替你一步一步把事情干完，。我测试了几个案例，真的有点被震撼到了。我只是在WorkBuddy里输入了一句话：

![BrowserSkill"已开始调试此浏览器取消｜图文 视频 用户](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0TOx3UD6DHw94Z0A751uZ6DsF7zPs5iaTtTzCul2BEbox9sXFcCEaqibBnLUjFXAJibCZoG6x1uBpvBBl9iaz87kAYba9oQvH7Nw0Y/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*BrowserSkill"已开始调试此浏览器取消｜图文 视频 用户*

我特意录制了一个视频，大家可以感受一下，全程没剪辑。9分20秒后，它给我抓回了772条评论，给我生成了一份完整的“WorkBuddy用户痛点洞察报告”。

![](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0Rmy16wY0oOKj82ibBLvTH6JMV1Nyc58bow2XbSE5S9dQLReZ6VFCiaAafQsRJF1wNaWQ9vfcxPYgzXfyEvfdGPgf4V1Eiaq4zMcE/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

而且这还没完，我又让它打开淘宝，筛选20家正在卖洗面奶新品、销量还不高的品牌旗舰店，最后给我整理成了一份Excel合作名单。

![公式 数据 审阅](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0QGmQrCVfZlIcy9S1F53Gics8DHM6r1m7271IeLibNJbBCGSfHfCtSEPmLeMvibpSna5RhACTUZXyXEy4NY4h4soOPNaWKCjYQftY/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*公式 数据 审阅*

![几个必须跟你说清楚的点(不然数据会误读)｜过程中的两个意外发现(已记进项目记忆，下次直接复用)](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0SPNNK2ub0FQaJvibC5AS1vXY8GGVKJpwibzoYdAyIdOoJAko61LIq4put1LfkCnKslZnnXp9gsUiae4T9PKKwMBMGgGAUlMoLGic8/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*几个必须跟你说清楚的点(不然数据会误读)｜过程中的两个意外发现(已记进项目记忆，下次直接复用)*

如果你也在用WorkBuddy、Codex、Claude Code或者Cursor，想实现浏览器自动化，这篇建议先收藏。

## 一、AI会操作网页不稀奇，难的是进入你已经登录的网页。
BrowserSkill就完美解决了这个问题。它是腾讯开源的一套浏览器自动化工具，由一个本地CLI、后台服务和浏览器扩展组成。但是这些技术名词不用记。你只需要理解一句话：它可以让AI进入你已经登录的Chrome或Edge，在一个单独的Agent窗口里替你操作网页。

Agent不会默认乱动你正在使用的普通窗口，你正常做其他事情就行。遇到验证码、登录确认或者需要你判断的步骤，它还可以暂停，把控制权交还给你，处理完再继续。

## 二、市面上这么多浏览器工具，BrowserSkill有什么不同。
看到这里，懂一点技术的朋友可能会问，Playwright、agent-browser、browser-use这些工具，不是早就能操作浏览器了吗。

确实，这些工具虽然都会点网页，但解决的并不是同一个问题。我列了个表你们对比一下就知道了。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0Tmk5Er0raEiabdwXpvIsdY1ian0CgBia9GUicDQyIWFCCPm2h9Ig4w74QMR2B3FZ2cY0ro3R4GRqdwotueaNmWpTxHVt9q4ibZiaLfA/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

BrowserSkill更适合另一个场景，就是我不想重新登录，也不想把整个浏览器交出去，我只想让Agent临时使用我的登录状态，帮我把眼前这件事做。

## 三、具体怎么安装。真正需要手动的只有一步。
安装过程比我想象中简单，大家直接跟着我的步骤去操作就可以。我一开始直接问WorkBuddy：

你知道BrowserSkill吗。这是腾讯开源的一款浏览器自动化Skill。你帮我查一下，告诉我能不能安装、怎么安装。

![查清楚了，结论先给你:｜能装，而且官方把WorkBuddy列为支持对象](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0QfICSgo6I4pwibqf597SA0IRbMvEk0ESibmW5WOGqXD7Lic8vadLojgUKG3zFaJrd1ZKhVyPKkdqUuE1V8ZLmyQxtSt8HDbsMFjE/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*查清楚了，结论先给你:｜能装，而且官方把WorkBuddy列为支持对象*

它确认支持之后，我又说了一句：帮我直接安装一下。

然后WorkBuddy自动完成了安装的事情，并且大部分安装工作，Agent都可以自己完成，真正需要我们手动处理的，是安装Chrome扩展。

WorkBuddy会给出Chrome应用商店的地址。

![帮我直接安装一下｜装好了。给你交个底:](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0SUlLsjhlV9jUjWy1nFg6NiaB5zOYab7nBMmOH9iaj2WbZCRhpzic3u1hqzY0UfJphTqpM2pGVSLYh0Muiaiaq3UFvkm5nqPrtfm874/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*帮我直接安装一下｜装好了。给你交个底:*

打开后，点击右上角的“添加至Chrome”。

![chrome 应用商店｜扩展程序 主题](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0SDkjIIeg7mKBAkh8WqHuIy9IfbdTDBPjtUCmrQ1ibOK4JfXG2HlWQSjLnKTeTBILicACAzQ4uRVBGVibFsBR3ACict6tBJYDs3tMY/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*chrome 应用商店｜扩展程序 主题*

浏览器会弹出权限确认窗口。

![扩展程序 工具 5,000 用户｜要添加"BrowserSkill"吗?](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0SuvjshJTyCwL0ZXvjNuk681one6BviaObRt5IgkqyyqETjukKRfDUXibtBVy5VFFtMdV3ibWY1NoPOEBiarro6DqmBjEyvLz3cwhk/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*扩展程序 工具 5,000 用户｜要添加"BrowserSkill"吗?*

安装扩展以后，我回到WorkBuddy，让它检查是否可以正常运行。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0TJk18KLD9C2Dg5HVbSKzbO6hYkUkhZzUoJnicky6Pia2XbEv9nnda4euuzLyj1lRVpbTtwiaN609jyz7QqdWankBuf5KapN3EdqY/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

到了上面这个画面才是真正的安装成功。

以后需要调用时，点击WorkBuddy对话框左下角的技能入口，找到 browser-skill，选中以后再输入任务。

![WorkBuddy你的职场超能十｜Apple 风格 UI 生成——简洁、精致、高...](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0R6R9UKvqvXDfRbOzdCXQBqSpRleibBxHzwGCyxLhs0wlQH6EDvNdgguIhx7SVESqTXDxa8EjRvzdZiaaAY8QwQLGet6DEV1vtZM/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*WorkBuddy你的职场超能十｜Apple 风格 UI 生成——简洁、精致、高...*

## 四、第一个实测：从772条小红书评论里挖用户痛点。
我想了解现在用户关于WorkBuddy还有哪些比较头疼的问题，方便我后续在写WorkBuddy选题文章的时候，能够更抓住用户的痛点。

![WorkBuddy你的职场超能力｜数据分析及可视化](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0T9JbjLsRanxAsicvBeNwKjImfjPw7CHCT4lbZEsPIVXdgntsyZaoGgcIypg5X2LQ5CtykhBzOPzj1p9icJLAibnk0Y8RKia9tudyo/640?wx_fmt=png&amp;from=appmsg#imgIndex=11)

*WorkBuddy你的职场超能力｜数据分析及可视化*

任务开始后，BrowserSkill单独打开了一个浏览器窗口。浏览器顶部会提示它已经开始调试，页面底部也会显示“Agent正在控制”，随时可以中断。

![BrowserSkill"已开始调试此浏览器取消｜图文 视频 用户](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0Qb2axRib2DSK8SGZLCibebL7kU95unJfGOHTlB11D0y7Ojhgd6pTtWZHhj7c1byuuicdDSibEHWNGCE4SFe51o9EbA9bq7dFtPw0U/640?wx_fmt=png&amp;from=appmsg#imgIndex=12)

*BrowserSkill"已开始调试此浏览器取消｜图文 视频 用户*

它先搜索WorkBuddy，再进入不同笔记查看数据和评论。最后一共运行了9分20秒。

![](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0QWPQvaftOB9pDswjOuj2BWOoicxVG4zOv5k83oMeDDmR4hWicsq6fVib98s63ZzTtCcHns3QcOTSypnzczDMqticJGmqPkibKmqJEc/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

这一步已经挺强了，但真正让我觉得牛逼的，是它继续把这些评论里的问题进行了归类。

![抓取小红书Workbuddy高赞评论痛点｜报告里有完整的原声引用和8个选题的优先级排序，原始JSON也存了，想按别的维度重新切随时说。](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0SPKfvlJT3YUQnakZUOZtQu5l2OEVoYssD3V2g6O8ypegibxjU5ym6eX55DFBprs6vrrJYUhPwhuvMvI56sqlaQibKkE9grZegaI/640?wx_fmt=png&amp;from=appmsg#imgIndex=14)

*抓取小红书Workbuddy高赞评论痛点｜报告里有完整的原声引用和8个选题的优先级排序，原始JSON也存了，想按别的维度重新切随时说。*

![](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0SElKZEFIicYK8XLAFprWlicqFh574CKtt2Z18hvKkJHfyfGicG4a6hF1vvSomJZwCCu4eaibLQoN3j1a2ibU7uO960gvccEYK0NFs4/640?wx_fmt=png&amp;from=appmsg#imgIndex=15)

这一步才是我真正觉得它有价值的地方。

如果只是帮我搜索5篇笔记，它最多算一个自动化工具，但它把772条评论变成了用户痛点，再把用户痛点变成了可以继续写的选题。

这条链路已经开始进入我的内容生产系统了。你也可以把这套提示词替换成自己的行业：

这套方法不只能找选题。做产品的人可以用它找需求，做电商的人可以找购买顾虑，做课程的人可以找学员卡点。

## 五、我又让它去淘宝找合作对象。
小红书跑通以后，我又想测试一件更接近商务的事情。

我有个朋友的公司业务，就是专门去找淘宝的一些新商家合作，需要去拓客，我就想这个事情能不能让Workbuddy去完成。

如果人工去淘宝找20家店，要不停搜索、翻页、判断是不是旗舰店，再复制店铺、商品链接、价格和销量。头都大了。所以我直接给了它这条指令：打开我已登录的淘宝官网，帮我找一些卖洗面奶的新品。要找品牌旗舰店，并且销量不太高的产品，方便我去找这些新品进行合作。

把这些数据做成一个表格，表格里面要有：店铺名称。商品链接。商品价格。对应销量。先帮我收集20家。

![](https://mmbiz.qpic.cn/mmbiz_png/99PzpXG5e0SMFAbzY1KYApPOcoMxWZfc3nhJLDV0UrdynFIJFV1g9MSjJCalupT6siaZTYQjqYJNsznL5aqqnq8gDEytbcqxPXqDInNgsGtA/640?wx_fmt=png&amp;from=appmsg#imgIndex=16)

BrowserSkill进入淘宝以后，搜索洗面奶，再根据新品、店铺类型和销量进行筛选。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/99PzpXG5e0RaJAPniaqoaDOt5tCWKpSR9RIhVIQsB4ibjibMcu9EtuQcJIA48vibh8XqNfXoxx6QMbaB4DE2yceHFsLlvsIalzrOSmoHDuFl0O8/640?wx_fmt=png&amp;from=appmsg#imgIndex=17)

最后生成的Excel，比我要求的字段还多，最终给了我一个excel表格。
