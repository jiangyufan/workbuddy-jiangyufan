---
title: "我用 WorkBuddy 把用了三年的手机速度提升了五倍"
source: "https://workbuddy.jiangyufan.com/index/hub/case/603"
type: "case"
chars: 1814
sections: 6
figures: 0
chapter: "12-我看别人怎么用"
---

# 我用 WorkBuddy 把用了三年的手机速度提升了五倍
我的Vivo手机用了三年，速度越来越慢，最近卡到什么程度。点开微信，转圈的时间够我喝一口茶。

相信使用安卓手机的朋友，时间长了都有类似的感受。我试过自带“手机管家”的一键加速，也清理过无数次“垃圾文件”。每次刚清理完好像快了一点，但过不了多久，又恢复原样。

今天我突发奇想，能不能用 WorkBuddy 来给我“整顿”一下手机。马上行动：用 Type-C 线，把手机连上我的电脑，打开 WorkBuddy，问它：

![](https://mmbiz.qpic.cn/mmbiz_png/37JPSyiaMbkUvOicu9NKwWIUIUt1dVhveCV10aC0IrHuemdoGyQAxeVeeSicjHrDIO02zJqusHyN6XcQYtULVMTmt5l8zzw3JWaphXlrBRrw28/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

然后它告诉我：

不过有一条技术路径可以让我真正帮你诊断：在手机开发者选项里打开「USB 调试」，再在 Mac 上装个官方小工具 adb。这样我就能通过电脑读到手机真实的运行内存占用、后台进程、存储明细、电池健康等数据，给你一份针对性的卡顿体检报告，甚至帮你禁用某些顽固的自启软件。

要不要走这条路。如果要，我可以一步步带你开启 USB 调试、在电脑上装好工具、然后连上手机帮你做一次实测诊断。

我参考了这篇文章，打开了 USB 调试选项：

![](https://mmbiz.qpic.cn/mmbiz_png/37JPSyiaMbkVzHxtPxhiakAejEibLY7Z9Y82qRh2esESSIedKKv8aq0vw6eGlCzuwUypicL0BNLa6c5dk6rOCWkn1GenhfzibWd5Y3brKIrC6Su8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

接下来就看 WorkBuddy 的表演了，只需要按照它的指示，逐步确认即可。

![已规划步骤、执行操作｜已执行操作](https://mmbiz.qpic.cn/sz_mmbiz_png/37JPSyiaMbkUiaT3kzCsDO0iauMTaYogQ2LpQ4IYMxyg6Mgps76Sjahbx2q3Kadaa7nGNV7Tia6Kib2lXUP3G8ibT5BCXHXT2tyfiafC7Y7fynpVTY/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*已规划步骤、执行操作｜已执行操作*

## 接下来，它做了几件事情。
1. 生成了一个详细的“卡顿体检报告”。

![一句话结论](https://mmbiz.qpic.cn/mmbiz_png/37JPSyiaMbkW4CoIQX5lEZxJ29xqnCtgoibKyK2epLiagfBhRqRUtI8CT3t4H16nMBedWMyYicsJgbUibT1ul0nf8dmsAeQtBs38UE5uzDibicVTJs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*一句话结论*

1. 给出了具体的“整改措施”：

把常驻的无关 App 真正卸载或冻结——治本。关掉大部分 App 的"自启动 / 关联启动"。关掉"内存融合"或调小。动画时长改成 0.5x （这可以参考我之前的一篇文章）。

1. 完成整改之后，重启手机，效果非常明显：

![重启后来复测一下，对比看效果（只读，不改动）。｜☑已执行操作](https://mmbiz.qpic.cn/sz_mmbiz_png/37JPSyiaMbkVB0jZVRHxiczrsk0ah5iaTq1libskq0DnzHYmME2nHlaVBdz1bqQ9FmGd8pCdUV8Npm7TmYUl6l4ryIttzJY0EKKaicWibGHBND1Sc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*重启后来复测一下，对比看效果（只读，不改动）。｜☑已执行操作*

接下来我又按照它后续的建议，对一些常用的 APP 做了优化，提速效果更佳明显。感受上，就是：这台用了三年的旧手机，终于恢复到了让我不再想立刻换机的状态。这已经够值了。

## 总结一下其中的几点经验。
1. 为什么手机自带的清理软件没什么用？

很多清理软件主要处理的是缓存和存储空间。这就像给办公室擦桌子：桌面确实干净了，但如果桌子下面塞着一堆正在运行的机器，办公室照样又挤又吵。

WorkBuddy 对手机的体检说明：问题很可能不只是垃圾文件，而是后台负担过重。

1. WorkBuddy是怎么“看见”手机的？

过程是，我在手机上打开开发者选项和USB调试，通过数据线连接电脑，并在手机端确认了这台电脑的调试授权。

WorkBuddy调用电脑上的ADB工具，读取手机允许访问的系统状态，例如：内存使用情况；存储空间；正在运行的进程和服务；已安装应用的包名；部分应用的资源占用。ADB是Android官方提供的调试工具。它的能力很强，因此权限也不低。所以，这一步有三个前提：

只连接自己的手机；只授权可信的电脑；使用结束后关闭USB调试，并撤销不再需要的授权。这不是让AI随便进入手机，而是人在授权范围内，让AI协助读取和分析数据。

1. 我没有让AI自动清理，而是先让它列清单

发现问题后，我没有对WorkBuddy说：“你看着办，全部优化一下。”。这句话听起来省事，实际上风险最大。因为AI看得到资源占用，却不知道哪个应用对我重要。

它认为一个App使用频率低，可能建议停用；但这个App也可能是我每个月必须使用一次的软件。所以，我让它先输出一份任务清单，由我确认之后，再执行下一步。

这个动作非常关键：AI负责找线索，人负责做决定。

## 最后，这段提示词可以直接复制。
手机连接电脑、打开USB调试，并确认ADB能够识别设备后，可以对WorkBuddy说：

## 第一步：只诊断，不执行。
请读取这台安卓手机的内存、存储、后台进程和服务状态，分析卡顿可能来自哪里。

现阶段只做诊断，不要卸载、停用、清理或修改任何设置。请列出证据，并区分“已确认问题”和“待确认线索”。

## 第二步：输出待处理清单。
请列出可能需要处理的第三方应用，包括应用名称、包名、资源占用、判断依据、建议动作和恢复方法。

不要处理系统组件、桌面、输入法、电话、短信、账号、安全、支付和设备管理类应用。执行前必须等我逐项确认。

## 第三步：确认后再处置。
只停用我已经确认的这些第三方应用，不要卸载，不要删除应用数据。执行完成后，输出操作记录和逐项恢复方法。

如果发现误伤，可以说：这个应用是我需要使用的，请恢复启用，并检查是否已经能够正常运行。提示词不复杂，最重要的是三个原则：先诊断、再确认、可恢复。下次，如果你的手机速度很慢，值不值得换。别急着下单，先用WorkBuddy给它做一次体检。我是崔博，我们下期见。
