---
title: "WorkBuddy 新挖到一个狠活 Skill：PDF 不只是能读，连结构都能拆"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/375"
type: "skill"
chars: 3253
sections: 0
figures: 0
chapter: "07-我要处理文档"
---

# WorkBuddy 新挖到一个狠活 Skill：PDF 不只是能读，连结构都能拆
![](https://mmbiz.qpic.cn/mmbiz_gif/gX9JE5tiaI7ibWWVA1RARlHw5jnibnfd6JGic5gARmlWo6uUAWD1ibWdqOWynFaJMcVWXw42637bhaKOybTxQgib4DEQ/640?wx_fmt=gif#imgIndex=0)

现在把 PDF、研报、财报直接丢给 AI 已经很常见了，但我最近碰到的一个任务，让我发现真正麻烦的其实是更前面那一步。

我手里有一份 11 页的人形机器人研报，后面不只是要让 AI 总结内容，还准备继续做 PPT、重排表格、提取图表里的数值。直接读文字并不难，难的是怎么先把这份文档拆得足够完整：表格不能散，图表里的数字不能只剩在图片里，阅读顺序也不能乱。否则第一步少掉一点结构，后面越处理越麻烦。

![](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyDPVMf8WiaR22jmE7zBBibkAwl8CUSJ39YUtzfUfu1U00cRvWlPWvytZHvmL5Lk0wlBCiaT292Ul3sL8qhLl71GtB4yafEct0WonM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

我在 WorkBuddy 里翻连接器时，正好找到 TextIn xParse，看起来和这个需求很对路，就直接安装上了。

![专家·技能·连接器｜应用·灵感](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyDehvaViaOA30ZiaMESexSOgWt7lrTYIkTJvqIYBosZMhiaHTwVyl4mDqkic79vib0Q7QkxZpMY0GcjGO6yX9CurngibJicHw5IiaPcVJ8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*专家·技能·连接器｜应用·灵感*

然后我就拿这份研报试了一遍。结果比我预期更有意思：196 个内容块、5 张表格、7 张图表、20 张图片都被拆了出来，图表里的数值也能继续拿来处理；后面即使换了不同的 PPT 生成方式，这些已经解析出来的结构化数据仍然可以继续复用。

如果你的文档后面还要继续交给 RAG、Agent、知识库或者数据分析流程，这种“结构保真”能力，比单纯把字识别出来重要得多。

先说 TextIn xParse 是干什么的。它不是简单把 OCR 再包装一层，而是一套面向复杂文档的解析服务。OCR 更接近解决“这里写了什么”，xParse 还要继续处理“这段是什么、先读哪里、表格怎么排、数字属于哪个单元格、图表里的数值对应哪条轴”。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyBfLEGPL5uHesLA1qPh3vp6JeKVVZQmqpVWE7X95sBgDibdCg14qxIadXaS5RQamCoMwRVic5ngJVn7Ao8tjoyXfErVMkr8icnGg8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

对普通用户来说，这个差别其实很好判断。

如果只是从图片里找一个合同编号、发票金额，普通 OCR 可能已经够了。但如果要处理财报、研报、论文、招股书，后面还准备接 RAG、Agent 或知识库，那就不能只拿到一串文字。表格关系、标题层级、阅读顺序、图片和图表数据，最好一起留下来。

WorkBuddy 本身可以读取普通文档，但遇到扫描件、复杂排版、跨页表格和图文混排时，真正难的是把原来的结构关系保住。文字即使识别出来，段落顺序、表格逻辑、图表和说明一旦散掉，后面的 AI 处理就容易出错。xParse 在 WorkBuddy 里补的，正是这层复杂文档解析能力。

![解析PDF并转换为markdown格式｜中国企业社会责任调查报告.pdf 解析这份pdf并转成markdown格式](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyCIcdKhvgelURQUUWsdP1icncvcZt61sylKuejylnqcElQhhwcHuLlsiap763bCJeLRVHSx9ghH9QJ7nH4Viacwc07E5QZzDeD8iag/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*解析PDF并转换为markdown格式｜中国企业社会责任调查报告.pdf 解析这份pdf并转成markdown格式*

TextIn xParse 官方支持 PDF、Word、Excel、PPT、图片等多种格式，可识别文本、表格、图片、页眉页脚、公式、公章等 16 类内容元素，还能处理标题层级、跨页表格、阅读顺序和图表数值，最终输出 Markdown 或 JSON，支持 50 多种语言。

![专家·技能·连接器｜资料库·灵感](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyCPCyKjKBibYtxOjoBCYxbHSbbTVBibKYOxUd8Ig8K8n8C7jnUzBZtgSBXkHqrS6siaicH9nAG98iaevKFFd6R4RCVYlQrZxI54DOrQ/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*专家·技能·连接器｜资料库·灵感*

官方给出的性能口径是百页级 PDF 约 2 秒完成解析，并披露了 1000+ 企业客户、累计处理 10 亿+ 页文档等规模数据。这些属于官方信息，我没有逐项做独立压测；这篇文章真正想看的，是它在一份复杂研报上的实际表现。

这次我没有单独写调用脚本，而是直接通过 WorkBuddy 里的 TextIn xParse 连接器来用。

这里的接入方式比我原本想的还简单。推荐直接走 WorkBuddy 的「连接器」。登录 WorkBuddy，在左侧「连接器」里找到 TextIn xParse，点「+」添加，完成直连后就可以直接调用。

![专家·技能·连接器｜腾讯健康全周期管理平台](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyCEHYlquaE7J4BXUtyutkektPnEUOM567ala6cU1ewCONVnyibT46E7GEQKuPxth4GqMyXAVl6eTeKkTI5xUibU93nOJ34Q7p9Mg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*专家·技能·连接器｜腾讯健康全周期管理平台*

TextIn 在 WorkBuddy 上架时公布的政策是，WorkBuddy 用户可获得每日 1000 页解析额度。

添加成功后，使用方式就很接近普通 AI 对话了。我这次给的指令很直接：把这几张 PPT 照片解析成结构化内容，保留表格、图表数值和阅读顺序。

![专家·技能·连接器｜应用·灵感](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyAJOLic5X1STz3fJeKicUcW7bJSSF7fCDia5xs7zz3rbgbuhylJUBIfxdHdhIuBgLicOSibgVjZxEBneSUGsNoeeDoTPDqWsWURar14/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*专家·技能·连接器｜应用·灵感*

![专家·技能·连接器｜应用·灵感](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyC2gSxXt4xpJzcLInM7AiagtQib5lBUende5uaptetTiaJQ6UyxHdxd9pGI65FPde6jng6cMIiaUa63ZSqia3DYTj7DFcLFjD7Exau4/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*专家·技能·连接器｜应用·灵感*

背后调用的是 xParse 的 pdf_to_markdown 解析能力。我保留了几个关键参数：parse_mode=scan、dpi=144、apply_chart=1。

这里面我比较关注的是 apply_chart=1。它让图表不只是以图片形式留下，还会进一步尝试提取其中的数据。这一点对后面的 AI 流程很重要，因为“能看见一张图”和“能拿到图里的数字继续计算”，完全是两件事。

实际跑完之后，PDF 正常解析完成。

![解析书版数双周报PDF为结构化内容｜交付物(位于 textin-parse/output/):](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyD4ibyAuQbcvn5GSAnWgdImCKuXB3BL5DibfJ5AHVu6ibiasH64LMqsYD5SicuF82t3O01Dn1ict2HkQgeiaWInyicI8YrKe7cegSrUZRw/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

*解析书版数双周报PDF为结构化内容｜交付物(位于 textin-parse/output/):*

这份 11 页研报最终得到 196 个按阅读顺序排列的内容块、5 张表格、7 张图表和 20 张图片。

正文顺序基本保留，标题层级可以从 outline_level 这类结构字段里继续拿，图片和图表对象也会单独存放。后面做重建、检索或者多模态处理时，不需要再回 PDF 里重新裁一次。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyDy2ia9HJvG1m0l4Lcd8MteCjzM3iaXMTXz2ficJZyM1NmexT7icASDnYqvmx9ulgkCpI4bedn0EiciccEXelAxIrAumZWiatWmxeG7a0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=10)

真正让我觉得 xParse 有价值的，是图表和表格这两类内容。

普通 OCR 碰到柱状图，可能会把年份、百分比、标题都识别出来，但很容易只剩下一堆零散数字。比如 28.6% 识别对了，却不知道它对应哪一年、哪一根柱子，后面的 Agent 依然很难直接使用。

xParse 这次会把图表识别成 image(sub_type=chart)，同时继续抽取其中的数据，以结构化表格形式放进返回结果。也就是说，一张图进去，出来的不只是图片，还能拿到一份可以继续查询、计算和校验的数据。说实话，这让我非常震惊。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyC9BD12Jzx5AUctHleG933Ff14CPaOibXSjqVy87E3HO2XIGrJZQDnIVpTYL6IS7dl7FlHo9ibqicVzptRhte2bwneic1bzWzHNxSs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=11)

这一点很适合 RAG 和 Agent。

因为模型真正需要的通常不是“我看见这里有一张图”，而是“这张图里 2024 年对应什么数值，和 2023 年相比变化多少”。如果前面的文档解析没有把这些关系保住，后面的模型再强，也只能在残缺输入上做推理。

表格同样如此。

这次样本里有一张 43 行×13 列 的重点公司市场表现及估值表，宽度和数据量都不小。对这类表，我最关心的不是某个数字有没有识别出来，而是行列关系有没有保住。

![](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyCsl0U3s0pFFu6Gd5T0R3tg51zPU1IxCXZicIpuG6xU4WwnlRrXG6FUZOlpxRDWebJx4W3INLv4SDg4G0xV5LD7LM7HSP9kIDPo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=12)

例如“815.39”这个数字本身识别对，并不代表解析成功。它还必须继续属于原来的公司、原来的指标和原来的列。表头错一列，后面所有数字都可能看起来没问题，但其实已经全错位了。

这也是 xParse 和普通 OCR 最明显的区别：它交付的不只是文字，而是带着结构关系的内容。为了看清这种结构化结果到底有多大用，我后面又走了两条不同的 PPT 路径。

第一条是直接做 PDF 转 PPT。这个环节调用的是另一项文件转换能力，不属于 xParse 本身。转换后正文和大部分普通内容都还在，但那张 43×13 的超宽表没有完整保留下来。

![](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyDFBBCHUcszlRoPmxMazO5UXUbUQTzwicdzicontwbicxObSMdOOrq1hNTEqfWWoVmLrbsPkbqQkcNKibAptibk4lolQF7ic7g9Jicqow/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=13)

我一开始以为，是不是前面的解析也把表弄丢了。

回头去查 xParse 输出的 raw_result.json 才发现不是。整张表的单元格数据还完整保存在解析结果里。

这件事反而让我更直观地感受到结构化解析的价值。

因为后面的文件转换环节即使出了问题，只要前面的结构化数据还在，就还有恢复空间。我最后直接从 xParse 的解析结果里读取这 43 行数据，用 python-pptx 把大表重新构建成原生 PPT 表格。

重建之后，我又挑了几个关键值做反向校验：拓普集团市值 815.39、绿的谐波 PE 298.45、三花智控 1,483.22，以及原表里的 #DIV/0!、斜杠等异常值，都还能从原始解析结果中找到。

![](https://mmbiz.qpic.cn/mmbiz_jpg/GWLeL0AYCyAtnzU6fwo7fBYz2hm7yC7d3V4U71oJW2Q0Xefc8kezMamEKRZy3wKyKBJuqeMFI5qc1agSUBwzEHuXbWVwxAO0zeJFu2MiaKjw/640?wx_fmt=jpeg&amp;watermark=1#imgIndex=14)

这里有个小细节我挺在意。

#DIV/0! 看起来像“脏数据”，但源表里本来就是这样，解析器就应该先忠实保留，而不是自作主张帮你修掉。对文档解析来说，保真往往比“看起来更干净”更重要。

然后我又试了第二条路。

这次不再使用前面的 PDF→PPT 转换能力，只保留 xParse 第一次生成的结构化 Markdown，再把它交给一个普通的 slides 制作流程重新生成 PPT。

![](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyDbtauOXubofQyL5ZgoEyNl4aoC5s5RibnoosTGaGic3ZcCD41waDvO3y0zkMepYwHq5m6QhN4MRic3L3ULTbCoQyXhUMxKibMB5fw/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=15)

这条路径里，下游工具已经换了，但前面 xParse 提取出来的结构化内容仍然可以继续往下用。

![](https://mmbiz.qpic.cn/mmbiz_png/GWLeL0AYCyAEyBc4aeg8nbtocZAI9NXOFw016YsPH76uCtrrUcbBqfsDApqrFM70FJ94B2pxaPy1N5N3HIz9zQRibTLR6bicNib6T0fwf0hSfY/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=16)

比如原 PDF 里的营收、归母净利润原本都是图表。xParse 在第一次解析时已经把图里的年份和数值提取了出来，所以换成普通 slides 工具之后，这些数据不需要重新 OCR，就能直接重新组织成原生表格。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/GWLeL0AYCyCIOWGm8agNVFNMlCd8Siaiagx9z1UNtxXEqrpYezGba5ficL1hpY1oFliaESgyGIibk8RINWfXCTxEFjDwwicXRFRgESXZ37U3yvv8s/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=17)

原来那张 43 行×13 列的估值表也是一样。因为单元格数据已经在 xParse 的解析结果里，后面的 slides 工具可以根据版面需要重新拆页，原表中的公司、市值、涨跌幅、归母净利润一致预期、PE 等核心字段和数值都还能继续读取并重建。
