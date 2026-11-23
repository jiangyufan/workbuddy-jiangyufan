---
title: "腾讯混元Hy4 flash + WorkBuddy，把模型生态正式补齐。。。"
source: "https://workbuddy.jiangyufan.com/index/hub/case/758"
type: "case"
chars: 2013
sections: 0
figures: 0
chapter: "09-我要省模型成本"
---

# 腾讯混元Hy4 flash + WorkBuddy，把模型生态正式补齐。。。
大家好，刘聪NLP。

两周前，腾讯混元 Hy4 正式版刚刚发布，我当时还进行了一手实测，见，Hy4正式版 + WorkBuddy，直接拿大结果。

进步很大，算是混元正式进入国模第一梯队了。

![要拿大结果了](https://mmbiz.qpic.cn/sz_mmbiz_png/oUDMrTdAeRN8Hc3AXiaovM3WDUSO0EgW1EAM4aKK599K8Oz0EFoY2CH3TUiaLTHKicVSSKUCKiaqf077cBoacxNiazEkcUNP703P5DPtCsXUYOGQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*要拿大结果了*

没想到 flash 版本这么快就来了，这次更快，没有了之前的雷霆大思考，更加适合办公、高频重复性场景，。

算是把模型的所有生态位都补齐了，。

Hy4 flash 的总参数量为 224B（其中 64B Engram 参数），激活参数 12B，支持多模态和 1M 上下文长度，API 价格相比 Hy4 大幅降低。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/oUDMrTdAeRORk4BDH6fssQBkLEOoHBt872FZ1pPl8JNKViaiaib1bNzOfBxE5hiceia4JjZic0xaRPZooDtEA87uLmTVxlwzicDlFb7KbwsaHvnmbU/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

![创作文档 分析数据 代码开发 UI/UX 生图生视频 金融服务｜今天帮你做些什么？@添加上下文，/调用技能与指令](https://mmbiz.qpic.cn/sz_mmbiz_png/oUDMrTdAeRMlGlibKUljnxXvCuvsfEkaJ4icLBJzQPRFpQjGGophjcH3mp3f81tW0wMDRd2NVB3fPg0JIrtAdf9TJZJYUejEk0biaSeKJtvPz8/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*创作文档 分析数据 代码开发 UI/UX 生图生视频 金融服务｜今天帮你做些什么？@添加上下文，/调用技能与指令*

先给大家带来一手测试，整体体验如下，。

速度确实快很多，任务完成时间会大幅缩短，没有雷霆大思考了，整体输出会简洁很多，更多适合场景办公、高频重复性的工作，。

前端、3D、后端的效果相较 Hy4 正式版有大幅下降，大概是 Hy4 preview 的水平，。因为思考没那么长，所以现在是指哪儿打哪儿，一般不会进行多余一点泛化，复杂任务需要多轮。

视觉推理还不错，我之前弄的推箱子游戏，第5关可以完成，但也会存在一些反复横跳的情况，但相较于其他 flash 模型要好不少。

先来看一个教育场景，比如做一些物理实验的实验演示，。探究物质质量与体积的关系，用天平和量筒测出不同铜块、铁块的质量与体积，得出比值关系。

整个演示，把称重、量筒读数、记录数据和归纳结论都讲清楚了，当换成更大的铜块，质量和体积都增加，同时质量除以体积的比值不变；换成铁块，就能看到两种材料的比值不同。这样密度这个概念，就很清晰的跟着操作过程呈现出来了。

整个内容， 8min 就出来了，算是又快质量又不错了，我这里对比了 Hy4 正式版和 DeepSeek-V4.1-Flash 整体消耗情况，Hy4 flash 还是从性价比，到任务完成，都很优秀。

![](https://mmbiz.qpic.cn/mmbiz_png/oUDMrTdAeROOZajuwprX2hlGzibIaWSFjhgRTYNwYEpeXS8sshta5UlYvsBU4DHUmhicGiaork9BxlhrB3EianVC2gSWHHkFGwykr6g1ibWwTatA/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

发动机内部的叶片、燃烧室这些结构都有做出来，启动以后，尾焰、转速和温度读数也会跟着变化。可以旋转视角、放大看内部，整体交互还是比较完整的。

接下来是锦鲤池交互场景，点击水面会出现一圈圈波纹，附近的鱼会受惊游开。水面光影和鱼摆尾游动的效果也不错，做这种小场景，还是挺有感觉的。

不过，也有一些 bad case，上一篇 Hy4 测过的键盘复刻，这次就没那么理想。对世界知识有所缺失，外观做出来了，但右侧数字区和方向键附近的排布有些串位。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/oUDMrTdAeRPNtoYrqp6gAQxK9GQPcND1XLqVET5ESJzVicpoLhfkicLDu89G7CYzictoG0mdhebcWicibtDFnlfWdDlSNoOXPDoEf8qA8N6PeG0Y/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

当然，flash 在办公场景表现的很好，。我们先看看之前我们常做的表格还原任务，。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/oUDMrTdAeRNRUiapHFep9ZBficAXFWQForrL82PxrYmV4qRlARr6gLTxLGRH6eRLHT1Kkd6fFtoEAPbZ3dmLavAYU6V7YABFVR3em2AR0eqyQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

结果如下，表格结构、内容都没有问题。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/oUDMrTdAeRM5JKWY0L5CnOabZndVcQD6bgAjRSE9icficWo5JK65cPQJ77uFTcrSnO2ZcPp7vvvk7a5S9CiacjiaNTVCjWicXz7Va2C53CFStCeY/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

还有几个 Fable5.2 很牛逼的 case，让 Hy4 flash 复现了一下，来自 X@MiaAI_lab，。

复现一个单笔风景绘图机，模拟机械绘图机用一支笔逐线绘出山、湖和树林，要求能看到笔尖移动、抬笔与绘图进度。

![做好了，单文件、零依赖：  plotter-no-2.html](https://mmbiz.qpic.cn/mmbiz_png/oUDMrTdAeRMWKgrO3Y97RLibqq9Wibr5zicYnO532qhEiauotiaK1Z4vRuZu497bV6ScT9MAribT9Mq6FlDNCc3ib2lrzkABtazX7qgqVwusEDDATY/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*做好了，单文件、零依赖：  plotter-no-2.html*

效果如下，山体的排线、湖面的线条和树林会跟着笔尖逐渐出现，绘图进度也在往前走，整体实现得还不错。

复现木活字掉落印刷，输入字母，让木活字像积木一样落下堆叠，再上墨、压印和翻纸，把随机排列变成可保存的海报。

![已完成，单文件可直接打开玩 hell-box.html (50KB，无依赖)。预览已打开。｜真实跑通的核心链路](https://mmbiz.qpic.cn/mmbiz_png/oUDMrTdAeRPCs04ruiaaVjywEKZ25iac0rx6ticpo84quTryqOibJ04C4O2RUvFKZhzRia5JGhUEVjICck8YIf50S7TacF8YDnDysZ0RtUgdq8Sw/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*已完成，单文件可直接打开玩 hell-box.html (50KB，无依赖)。预览已打开。｜真实跑通的核心链路*

效果如下，木字块会翻转、碰撞，堆在底部，还能把堆好的字块重新摇散。点击印刷以后，会弹出一张带有油墨质感的印样。

还有一个火星温室控制台，字符终端风格的温室模拟，展示作物、水循环、电力和日志；沙尘暴来临时需要分配有限能源。

![](https://mmbiz.qpic.cn/mmbiz_png/oUDMrTdAeRMXEGm84bdMQDiaricMSYyzAiaIPlhKd3RkzrMjdXmIxAsFvpv2AyEibykV4L0cX6S7U2owY24ricWfnRMgSVGT5f76pASwZWsUibjR8/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

效果如下，页面里的电池电量会持续变化，调整照明的操作也会写进日志。音乐也可以放，配上这种老式屏幕和字符画，整体感觉还是挺到位的。

还有之前的推箱子实验，hy4 第五关可以通关，但是也会出现一些重复执行的步骤，其他 Flash 模型很多无法在规定的时间和步骤里通过，。

同时速度很快，相较于其他雷霆大思考的flash模型，Hy4 flash的效率是极高的。最后，。腾讯混元这波算是把模型生态位都补齐了，。flash 版本、正式版本都有，你可以根据你的真实任务场景选择合适的模型。并且在国内大家对Work Agent的认可度也是越来越高，。

已经从原来的vibe coding到了现在的vibe working，。我们的agent work社群都已经快 50 个了，。

![AgentWork 社群交流群 45 (200) 外部｜AgentWork 社区交流群 37 (195) 外部](https://mmbiz.qpic.cn/mmbiz_png/oUDMrTdAeRMASgH3MRxP9ACQDp1AEbcAeJeaIIp9DDwjgbasmhhjBIng3gK5cp8yUgZYsOy1icHaNAGOm4TpX0jgibEnia5ibzlkHib7eOzgsV60/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*AgentWork 社群交流群 45 (200) 外部｜AgentWork 社区交流群 37 (195) 外部*

说明国内的agent 工具，是可以解决大家真实落地场景问题的。当然，不可否认，我们现在跟国外的顶级闭源模型还是存在差距，。实话实说，Fable5.2出来的时候，我感觉天都塌了，。国内外的差距又大了一些，但是这不影响我们追逐的步伐，。只能说，我们需要继续加油啦～。

最最最最后，现在在WorkBuddy上使用Hy4 flash 免费，赶紧用起来吧。
