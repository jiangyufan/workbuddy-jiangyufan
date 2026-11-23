---
title: "深度拆解WorkBuddy新功能「人机双写」：好用吗？如何用好？"
source: "https://workbuddy.jiangyufan.com/index/hub/case/925"
type: "case"
chars: 3556
sections: 4
figures: 0
chapter: "13-产品更新与判断"
---

# 深度拆解WorkBuddy新功能「人机双写」：好用吗？如何用好？
![AI为什么终于能直接改 Office了?｜拆解WorkBuddy「人机双写」的底层机制与能力边界](https://mmbiz.qpic.cn/sz_mmbiz_jpg/O8sK574ibiatopEibdqCiacXoy35BeXqcUdnLrrBeWpv3uPsQ3vibqP01pCNLcoI2E1Fchy0iaYRLibrVlEuBW4R1yMjNub7UUn1zicGibxT3HxXKXLA/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*AI为什么终于能直接改 Office了?｜拆解WorkBuddy「人机双写」的底层机制与能力边界*

AI为什么终于能直接改Office了。

最近，WorkBuddy 官方发布了一篇文章，标题很直接：《刚刚，把 Office 装进了 WorkBuddy，实现了人机双写》。

文章里演示了一种很顺滑的工作方式。

打开一份 Word、Excel 或 PPT，选中里面的文字、表格、图片或者某个页面元素，点击「AI 编辑」，再用自然语言告诉 WorkBuddy 想怎么改。

AI 修改以后，结果会直接出现在当前文档里。人可以接着改，AI 也可以继续改。

![帮我润色一下｜+新建任务](https://mmbiz.qpic.cn/sz_mmbiz_png/O8sK574ibiatqgn57aZA6taHmPS6Dlj8SETLUrGBldb3oJ7bH8j4ibFibS1Y4rI1FubSTIuHHnT6Lu8cY5Cr9Pr5oP4pxUS8EibpLjYF2VgV5bLU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*帮我润色一下｜+新建任务*

WorkBuddy官方展示的选中元素直接AI编辑入口。官方把它叫作「人机双写」。如果只看演示，这个功能很好理解：以前要来回复制粘贴，现在可以让 AI 直接在文件里动手。但我看完以后，第一反应不是「这个功能真方便」，而是冒出了更多问题。

过去 Agent 进不去 Office，不是因为不会写字，而是因为它不知道怎么准确操作一个 Word、Excel 或 PPT。现在为什么突然可以了。

它修改的到底是不是原文件。背后调用的是插件、Skill，还是 MCP。Word 里的一段话、Excel 里的一个格子、PPT 里的一个文本框，在 AI 眼里究竟是什么。如果它真的在原文件里修改，原来的样式、公式、母版、动画、宏和复杂对象还能不能保住。

这些问题，官方文章没有展开。

而我最近正在给电子工业出版社录制《WorkBuddy Agent 工作台实战课》。如果只把官方功能重新演示一遍，价值很有限。

我真正想讲清楚的是：这项能力为什么现在能够出现，它和过去的 Office 生产方式有什么本质差别，以及我们到底可以信任它到什么程度。

所以我没有先写教程，而是从课程项目里复制了三份真实文件：一份旧版 Word 合同、一份包含多个工作表、公式和图表的 Excel、一份 15 页的原生 PPT。

然后，我让 WorkBuddy 分别在这三份文件里完成一次真实修改，再从编辑器工具、文件结构和保存结果三个层面，做了一轮黑盒拆解。

这篇文章，就是我拆完以后得到的答案。

## 过去，AI 为什么总要先把 Office「搬出去」。
先从一个大家很熟悉的现象说起。过去我们让 Agent 处理 Word，常见链路是这样的：

Word → 提取为 Markdown 或其他中间格式 → AI 修改内容 → 重新生成一份 Word。

Excel 和 PPT 也类似。Agent 可以先读取里面的文字和数据，再通过脚本或专业 Skill 生成一份新文件。这条路线当然有价值。我之前做 Word、PDF 和 PPT 课程时，大量使用的就是这种方法。但它有一个本质问题：AI 处理的是从 Office 里提取出来的内容，不是我们正在操作的那个 Office 工作现场。

![过去是搬出去重建，现在是进入原文件协作｜核心差别不在写得更快，而在是否共享同一个工作现场。](https://mmbiz.qpic.cn/mmbiz_jpg/O8sK574ibiatps0IcUzVQ1G8VP2ibsmYbFJqBREVOiatlu0oRgwkvPhUjGfsRrFFso4sFnQva51ibOYjHmQutsjKohL9EngrjuxTVZwgibjTaUvb4/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*过去是搬出去重建，现在是进入原文件协作｜核心差别不在写得更快，而在是否共享同一个工作现场。*

过去搬出去重建，现在进入原文件协作。为什么要先转成 Markdown。

因为 Markdown 是一种结构清楚、机器容易读写的文本格式。标题、列表、引用、代码块都可以用简单符号标出来，Agent 很容易理解。

可一份真正的 Office 文件，远比一篇纯文本复杂。Word 里不仅有文字，还有段落、文字范围、表格、图片、页眉页脚、分节和样式。Excel 里不仅有数据，还有工作表、单元格类型、公式、图表、透视表、条件格式和外部连接。PPT 里不仅有每一页的文字，还有文本框、形状、图片、坐标、层级、母版、备注和动画。

过去的 Agent 能读出很多内容，却很难准确回答这些问题：你说的「这一段」，在文档里的起止位置到底在哪里。你说的「这个格子」，属于哪一个工作表，是字符串、数字还是公式。你说的「右边那个副标题」，到底是第几页的哪一个 Shape。你手动改完以后，AI 怎样知道当前页面已经发生了变化。

所以在很多 Agent 产品和内容生产场景里，更常见的做法，是先把内容搬到机器容易处理的中间格式里，改完以后再生成 Office 文件。

说得再直白一点：过去不是在装修原来的房子，而是把屋里的东西搬出来，整理完以后，再盖一间新房子。这适合从零生产一份报告、白皮书、课程手册或者整套 PPT。但如果你只想修改一个段落、补两列公式、调整一个文本框，这条链路就显得很重。更麻烦的是，人和 AI 很难围绕同一个最新版本连续工作。

AI 生成一个文件，人打开修改；下一轮 AI 又要重新读取。每次协作都像重新交接一次任务。

## 这次升级，不是 AI 更会写了，而是终于有了「手」。
很多人看到「人机双写」，会自然理解成模型能力升级了。但我拆完以后，最核心的判断是：

真正的变化，不是 AI 的脑子突然变聪明了，而是 WorkBuddy 给 AI 装上了一只能够伸进 Office 编辑器里的手。

![不是更会说，而是终于能动手](https://mmbiz.qpic.cn/mmbiz_jpg/O8sK574ibiatoMZb8AJIVzZdBqNMicibNHbXayVwtyic2SMaWANLKogmuu5icNokvSYBtLaXfhtwtibV5zTE6F9BycdVUQSUqQ9kRQqhHZ1yCtztRI/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*不是更会说，而是终于能动手*

不是更会说，而是终于能动手。过去，模型可以分析一句话该怎么改，也可以给出修改建议。但它没有一个稳定的操作表面，不能可靠地把「改这里」翻译成一个确定动作。

现在，WorkBuddy 打开本地 Office 文件以后，不只是把它当成静态预览图展示出来，而是把它加载进一个真正的文档编辑器。

这个编辑器会把文件解析成一套可以查询、定位和修改的对象模型。人看到的是一份正常的 Word、Excel 或 PPT。AI 看到的却更像一张对象清单。例如，你在 Word 里看到一段文字，AI 看到的可能是：文档中的某个文字范围 起始坐标：2899 结束坐标：2959 对象类型：段落。

你在 Excel 里看到 B7，AI 看到的是：工作表 ID：000001 行：6 列：1 值类型：STRING。你在 PPT 里看到一个副标题文本框，AI 看到的是：第 1 页 Shape ID：000034 对象类型：文本形状 位置与尺寸：一组确定坐标。

![AI如何把「这里」变成准确地址?｜页码/页面 ID](https://mmbiz.qpic.cn/mmbiz_jpg/O8sK574ibiatrpOQWPiczZxtu83Jw4bU2Jib7osHoay9hxY9icNffRetJITuKcibLxZLHqL95NJ3dkTa1Veick7533WianwVfPVCUS1ibZu1a6Dqibz1I/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*AI如何把「这里」变成准确地址?｜页码/页面 ID*

把这里变成准确地址。这一步非常关键。

在编辑器已经识别并选定对象的前提下，「这一段」「这个单元格」「这个文本框」才有机会被翻译成机器能够执行的具体地址。

## Skill、MCP、编辑器，到底谁在干活。
这里最容易讲乱。

有人看到 Skill，会说「是 Skill 在修改 Word」；看到 MCP，又会说「这就是一个 MCP 插件」。这些说法都只对了一部分。

可以把整条链理解为一次接力：

Skill 是操作手册和路由规则：告诉 Agent 先做什么、调用什么、注意什么边界。本机能够确认的两个关键入口是 tencent-docs-routing 和 tencent-local-office-edit。

MCP 是标准插座：把读取 Word、写入单元格、修改 PPT Shape、保存文件等工具，以统一方式暴露给 Agent。

editor_sdk 是执行发动机：在本次本地 Office 编辑链路中，它持有打开的文档实例，执行对象级修改、维护编辑状态并保存文件。

编辑器是共同工作现场：它把当前文档呈现给人，并连接 editor_sdk 持有的编辑实例。人和 AI 的修改进入同一个文档模型。

压缩成一句话：

Skill 告诉 Agent 怎么做，MCP 提供标准插座，`editor_sdk` 真正执行修改，编辑器让人和 AI 围绕同一份文档继续工作。

![一次Office 修改，五个角色如何接力?｜人:提出要求/检查/接管](https://mmbiz.qpic.cn/mmbiz_jpg/O8sK574ibiatqdJDL41ZFeCHSEiahBTogqV1wDNvDbYQ4pHHGqlysDicm3yc5xkAHe93hUVaCgOq58NckMiazdlJxcdlzdAEp25qpYKYibqEdj3Iw/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*一次Office 修改，五个角色如何接力?｜人:提出要求/检查/接管*

Skill MCP editor_sdk与编辑器分工。这也解释了一个重要问题：它不是一个需要用户额外去市场里安装的普通 Office 插件。

当前本机看到的，是随 WorkBuddy 应用分发的腾讯文档内置路由 Skill、本地编辑 Skill 和 editor_sdk 工具层。

但基于黑盒证据，我们也不能反过来断言产品内部完全不存在插件化封装。能确定的是：用户不需要自己另外安装一个市场插件，才获得这项能力。

## 为什么 AI 一改，页面上就能马上看到。
如果 AI 只是偷偷修改了磁盘上的文件，页面为什么会立即变化。答案是：AI 操作的不是一个冷冰冰的文件路径，而是一个已经打开、带状态的编辑器实例。

文件进入编辑器以后，会获得一个临时的会话标识，可以把它理解成当前文档的「工位号」。在工具里，它叫 file_id。

打开文件 ↓ 获得当前编辑器实例的 file_id ↓ 读取段落、单元格或 Shape ↓ AI 写入当前文档模型 ↓ 修订计数递增 ↓ 变化同步到页面 ↓ 人继续修改或确认 ↓ save_file 保存到本地。

![为什么AI一改，页面上就能马上看到?｜① 打开文件](https://mmbiz.qpic.cn/mmbiz_jpg/O8sK574ibiatocyqEWumibA8WYW3KJuAlSFE3ntoFHvXl3eJp6ZP2fx4rFdDn9ibwAsg3fvbbeicLfDWNmPHOOva7jqsn9hApDY0On4zmibORsrP8/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*为什么AI一改，页面上就能马上看到?｜① 打开文件*

同一编辑器实例中的实时协作闭环。我在三类文件的实测中，都看到了修改后的文档修订计数递增：Word：0 → 1。Excel：0 → 1 → 2。PPT：0 → 1。

Word 还暴露了 AI 编辑记录和回退能力。部分 Word 和 PPT 工具说明里，能够看到 Revision、Undo Unit 和 SSE：简单理解，就是记录一次修改、支持按操作撤销，并把变化推送到页面。
