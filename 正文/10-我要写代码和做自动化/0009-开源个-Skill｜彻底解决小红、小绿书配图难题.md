---
title: "开源个 Skill｜彻底解决小红、小绿书配图难题"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/348"
type: "skill"
chars: 3339
sections: 2
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 开源个 Skill｜彻底解决小红、小绿书配图难题
![上线基本空调｜上线最大空调可以显示](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DW5olXdhQoFySLPSzHzVDYUr8NiaxGf5bicChSAkft0puc8RArOGvwmKXgTmtw1lIPbBtMQibHMfjreia7LS3cpeRrDsXaylpDYoAs/640?wx_fmt=png&amp;from=appmsg)

*上线基本空调｜上线最大空调可以显示*

前段时间开源了 guizang-ppt-skill，之后我自己用它做内容的时候发现一件事。用它出的网页，单张截下来发到图文平台，反响和数据比我手工排版还很多。

![时间对比·达成 10,000 STAR 所需天数｜藏师傅的 PPT Skill 突破 1 万 Star 了!](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DVmNsiamv3f23mx3QCW9z7wNlvK4ZIKGWz7rWQktHtShfEI0gbdxxmbkpkLexR9e7STLVL0eQYjw7Zgicr2UADxAiae7vZYwlwEgY/640?wx_fmt=png&amp;from=appmsg)

*时间对比·达成 10,000 STAR 所需天数｜藏师傅的 PPT Skill 突破 1 万 Star 了!*

我相信你之前也找到过一些这种生成3：4 卡片图的提示词或者 Skill。他们几乎都是一个味道：Tailwind + 大色块 + emoji 堆砌 + 中规中矩的字号层级。看完之后，我大致能理解为什么 AI 出的图文卡片那么容易被一眼识破，它们做的是网页，不是杂志。

它们做的是网页，不是杂志。图文卡片对比 PPT 完全是另一种生物：竖屏、信息流里 1 秒钟决定停不停下、靠图说话而不是靠字。版式不同、节奏不同、读者不同。

下面讲讲它好在哪、我为什么愿意在它身上花这么多时间。

## 二、到底好在哪里。
先把目标说清楚：3:4 竖图是图文卡片的主战场。这个 Skill 的绝大部分设计精力都在 3:4 上，字号层级、版式比例、断行规则。全部按 3:4 在手机信息流里被滑过的真实场景校准过。21:9 和 1:1 公众号头图也都支持。

![小红、小绿书彻底解决小红、小绿书配图难题｜在稻城看见cinter](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DUEk4uHsNZn3icRSsyybdIkx569TvLNGQfMUBibGuScgLW1LAxF7JB0pmH4velmjdkRud69O6VLN1Xp74plLALXXgicKA8hZNlbQs/640?wx_fmt=png&amp;from=appmsg)

*小红、小绿书彻底解决小红、小绿书配图难题｜在稻城看见cinter*

下面从图文创作者最关心的事开始讲。

1. 1 它分得清你在写什么，然后用对的方式去配

图文平台上的内容是分门类的。一篇影评和一篇产品测评，需要的视觉语言完全不一样；一篇旅行散记和一篇职场干货，该用的版式也不是同一回事。但绝大多数 AI 工具不管这件事，你写什么内容它都用同一套模板套出来。结果就是所有人发的卡片都长得像一个公众号的封面流水线。

这个 Skill 内置了 11 个常见图文品类的适配规则：旅行 / 生活方式：杂志风为主，暖色板，大图压全屏，衬线大标题；职场 / 干货 / 商业洞察：网格风为主，深色背景，数据大字报版式；影视 / 文化：偏冷色调的杂志风，电影海报式版式，人物特写优先；

产品测评 / 数码：网格风，对比矩阵，设备框美化截图；读书 / 笔记：杂志风，衬线字体，引文居中版式，留白拉满；美食 / 探店：高饱和杂志风，俯拍图优先，文字向四角让位；

![创业的第三年 things｜“如果你做的事情没让你怀疑自己，那它大概也没让你成长。"](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DXdTqW0jNUFoQ7LL1a3UXL4gKTIiaMQUXYD8VHb4GfNFVKkZxKGQY21o9PQuibDlG8ogXgicYNQxv1t1YWWQN3aITY91NmRiagl3NM/640?wx_fmt=png&amp;from=appmsg)

*创业的第三年 things｜“如果你做的事情没让你怀疑自己，那它大概也没让你成长。"*

我甚至专门为旅行博主做了地图组件。你可以把店的位置和旅行路线都标注在上面，AI 会自动帮你生成标注。

![下午从北往南走｜VOL. 02 · OVERVIEW·京都全图](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DUr3rHpY2N108O9icMAYTK0oCiaI7DGP1eXaKnqyzBX1fNTNoiaibzKqCmI0Tia3hAKYUqSXicVweWhfSuic1U2PGpyvn5WMV2lupuIYM/640?wx_fmt=png&amp;from=appmsg)

*下午从北往南走｜VOL. 02 · OVERVIEW·京都全图*

同一段文字喂给它，你说这是影评，它给你电影海报式的卡片；你说这是产品测评，它给你带设备框的对比图。

![同一段文·两种品类｜云岚法桐午后](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DVmMekTDaQmQ8IWZbT07lGTCsagUMniaKucRWAfhbYUDXjPLxQicx7JHz1Mfcl8yvibub7bOCWUxhYrYIic9DKiaNwnvd1bVZU0vvLw/640?wx_fmt=png&amp;from=appmsg)

*同一段文·两种品类｜云岚法桐午后*

更重要的是，它有明确不接的活：追星粉丝向，需要的视觉语言完全是另一脉；纯促销硬广，违背它强调内容性的设计哲学；超过 12 屏的长教程，图文形态不是长教程的最优载体。碰到这些场景，Skill 会在开头就告诉你"你可能想用别的工具"。

这是我故意留的。能力边界比能力本身更能定义一个产品，一个什么都能做的 Skill 最后通常什么都做不好。

一个什么都能做的 Skill，最后通常什么都做不好。

1. 2 文字怎么压在图上，这件事我啃了很久

文字压图是图文卡片里最难的一件事，也是最容易暴露"AI 感"的地方。压不好就会出现三种翻车：1.。文字盖在人脸或产品中心位置上。2.。白字压浅色背景或黑字压深色背景读不清。3.。文字横跨整张图把本来好看的构图毁掉。

![三种典型翻车样态·文字压图反例｜今日新品上市](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DX73RM6WJXJZCQshDSjDQhFRzicoeBXjUxup1WDWnkhd8XgVFS7WibqwricNS1biascMVd7JjzJiaRBD02DSz2xTc6J9KT85gfzYlX8/640?wx_fmt=png&amp;from=appmsg)

*三种典型翻车样态·文字压图反例｜今日新品上市*

Skill 处理这件事用了三步：识别图里的主体：人脸、产品、文字密集区，版式上自动避开；算落点区域的色和明度：决定字色、要不要加蒙版、阴影该多深；字号和断行自适应：根据落点区域大小动态调整字号和换行位置，而不是写死字号让它溢出。

![Skill落字三步法｜识别主体·划安全区](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DU2Lk01cJiaiak1aTDEicrGJwUPBiar8GdEtbNYX2fpqRRgU7dOTK1kGibaBMGOlblIuDrMmMfqKTAJWicq5Y2RhNbxQRVTcwg8yMRbw/640?wx_fmt=png&amp;from=appmsg)

*Skill落字三步法｜识别主体·划安全区*

这套规则跑下来，卡片的"高级感"基本就立住了。读者看不出"被压上去的字"和"图本来就在那里的字"的区别。

1. 3 图片从哪来：这是和市面上 AI 卡片工具最大的差别

绝大多数 AI 生成图文卡片的工具，要么让你自己上传图，要么用 emoji 顶替，要么生成一些一眼 AI 的插画。

结果就是手工补图很累，或者堆 emoji 显得很假。这个 Skill 默认接入了三个免费可商用图库：Pexels，支持中文搜索，大众化场景够用；Unsplash，摄影质感最强，人物、生活、空间类内容首选；Wallhaven，游戏、摄影、壁纸之类的图都在这里，版权混乱。

![别再用 emoji 1硬凑配图｜这个Skill会按正文语义去图库拿真实照片,裁切到版式里,并把来源和版权风险交代清楚。](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DUSu6weuVCNYJIgXicjsGeMntwtG4hctCLibB56eK3Fvh0aBrjAzib4dZmO0AiayDR6SsFEuGbXTS287Qp00HAicDo5BJI1tUfBibRto/640?wx_fmt=png&amp;from=appmsg)

*别再用 emoji 1硬凑配图｜这个Skill会按正文语义去图库拿真实照片,裁切到版式里,并把来源和版权风险交代清楚。*

它会根据正文段落的语义自动派发搜索词、拿回图、按版式裁切到位、避开人脸或主体被切掉。你拿到的是一张配了真实摄影图的卡片，而不是一张色块卡片。而且它也不会死板地去寻找绝对没有版权问题的图。能拿到的图都会告诉你，由你自己来判断要不要放版权不明确的图片。

另外，现在各个平台对 AI 带水印的问题管得很严。

目前你用的大部分 AI 生图都会有水印，而有水印就会被平台标注，一旦被标注就容易被限流，这是大家非常困扰的一个问题。

1. 4 截图也是图：四件套美化

我们的很多内容用不了摄影图，得是软件截图、聊天记录、产品界面。Skill 内置了一套截图美化：

加 macOS / iOS 风格的设备外框（browser chrome 或手机边框），用不同材质的背景托住截图，格纸、点阵、暖白或深色，让截图不再白底飘在白底上；

同时根据视觉风格自动匹配阴影层次和圆角参数，两套风格各有一套截图配方，前后一致不用手动调。

![把原始截图当成普通图片放进卡片。底层页面残留，边缘比例和截图自带留白，会一起进入最终画面。｜截图美化之后](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DWjFGDZ4OUtIiaHEVHbaqSesd69rfoV8pYt9FKYjwpuqVo28xXddSiaFGic3Nibth82YA0nOXmrBRS0Z1ibNdUZ29JibWIicbBFibQRiaGw/640?wx_fmt=png&amp;from=appmsg)

*把原始截图当成普通图片放进卡片。底层页面残留，边缘比例和截图自带留白，会一起进入最终画面。｜截图美化之后*

简单一句，你随手截的图，过它一道，看上去就像产品官方做的宣传图。

1. 5 AI 生图：克制地用

只有前面所有找图渠道都拿不到合适素材时，Skill 才会调用 AI 生图。生图时会强制带上风格约束词，避免出现"一眼 AI 插画"那种平庸视觉。我宁可它少用 AI，也不想它把 AI 用成那个让所有图文卡片长得都像姐妹的元凶。也避免你使用 AI 图片导致内容曝光受影响。

![典型反例·OVERUSE｜一眼 AI 插画](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DWicOkX2HolrnY2H0ArdoqKOFntfKaR6g7pfqsuW2us4q2jAtuq8dVDKKAXSq11wA209nm1bD2eJoOaABl8JibBATmnPgeoVHTwg/640?wx_fmt=png&amp;from=appmsg)

*典型反例·OVERUSE｜一眼 AI 插画*

1. 6 视觉系统：两套风格 + 28 个版式骨架

熟悉我之前的 PPT 的人会觉得眼熟。这两套视觉系统和版式骨架，是从 PPT Skill 那边沿用并重新校准过来的。我就不重复展开，简单说一下它在图文卡片场景下的样子。两套视觉系统：

杂志风：你在《The New Yorker》和上海译文社的封面上看到的那种排版。大留白，衬线大标题，版式不对称，文字有呼吸感。

网格风：Massimo Vignelli 和 Helmut Schmid 瑞士平面设计那一脉。强网格，无衬线，几何感，用色克制但精准。

![M09 - LISTENING / 周日早晨｜让Gould替我开始这一天。](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DWqo66URrU1lqJicdibCbpaeO9Mqnp3Y1tJNmNN5piahbj0GfLxPOkHuCbFRrjXTWGPSSJ12xeibH4OD58bJBCicwWmI87BBMricPF9A/640?wx_fmt=png&amp;from=appmsg)

*M09 - LISTENING / 周日早晨｜让Gould替我开始这一天。*

28 个版式骨架，是我从过去十年看过的杂志、海报、专辑封面、电影海报里挑出来，经得起放大看的那些。

AI 在"自由版面设计"上现在还是平庸的，给它一个被验证过的骨架，它的任务就从"设计"降级成"填充"，成品稳定性立刻上来。

10 套主题色板、固定字体搭配、有限图标库，这些细节就不一一列了。

![把手机扔进抽屉｜一天9小时屏幕](https://mmbiz.qpic.cn/mmbiz_png/ofWbZTuv4DVFoHmRSWWMDWC8MgqRGyeUu7RPuVrKuxtKFGrEKVvlxrCE8yMriaRMkGv07xvicNribkWaBdiaxncnicXslZ86sqQicyVnjTGibXny1g/640?wx_fmt=png&amp;from=appmsg)

*把手机扔进抽屉｜一天9小时屏幕*

它们的逻辑是同一个：限制不是阻碍，是底线。给一个内容创作者无限的颜色选择，他更容易做出难看的东西；给他 10 套被验证过的色板，他做出能看的东西的概率会接近 100%。

## 三、为什么要这么做。
1. 1 设计角度：杂志感非常有效

为什么走杂志风和网格风，而不是更"现代"的卡片设计?。图文卡片的本质，和印刷海报、画报、专辑封面是同一种东西。用一张静态图，在 1 秒钟里说服一个陌生人停下来。杂志和海报在过去一百年已经把这件事研究透了。网页设计语言是为可滚动、可交互的场景做的，搬到一张静态图上，会显得用力过猛、信息平淡。

![杂志感 vs网页感·同一张静态卡片｜安福路下午两点](https://mmbiz.qpic.cn/sz_mmbiz_png/ofWbZTuv4DXnBibswqUmkSRfyWrpornNOWnh8N6yYU0kia8mCNqb5BtniaIOxkIglN9upVZrkWWUziaIaibYOL8P4he724mUVk9BPH29jTxeI1TI/640?wx_fmt=png&amp;from=appmsg)

*杂志感 vs网页感·同一张静态卡片｜安福路下午两点*

所以这个 Skill 在视觉决策上的所有"为什么"：为什么大留白。留白是杂志告诉你"重点在这里"的方式；为什么衬线字体优先。衬线字体在大字号上有印刷品的重量感；为什么版式不对称。不对称会制造视觉节奏，让眼睛知道先看哪；

为什么用色克制。社交信息流里，克制的色板反而比饱和度高的更显眼，它和周围所有"喊得很大声"的卡片不一样。
