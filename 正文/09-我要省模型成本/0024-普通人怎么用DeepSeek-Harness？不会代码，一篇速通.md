---
title: "普通人怎么用DeepSeek Harness？不会代码，一篇速通"
source: "https://workbuddy.jiangyufan.com/index/hub/case/551"
type: "case"
chars: 2435
sections: 5
figures: 0
chapter: "09-我要省模型成本"
---

# 普通人怎么用DeepSeek Harness？不会代码，一篇速通
![普通人能拿它做什么?](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4YzYRANZNyu4mtNzu7Ze4wM1hSmribrjrvs8jHTml4of8ibeMK1PzV28QNHDxibia7NqiaM3O8N656Te7kZpK71CI4RDpUF3H5vWw3c/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*普通人能拿它做什么?*

这两天，梁圣在互联网上挺火的，DeepSeek 接连发布 DeepSeek V4 PRO 正式版模型和开源工具 DeepSeek Harness。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/XjrGzTnbp4ZGbGmNcTibEsh0XKGgicnpB1oNwnmjhFqmn2P9icN0AbOUuoC1HoiaicoweTGNoiaR7byuiaCHLsctiarufo0GuQlzBadlJhp5H2geC6g/640?wx_fmt=gif&amp;from=appmsg#imgIndex=1)

DeepSeek V4 的API当前已更新到V4-Pro-0813。它支持百万上下文、工具调用和Responses API。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4ZKIkfyJO6cGBmfx5R5yUibzVhmnGwtTcDBsBf4Bhep6Wh2eicbF1CBuKfXvCjGTRaICxoPs8LPiaObfWZtAl85Y2mj627G9nuqiaU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

大语言模型大家已经不陌生，DeepSeek Harness 又是个啥。名字有点技术，官方介绍里又是插件、沙箱、调度和循环，很容易让人以为这是程序员才会碰的东西。但其实人人都可以上手使用。

![公告10.4k forks*西羊石AI短剧](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4bP6mXxIicdE0fr8h6Zs4x6Iz0JSFgnVK3VJDfCWSeK1QFCXw9duTet3wyLxHlKxNqjtt3Rz5JOrSLsMniaFYyOWAqbRSI2w3NWo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*公告10.4k forks*西羊石AI短剧*

下面我来给大家简单普及它是什么东西，同时快速教大家如何利用它实现工作提效。

## DeepSeek Harness到底是什么。
可以先把大模型想成一位很会做菜的主厨。它能理解需求、判断做法，也知道下一步该干什么。

但如果只把它放在聊天框里，就像让主厨隔着玻璃给你讲菜谱：冰箱在哪、刀具怎么用、订单先做哪一桌，它都碰不到。

Harness更像是主厨身后的整套后厨。

文件是食材，终端和各种工具是设备，计划与调度负责安排先后顺序，沙箱和权限决定哪些操作可以执行，会话日志则把前面已经做过的事情记录下来。

模型接入这些能力以后，才有可能从真正去读资料、改文件、运行命令，最后交付一个成品。

![围绕模型搭建的一套执行环境｜权限和界面连接起来的一套执行环境](https://mmbiz.qpic.cn/mmbiz_png/XjrGzTnbp4a8TVycHVGBCAib1ibPfF49DPwHgTrJicJLA4CEptfHt0qU8VmibAt1iagX0uEpcDjgK9RQk47YdX16vItnvPkmoJ8MuSWsxAia61cEs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*围绕模型搭建的一套执行环境｜权限和界面连接起来的一套执行环境*

换成更专业一点的说法，Harness就是围绕模型搭建的一套执行环境。它把文件、工具、会话、计划、上下文、存储、沙箱、权限和界面这些东西连接起来。可以这么理解：Agent = Model + Harness。

如果拿大家更熟悉的工具来对比，Codex和Claude Code更接近已经调试好的一套成品工具，用户可以继续往里面添加Skill、MCP和规则。

DeepSeek Harness则把更多底层部件开放了出来。

它保留Cordis作为连接各个组件的基础，再让模型适配器、工具注册、会话日志、Agent Loop等模块通过插件的方式组合起来。

## 如何安装和部署DeepSeek Harness。
DeepSeek Harness可以在Windows和macOS上运行。在终端中输入下面这条官方命令。

- shell

- powershell

打开页面后，在模型设置里填入DeepSeek API Key，API Key 需要自行去DeepSeek官网的API开放平台获取。

![探索未至之境｜与DeepSeek免费对话体验全新旗舰模型](https://mmbiz.qpic.cn/mmbiz_png/XjrGzTnbp4aV9hFsymaRGBQYIl8gYiaJ7PpZA0SeP9GBEL2yA691UVeib8C8QnMugzmaibwdMuUluWiaNmoMTExmHHks1m4bS7IIwLklxdnb4es/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*探索未至之境｜与DeepSeek免费对话体验全新旗舰模型*

⚠️注意：API Key 不要发给别人，也不要直接放在公开截图里喔。如果不想自己操作终端，可以用电脑上已安装的Agent来替你执行这些操作（推荐）。可以将下面这段话发给 WorkBuddy/Codex/Claude code等桌面Agent工具。

![安装并启动完成。](https://mmbiz.qpic.cn/mmbiz_png/XjrGzTnbp4YbYW0CvicMGnfQWUrPr2Qq4GGH2xXXhHG5HExwRMSmXULohbufycZ99vibaQabPcKTtibqnDwElGKl7cjTDD5HFYpgIPr6Rz8bV0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*安装并启动完成。*

只需要点击它返给你的本地Web UI链接，或者在浏览器中打开，即可运行DeepSeek Harness了。

![探索未至之境预览｜描述你想要构建的内容](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4Zwv34VdOTv3WBTYfgmW3HPM9hCasicQq3rSyLFNzDfObNYAPZ9jBeUAicxlFuNNPxCpybNkLsjq77GDibjmuPpAcfJrNVbCFt4Eg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*探索未至之境预览｜描述你想要构建的内容*

## 最特别的地方，一切皆插件。
不少产品都有插件市场。

Chrome可以安装扩展，Codex、Claude Code和WorkBuddy也能通过Skill、MCP或工具增加能力。

DeepSeek Harness的差别在于，插件不只挂在Agent外面。

按照官方架构说明，模型适配器、工具注册、会话日志和Agent Loop本身也可以作为插件，并通过配置组合或替换。

这些插件由Cordis连接起来。

用户可以更换工具、存储、上下文管理、权限策略和交互界面，也可以为某类工作组装新的Agent preset。

自主性因此变大，配置成本和兼容风险也会一起增加。

也就是说，如果你对DeepSeek Harness里的某个部分不满意，可以直接替换对应组件，或者通过安装插件继续扩展，很多时候并不需要去改框架本身的源码。

![DeepSeek Harness 开发者预览版｜一切皆插件](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4aJBwZ3s7DuSDpDhWGibSrDTsmpQcBCdGYZctgfIfAv6zAKtn5Q5zqjGcdzRrRdt01ZauSOVfIATZZSicc3mT0ao5ApzypwZZ3UA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*DeepSeek Harness 开发者预览版｜一切皆插件*

我们可以在 Github 上搜索 dsh-plugin 标签，可以看到许多网友开源的DSH插件。

![scy1石片短剧](https://mmbiz.qpic.cn/mmbiz_png/XjrGzTnbp4YmoVHoyeaibZ3E1c1iaKSnJPx6fnOUZztRYpZjfwmAYD0EdEFdUHxPXU28Fytcxk7nuZVMN3H0JFD5q4ReicAQ6rXHCkdT5KZrTA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

*scy1石片短剧*

例如这个 dsh-web-ui 插件，它功能很强大，优化了原始UI界面的任务看板、Git图谱、右侧面板，内置了鲸鱼娘的桌面宠物，好包含了10款皮肤的选择。

![移动维远程｜葡鱼鲸宠物](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4a4r2Q6Ohz34y1f6EGDcopxDzaic5rdGpobkmw7cXvG0FxMPKloK6NoAPLFicFvyLPmgHxsGnexPHWlj1pXWh4fTzia3OPWlCpxTU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=10)

*移动维远程｜葡鱼鲸宠物*

安装起来也很简单，比如这个鲸鱼娘皮肤插件很漂亮，直接在DH的窗口中发送指令：

![探索未至之境 预览版｜DSH标准模式](https://mmbiz.qpic.cn/mmbiz_png/XjrGzTnbp4aBcn8ia7jboTbhE91xdEzjESzQtkaV1x2VrD9o9QlXs8XFkJzT7xvDyNc7MqLbicRTG8Fky6EE3PMLZhNibLT4DAIDOicEV2F9j7I/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=11)

*探索未至之境 预览版｜DSH标准模式*

帮我安装插件 zhu1090093659/dsh-web-ui。安装好之后，只需要重启 DeepSeek Harness，就可以更换UI了，。

可以看到，在设置-插件-插件配置中，已经多了一个 Web UI插件，这个就是刚才安装的插件，除了内置了9款皮肤，还增加其他面板的设置，比如非常实用的右侧面板。

![打开配置文件 ×｜![](30,79,54,100) 通用设置](https://mmbiz.qpic.cn/mmbiz_png/XjrGzTnbp4a29K2DRoPPu96x6gFusnB4z9C5FbfoMf4P7IxrNPibRgT7icgiaF6uecjhalf2DDWZTDafZprBlBkCCCoYteTiblgeibzZfCySdWRA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=12)

*打开配置文件 ×｜![](30,79,54,100) 通用设置*

![你这吃日饭的Session log｜鱼大肥鱼。](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4assiaFnCh9bay5ggaFdPqbRlrrooKV1S6wL70ed2Iz3kicYTs6oD1ovxkBFgUXQFqMxLamMm8pF0p7V3sOlbNKvTMbZQ45FDDN0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=13)

*你这吃日饭的Session log｜鱼大肥鱼。*

还有非常多插件的选择，喜欢体验的朋友可以自行探索。

![■ `dsh-focus-chat - ` 「聚焦会话」精简视图，只关注最终产出结果。｜代码名称 - 西羊石AI短剧](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4aspKg47gTJMs95wSExMefWgdlqWPl0miaeu814PrOHP2cX4Q1d2xiclMaicHPc41msLibUQL21bm6EuN2smqoXVB4yG4diawib7UE5g/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=14)

*■ `dsh-focus-chat - ` 「聚焦会话」精简视图，只关注最终产出结果。｜代码名称 - 西羊石AI短剧*

## 四种模式的选择。
我们当前官方预设里有四种使用模式，许多朋友可能刚接触不太明白。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/XjrGzTnbp4biclXPk5j0FoljibL1pUlJjjGYfPptrooXtXNKVrbICtrCSxTh1MDpic5HwFDzGxhYU8F8KzYXDExF6T8XxddZGPicpMqczjqLOoU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=15)

普通用户直接使用标准模式即可。PTC模式有一定技术门槛，另外两种可以先了解，不必急着用。创造模式可以把一套工作方法做成新的preset，这也是DSH很特别的地方。当前版本仍在快速变化，创建过程中会遇到插件结构、配置和兼容问题。

普通人可以先用标准模式把任务跑通，以后遇到许多重复项目，可以再决定是否值得把这些流程封装起来，会省下不少排查时间。

## 普通人可以用它做些什么。
前面讲了这么多，可能有些平时不太接触开源工具的朋友还是有点懵。其实没关系，对于普通用户来说，先把安装和基本使用跑通就够了。下面我们直接进入实操。

1. 将工作资料整理成HTML工作台

第一个案例，我们先从一份咖啡品牌的销售数据复盘开始。虚构品牌栖岛咖啡有12家直营门店，7月做了一次会员季活动。
