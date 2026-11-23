---
title: "用 WorkBuddy 给孩子搭了个错题本工作台，期中前终于能用了"
source: "https://workbuddy.jiangyufan.com/index/hub/case/454"
type: "case"
chars: 2369
sections: 4
figures: 0
chapter: "02-我是老师"
---

# 用 WorkBuddy 给孩子搭了个错题本工作台，期中前终于能用了
上个月孩子月考数学差点不及格，我这当家长的，心里一直搁不下。其实早就想用 WorkBuddy 给孩子弄个错题本了，但一直没想好要做成啥样——既想要方便，又想要少花钱（那些这个会员那个会员的，能不买就不买）。结果一拖再拖，拖到又要期中考试了。得，先弄个能用的简单版，后面再慢慢加功能。

## 一、说干就干：在 WorkBuddy 里建个"家"。
这步没啥技术含量。打开 WorkBuddy，新建一个任务，选好工作空间，我给这个任务起了个名字叫「火山错题本」——意思是错题像火山一样，攒多了得赶紧处理。

起名这事儿随便，关键是给它安个"家"。后面所有的错题照片、整理页，都归到这个任务的工作目录底下，清清楚楚，不丢三落四。

## 二、把需求一次说清：给 WorkBuddy 的提示词。
这种活儿，最关键的其实不是工具，是把需求讲明白。你含糊，它产出就含糊。我把脑子里想的整理成一份提示词，发给了火山错题本。

下面是我优化过的版本（第一稿我写得很乱，后来改成了这种分块、带规则的写法，效果立马不一样）：

我是一位初中学生的家长，想用你来搭建一个本地的「错题本工作台」（用 HTML 展示），帮孩子整理数学错题。【工作目录】D:\数学错题库 - 原始题/ ：入库时存放原始错题照片 - 整理后题目/ ：每道题生成一个整理页 HTML - 错题总表.html ：一直更新、汇总所有题的表格，并链接到各整理页 【入库方式】我在任务栏拖入一张错题照片，并说"入库"，你要帮我： 1) 把照片存到 原始题/ 下； 2) 整理成一份 HTML 放到 整理后题目/ 下，字段包括： 原题、我的答案(错的)、正确答案、错因分类(计算错误/概念不清/审题不清/粗心大意/方法不对)、涉及知识点。规则：我没给你的内容就留空，绝不要自己编。3) 基于原题再生成 3 道类似题（题目+答案放进同一份 HTML），要求： a) 数字全换新，但考点不变； b) 难度与原题一致，不许变简单。4) 把这道错题追加进 错题总表.html（含以上字段 + 链接到整理页）。【工作台四大模块，用 tab 切换】 1. 入库 - 显示最新入库的题目（原题/错答/正答/错因/知识点） - 可编辑以上字段并"保存"，写回整理页 HTML - 有"增加"按钮，手动录入一道新题，复用上面的入库逻辑 2. 错题本 - 列表展示所有错题（原题、错因、链接到整理页） - 可删除；底部用进度条统计各错因数量分布，并按知识点统计数量 - 注意：只读…

我主要做了三处优化，你可以照着学：

- 把需求拆成"模块"：原来我一股脑写下来，WorkBuddy 容易漏。拆成入库 / 错题本 / 随机抽测 / 类似题四个模块，每个模块要干啥写得明明白白。
- 把"不知道就留空"这条铁律写死：孩子哪次错因为啥，照片上不一定看得出来，我就明确说"没给的别编"，不然 AI 给你编个错因，反而误导。
- 类似题下了死命令：数字换新、考点不变、难度不变。不然它为了"友好"把题出简单了，练不出效果。

## 三、拿一道真实错题跑一遍。
工作目录我设在 D:\数学错题库。正好手头有一张孩子八年级的错题照片，就拿它试。原题是这样的：

![](https://mmbiz.qpic.cn/mmbiz_jpg/95icgMZNPWIqPAFuHoYAky5Af5PgniacxV0O6xMosoQEicY5jGwkhPv36ib7czoYbO3sNokmZC5a9wTDkr3d2HOZBW4AWpiavWVtedfotDgowcA0/640?from=appmsg#imgIndex=0)

1. 1 拖进照片，说句"入库"

在任务栏把这张照片拖进去，输入「入库」两个字，剩下的 WorkBuddy 自己干。

![](https://mmbiz.qpic.cn/mmbiz_jpg/95icgMZNPWIrYkgNOYxLibx7V5J5kcoXuArFeEw6Sge7mvTHQut3MovE4ysCIqDUQlvdQZfxJfQ16mibzehEicvoweLN3nF3IVdZJQID7iay8Qias/640?from=appmsg&amp;watermark=1#imgIndex=1)

它干了几件事：把原图存进 原始题/；生成一份整理页放进 整理后题目/；往 错题总表.html 里追加一行；再依据原题出了 3 道类似题。

整理页长这样：

![错题整理·八年级1｜正确答案 0](https://mmbiz.qpic.cn/mmbiz_jpg/95icgMZNPWIquf9qmQ6gicic9NaAC1jZ2XneFR76aa47hWWMlhAYgIL4ADL8sCm1rUDlllh0D0Es2prr1aWiaysaAPxWpOzcG1gVLnuvia96jSKY/640?from=appmsg&amp;watermark=1#imgIndex=2)

*错题整理·八年级1｜正确答案 0*

你看，原题、正确答案（这道题算下来是 0）、错因、知识点都列出来了。我的答案（错的）那一栏是空的——因为照片上孩子没写过程，我就没给，按规则它老老实实留空，没有瞎编。下面三道类似题，数字换了、考点还是二次根式化简，难度也没降。

1. 2 错题本模块：一眼看薄弱点

点开「错题本」这个 tab，所有错题列成一张表，还能按错因、按知识点做统计：

![](https://mmbiz.qpic.cn/mmbiz_jpg/95icgMZNPWIpfZ8oHfuCUWGWArdae1062S15TN7EXjsrDkjqk20eCRL899fJSUo3IfC1XU3sGH2vtic2cFq3oVOYZh5hyzia07ErMBL4dH5HwI/640?from=appmsg&amp;watermark=1#imgIndex=3)

我最看重的就是底下那两条统计。哪类错因最多、哪个知识点最弱，进度条一拉就清楚。辅导孩子的时候，直接往薄弱的地方使劲，不用瞎抓。

1. 3 随机抽测：遮住答案自测

「随机抽测」只给你看题目，答案藏起来。让孩子先做，做完点"查看解析"才出答案：

![火山错题本·工作台｜③ 随机抽测](https://mmbiz.qpic.cn/sz_mmbiz_jpg/95icgMZNPWIpsXJjkbcfhjHGKRkXib6UxYSrWWyWWiaWYibsibu381qZI1cPMoKWibYsKJYV9Fjjicf0k9XGor5iag2J6vLXnN6mrDtQJA6Ky0Xe99E/640?from=appmsg&amp;watermark=1#imgIndex=4)

*火山错题本·工作台｜③ 随机抽测*

这个功能专门对付"看着答案觉得会，自己一做就废"。

1. 4 类似题练习：换数字练手感

「类似题练习」里选一道题，下面就把它的 3 道类似题列出来，同样先不给答案：

![火山错题本·工作台｜③ 随机抽测](https://mmbiz.qpic.cn/sz_mmbiz_jpg/95icgMZNPWIpOGp11ghLIr3xzIMiavbpdRl4HxD6tqqKuyMIPey64LRsNwqHRrWCsuVBz0qyibRtDoQHTPV4dBpHVralnV0Jd0oSVjlPCoQryw/640?from=appmsg&amp;watermark=1#imgIndex=5)

*火山错题本·工作台｜③ 随机抽测*

孩子把同一类题练熟了，下次再遇见，手感就来了。

1. 5 入库页面：没照片也能手动录

前面说的都是"拖照片进任务栏、说句入库"。但其实这个「入库」页面本身，也支持不用照片、纯手动录题。

打开「① 入库」这个 tab，上面一栏是"最新入库的题目"，下面就有个「增加」按钮。点一下，弹出一个表单：原题、我的答案（错的）、正确答案、错因分类、涉及的知识点，自己一项项填进去，点保存就直接入库了。

![火山错题本·工作台｜③ 随机抽测](https://mmbiz.qpic.cn/sz_mmbiz_jpg/95icgMZNPWIpTMgkcY9iciaUb50cU1DjqMh9v2U0SFDPpze7WNzqmlnJYJ2b609aiaZ3FssMMQ9sGZybT2ZCicYU0csjevz6JHNT7UHTccNd6FXM/640?from=appmsg&amp;watermark=1#imgIndex=6)

*火山错题本·工作台｜③ 随机抽测*

它走的是和拖照片一模一样的整理逻辑——照样会生成整理页、往总表里加一行、顺便出三道类似题。上面那张图，上半部分是"最新入库题目"，能直接编辑再保存；下半部分就是点「增加」之后弹出来的手动录入表单。

说白了，拖照片是给"懒得打字"用的快捷入口，手动录入是给"想自己整理"用的。两种方式最后都归到同一个错题库里，数据互通，互不影响。所以哪怕哪天孩子把卷子弄丢了，你凭记忆也能把题补进去。

## 四、这只是"能用的简单版"。
说实话，上面这套就是为了赶在期中考试前，先有个能用的东西。它解决了最核心的痛：错题有人整理、有地方存、能统计、能自测、还能举一反三。

但要说方便，还差得远。比如：

- 多设备同步：现在数据全在本地电脑，手机上看不了。以后可以接云存储，电脑整理、手机抽测。
- 按章节 / 日期分类：题多了以后，得能按单元、按考试筛，不然就是一团。
- 导出打印：老师有时候要纸质版，能一键导出 PDF 就好了。
