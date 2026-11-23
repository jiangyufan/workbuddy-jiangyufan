---
title: "我用 WorkBuddy + ima 做了一个知识点驱动的中考真题推送系统，对你"
source: "https://workbuddy.jiangyufan.com/index/hub/case/463"
type: "case"
chars: 2054
sections: 6
figures: 0
chapter: "02-我是老师"
---

# 我用 WorkBuddy + ima 做了一个知识点驱动的中考真题推送系统，对你
## 一 系统：它不让学生"搜题"。
市面上的题库产品，逻辑都是"你搜什么，我给什么"。但复习真正需要的不是搜索，是安排。所以我把顺序反过来：先知道学生学到哪了，再决定今天给他做什么题。这套系统知识点体系覆盖 207 个考点。数学 54 物理 25 化学 21 语文 16 英语 10 历史 50 道法 31。

![知耳语驱动 真题推送｜数学 物理 化学](https://mmbiz.qpic.cn/sz_mmbiz_jpg/icwwYHgFjjNZUriabOuNpurwcQphFkEsbnxKLY1XSxHjXIMT4AoAdXbFI1CmUs9ibib6pnCbRnVRY54lxCkHgjLibv3t4MKQaicDaL9QyN0wjetDw/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=0)

*知耳语驱动 真题推送｜数学 物理 化学*

它的六个模块是：今日练习—— 每天一份题单，由算法排，不由人挑。

![知识点驱动·真题推送｜数学 物理 化学](https://mmbiz.qpic.cn/sz_mmbiz_jpg/icwwYHgFjjNatIEFjjfzHyQb3cyApYfScBic5wZaTcib53QYzxsJwkvgwuiaSXUNjAYcRibV9oxPdFzaic6IEK4kjSOwOEw4ayj92Nd7AGDtICGVU/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=1)

*知识点驱动·真题推送｜数学 物理 化学*

知识点地图—— 板块 → 章 → 考点三层，"学到哪了"可以按年级设，也可以按章节勾选。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/icwwYHgFjjNa8tpf8gWia7CSbJEMZTun1tSFJJILXOYBG37tBnkGAuxvRVcgibj5kceEicEMKtbXhGBD3O7nS86iaXHIWXiaXcNbqzdIqcNCH4aNM/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=2)

进度看板—— 各板块掌握度一目了然。

![知讯点版吧·具能推送｜数学 物理 化学](https://mmbiz.qpic.cn/mmbiz_jpg/icwwYHgFjjNaibI2UtAib7ct8NpWnjTRo2vSfZa0aW2xbj4XGIeaFV944yzIysEoVnPZibc1DqTAAw5qYwsve4msFm4lchYgE0uQMU1rQshlraI/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=3)

*知讯点版吧·具能推送｜数学 物理 化学*

错题本—— 错题按 1、3、7、15、30 天的间隔回收。

![知识在规划，真正推进｜教学 物理 化学](https://mmbiz.qpic.cn/mmbiz_jpg/icwwYHgFjjNYiapZk0GNhefTLniajhU8c4Oqpdn3T0OeY4ofYolSLEYE2LcxIAgbqV0viaT6Uba1JwMMAkHqzjJ7q1NbFQsdiblicMMVrJk3t3a4I/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=4)

*知识在规划，真正推进｜教学 物理 化学*

题库—— 可切"只看真题"，每道题都标着出处。

![知识练习题｜数学 物理 化学](https://mmbiz.qpic.cn/sz_mmbiz_jpg/icwwYHgFjjNa2Yl8Gznx2daueHDaiae6WKah6a7NlZ9xsiateUVjO9sCr5ReuGPiaBR3gKbULNqoAdG9iblLiag33nPBicHayByKTDIjuSic3856MGM/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=5)

*知识练习题｜数学 物理 化学*

打印—— 一键出 A4 练习卷，可选附答案、附解析、标注考点、预留作答空间。

![](https://mmbiz.qpic.cn/mmbiz_jpg/icwwYHgFjjNZwjoltjnqnJQHzwHrcSnnnphwBfG8AzC80Soz2IUN7Y59fqX8jOyoe9l3rTpfIk9aez3pQAYCdXhiaKwe0tXfCweJias6nJibP4g/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=6)

![](https://mmbiz.qpic.cn/mmbiz_jpg/icwwYHgFjjNZ6OUQC5TkFum42qTehBbQwKfUGDFiaTWbjAeJtbGbEfibmJDsT9Jhl0QvXh3YQD3CicxeYQY7XMN224agUp632kvjEkYicQicbpxwQ/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=7)

它有两条硬约束：

- 只从"已学"考点出题，不会推出还没学过的知识 ② 真题优先，同一考点下真实真题的排序权重高于演示样题

排题不是随机抽。优先级由六项加权算出：

掌握度 0.34 遗忘后的保持率 0.24 中考权重 0.18 久未练习 0.12 前置考点是否就绪 0.12 近期曝光过 扣 0.20。

每天先留不超过 30% 的名额回收错题，再推进新考点，其余做滚动复习；前置考点没学好的，该考点降权 35%，先回头补地基。

技术上它是一个零依赖的本地网页：双击 index.html 就能用，数据存在浏览器本地，不上传、不联网。

二 题从哪来：ima 存，WorkBuddy 造。

## ima 负责"存"。
我在 ima 订阅了「天津中考知识库」——834 份资料、3.7 GB，天津历年各科真题、各区一模二模三模卷、复习资料都在里面。这是我整个系统的题源。

ima 在这里做的是它最擅长的事：把散落的资料收进来、存住、并且能被检索到。

更关键的一步：WorkBuddy 通过 ima 连接器，可以直接列出我订阅的知识库、按关键词检索、并把文件正文取回来。

以 2017 年天津中考化学卷为例——检索到之后取回的正文里，每道题后面都带着【答案】【解析】。也就是说，ima 已经把 PDF 解析成了带公式的文本，我拿到的不是一堆图片。

## WorkBuddy 负责"造"。
拿到正文之后，把"文字"变成"题目"，是 WorkBuddy 的活：

1. 结构化 拆成题干、选项、答案、解析，标上学科、年份、地区、分值、难度，再挂到知识点树的对应考点上。2. 校验 计算题独立重算一遍——卷上写 88.3%，我得自己算出来也是 88.3% 才收；解析出的歧义按学科常识定案，并把理由写进注释。3. 写测试 319 项断言，锁死两条底线——每道题必须能追到原卷题号；解析里不许出现"更正""我认为"这类字眼。4. 生成和维护应用 题库文件、调度算法、界面、打印排版都是它写的，改完跑一遍测试。5. 导出与回传 题库导出为 CSV / JSON，同步回 WorkBuddy 资料库。之后在资料库里问"物理电学欧姆定律"，能直接检索到题干、选项、答案和解析。

## 分工大致是这样。
收集、存储、检索资料 → ima 取正文 / 读本地文件 → WorkBuddy 结构化、挂考点 → WorkBuddy 执行，我拍板 复算、定取舍 → 我拍板 写测试、跑测试 → WorkBuddy 应用、打印、导出、同步 → WorkBuddy。

## 还有一条备用路径。
连接器不是每次都能用。有几次，ima 的工具调不出来，我走的是另一条路：从 ima 客户端把 PDF 拖进对话，WorkBuddy 直接读本地文件，再跑 OCR——PyMuPDF 渲染 + RapidOCR 识别，一份 14 页的卷子约 6 分钟。2015、2018、2019、2020、2021 年的化学卷都是这么进来的。

两条路的区别：连接器通的时候，拿到的是 ima 已解析的文本，质量更高；不通的时候自己 OCR，慢一些，但对付扫描件够用。

重要的是两条路都能通向同一个下游——结构化、校验、入库、测试，这一套流程不变。三 AI 不能替我做的那一件事。这道题收不收"，这道关我始终自己拍板。

一道题脱离原图能不能做——化学卷里"下列实验操作正确的是（）"，四个选项全是图，不收；解析里出现两个互相矛盾的数字，取哪一个；答案和题干对不上时信谁。

这些判断背后是学科常识，也是责任。

2015 年那卷，最后进库 26 条，另有 4 处明确放弃：实验操作正误图、装置图中仪器的名称、选发生装置字母、选洗气瓶进气口序号。

其中装置图那道我拆开收——两个化学方程式不依赖图，收进来；填字母和序号的小问，放弃。每一份题库文件的开头，我都写了一段"不收清单"。这套系统里，那份清单比题量更值得看。这也是我对"AI + 教育"最实在的一点体会：AI 最可靠的用法不是替你出结论， 而是把"把事情做扎实"的成本压下来， 让你有余力去较真。

## 四 还差什么。
我优先把化学真题都放进来了，其他的还没放多少，想着先把用化学这科跑通。后续还可以加入针对错题自动生成相关练习功能，关键是只要有思路，现在做起来很容易。
