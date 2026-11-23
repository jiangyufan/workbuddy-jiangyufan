---
title: "花三小时，用WorkBuddy做了一个高三班级的成绩管理工作台"
source: "https://workbuddy.jiangyufan.com/index/hub/case/467"
type: "case"
chars: 2148
sections: 4
figures: 0
chapter: "11-我要搭个人工作台"
---

# 花三小时，用WorkBuddy做了一个高三班级的成绩管理工作台
HI，大家好，我是星光。

国庆假期和朋友们聚餐，其中一位朋友是高三班主任，广东人，推杯换盏间，又谈起想让我用Excel帮他做一份班级成绩管理表，导入考试成绩后，班主任和各科代课老师，可以直观的看到不同分数线的上线人数、临线人数、自身科目的成绩区间分布、退步学生名单，并据此设定谈话名单，动态更新谈话状态等等交互功能。

这事看起来简单，但涉及到交互功能，即看板和数据源相互读写，实现起来就复杂了。放在过去，我并不愿意做，关系再好，也不能拿自己所剩无几的头发开玩笑。但自从结识了WorkBuddy，又解锁了资料库加持下的工作台功能，我就有点儿悍勇无畏了，再加上酒意上头，触发了山东人的豪爽血脉，当场彪了一句粤语：湿湿碎啦，包喺我身上啦。

于是把这位朋友的需求发给WorkBuddy整理完善，又花了3个多小时，制作了如下样式的工作台。工作台案例网址：

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/JfCjVdhWmyVSKU9Ys9VqXKC7oVbliaz5S4Oj7enBHgEP70HNc7fSYYo5Z0pRUqmPYgejibvn5jBHmeQTKOH2Bxh7Xnu4J3BibxVYnN0WZ9EYw0/640?wx_fmt=gif&amp;from=appmsg#imgIndex=1)

## 1 - 控制面板。
这位朋友推崇极简主义，所以可有可无的图表和报表一律不使用，页面布局也尽量简洁，首先是由筛选控件组成的仪表盘控制面板，如下图红框所示，包含了科目、当前考试类型、对比考试类型、目标线、退步预警阈值和临界区间阈值等。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JfCjVdhWmyWKe0fiau8OJ6iboE7rf0xMked4U6qCXgHU9vapg9HojReklogwDPspaRKAcKV8ZcMNN0AvPcvMwHIGtAl2Cyv8esghSLRIXsAJs/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

控制面板的选项一旦切换，所有 KPI 卡片、图表、表格等信息都会跟着联动更新，甚至布局也会随之切换，例如，当选择全科时，单科成绩分布图会自动消失，反之，则显示。

![](https://mmbiz.qpic.cn/mmbiz_gif/JfCjVdhWmyUfZxMeqg7z4aIYyA8HHCysZic3u0pkhNrYIf2zsZzajI9sich8tTNrxbLJInLcONfNgujtxFwvicwJnNYia9U64dJEyVkkibDMEAXw/640?wx_fmt=gif&amp;from=appmsg#imgIndex=3)

筛选器【科目视角】包含了全科和6门单科，这是由于使用者包含了班主任和各科老师两类角色，班主任更关注全科成绩情况，而单科老师只负责自己的科目，与学生交流谈话时，也需要按角色分类记录。

## 2 - 操作入口与KPI指标卡片。
接下去是操作卡片和KPI指标卡片，如下图所示▼。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JfCjVdhWmyURMibL8ibpL63KIYibUvCN9gA9dZJWFK8J1x2N2aFUAObHxUmR2FPMWAxe7GoBo42TfibHxBXFPKNGicbPPSia8F5w21MzvKeib63CDs/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

1. 1 操作卡片

操作卡片包含了【导入成绩】、【记录谈话】、【询问AI】等。

【批量导入成绩】，用于成绩导入后端CSV数据库，可以选择考试类型与科目、支持文件直接拖动载入，并提供模版内容。

成绩导入数据库后，会自动对比上一次考试的成绩，将全科成绩退步>=20，或者，单科成绩退步>=10，自动标记为待谈话；其余则继承之前的状态值。

![批量导入成绩｜①考试(必须确认，不会跟随顶部筛选器)](https://mmbiz.qpic.cn/mmbiz_png/JfCjVdhWmyXHFw79e74WwT7PEz3raxlDzltH8BtAXLJNicSOUXUmaHiaIqWWbFjMKpKE8Cib7NwDlO5P97rVPpianFVz8lzJaqZOHN7jd1O7DJU/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*批量导入成绩｜①考试(必须确认，不会跟随顶部筛选器)*

【记录谈话】，用于记录与学生的谈话内容；可以根据学号和姓名模糊搜索学生，选择日期和科目等，并将下次跟进日期自动设置为一周之后。

![](https://mmbiz.qpic.cn/mmbiz_png/JfCjVdhWmyWu6637tIDLlnibaYoCMHUtFmam6PEEZh7uH7fgxKn5libxU82w6ic0UDic2csYpXicQRWqfkuF9346GbwRNvXY5FahqB3KtPibxiaRF0/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

【询问AI】，用于自动生成报告，可以选择报告类型（个人、班级、某次考试），不同类型会出现不同选项②和③和④。

![询问 AI·生成成绩报告｜①报告类型](https://mmbiz.qpic.cn/sz_mmbiz_gif/JfCjVdhWmyWmpgX6tFaWvjKu7lU6aGn5Z4gTVhe9HbL3CJKcDbL1UWicoYybMVbyPHh78sMHkBltoy5eGIr8oywCN6vyF3FkJicib5PR4hibAIc/640?wx_fmt=gif&amp;from=appmsg#imgIndex=7)

*询问 AI·生成成绩报告｜①报告类型*

1. 2 KPI卡片

KPI指标卡片有5个，其中「达线人数」受筛选器「科目视角」的影响，如果选择全科，则是达线人数，如果选择单科，则是不及格人数。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JfCjVdhWmyUoLbN673IHDClqeyL8ybQTedAjU8aEbjWichGRqtcjnKXxGz2Y3eKa0duiaphpySePyWjCKDAtJDf1EopxyicK2I9AnVUjN4u3PE/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

除了班级均分之外，其余4个卡片均内置了数据下钻弹层，展示对应的明细表格。例如，点击卡片「退步预警」，弹出如下界面。

![](https://mmbiz.qpic.cn/mmbiz_gif/JfCjVdhWmyXicUoVXE0UGJVNNvh6fbl8Nmn1hn5yfMEmP6wBict5mQSLS8bEb3doOG8f1XczeiaiclficCibgNH6GyxeXyibEAuTDSIPQEWZic4Qibcc/640?wx_fmt=gif&amp;from=appmsg#imgIndex=9)

该界面的表格（本工作台的任意表格）均支持点击标题进行排序；通过点击「跟进状态」列的值，可以快速修改状态，包含了待谈话/持续跟进/已完成等，且会直接修改资料库内的CSV数据库；在「操作」列，支持修改分数/设置谈话内容等，同样会同步修改数据库的内容。

最后，点击本工作台任意表格中的人名，均可打开如下数据下钻弹层，展示该学生历次考试成绩、趋势图、谈话记录等信息。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JfCjVdhWmyVjX3GrpkO6FXZ0aKWG0KibbPUjGXpHfJhHSBzWFVVFh3woNseicx2kt7e6WHGN4hOyH2Hicpm5tiaGBPFUgQTGUc6bCHo9bLoxnMQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

## 3 - 可视化图表。
接下去是数据可视化区，包含了三个图表。①总分分布图，它会与筛选器「考试类型」和「目标线」联动，将高于目标线的柱子，比如211/985/华五等，填充为一类颜色，低于目标线的填充为灰色。②单科分数分布图。③均分趋势图。鼠标悬停在这些图表的元素上，会显示相关数据——都是一眼能看懂的基础图，没有什么特别的。

![](https://mmbiz.qpic.cn/mmbiz_png/JfCjVdhWmyUfgoF0BWloAtJicOL1iatkicqESWiadFvVzxV0MerhkfyJKaaS4D0ictySoVB62ohWBMLCEaNGe5xIw0pmdBD0tI2ysrh2ZNClJ4Uk/640?wx_fmt=png&amp;from=appmsg#imgIndex=11)

## 4 - 表格区域。
最后是表格区域，提供了最常用的两份表格，退步预警名单和全班本次考试的成绩明细表，均支持点击标题排序、点击人名弹出个人明细弹层、跟进状态快捷操作、分数修改等功能。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JfCjVdhWmyUrzgowbkbZyMYrA2sTJkHqmY5PibZMpBic3D2xgp4ZhlGPBR7CCbWicjUibAWbBt57x2XTH7V0upS2NXBZ8pJPaf7QAia5w1RniaoHo/640?wx_fmt=png&amp;from=appmsg#imgIndex=12)

以上是前端HTML页面的功能说明，为了实现数据的存储与交互、不同操作人的权限，WorkBuddy在资料库又创建了9张CSV表格，包含6科成绩表、考试类型维度表、状态跟踪记录表等。

![学生成绩管理系统｜▶高三(3)班成绩管理工作台.html](https://mmbiz.qpic.cn/mmbiz_png/JfCjVdhWmyXu2kOn8D0uwtpX1Z289BjEWSkR5lDcNVJrrEt7y7yE0wW2G9NndTpS62AAGoKQGHCt8oUQ7uJdzovtu5ibbhfTljx4eiblibWiaI0/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

*学生成绩管理系统｜▶高三(3)班成绩管理工作台.html*

打个响指，是的，以上均由WorkBuddy自己执行完成。我开始是做一个大自然的搬运工，把朋友的需求转发给WorkBuddy；然后做狄仁杰，让WorkBuddy做元芳：“这件事元芳你怎么看。”；WorkBuddy发表它的看法，于是我最后化身张飞：“俺也是这么想的，就这么办。”，有时候也会提醒它：“你这个方案最可能导致的问题是什么。如何补救。”…

具体的制作及调试过程，参考知识星球教程「第18课：认识资料库（下）搭建个人工作台」。

话说自从有了WorkBuddy+HTML的超级组合利器，我怎么看Excel做的报表或看板都不顺眼 事实上，Excel自己也看自己不顺眼，于是推出了Excel文件直接转换为HTML网页的功能，比起Excel自身来，交互更方便，可惜国内用不了，希望是暂时，虽然希望不大。

盖木欧瓦，下期再见。

加入星球后，你的微信会收到一条平台推送的消息，里面有我的个人微信，务必加一下，之后邀请加入微信群，方便问题答疑和作业练习等。

![看见星光 送你一张星球优惠券｜新人立减券](https://mmbiz.qpic.cn/mmbiz_png/JfCjVdhWmyVCpNEs3BxjzNbID9JNF5auIaqBZqND3pnDF1x7NI9k9fqMGmykD8Qb4ia2J3mVJ5C84kja6XbqcDZYLk4UrEIrs2xWsfxsExmc/640?wx_fmt=png&amp;from=appmsg#imgIndex=15)

*看见星光 送你一张星球优惠券｜新人立减券*
