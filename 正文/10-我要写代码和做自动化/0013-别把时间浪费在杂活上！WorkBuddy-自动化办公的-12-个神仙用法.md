---
title: "别把时间浪费在杂活上！WorkBuddy 自动化办公的 12 个神仙用法"
source: "https://workbuddy.jiangyufan.com/index/hub/case/604"
type: "case"
chars: 3170
sections: 2
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 别把时间浪费在杂活上！WorkBuddy 自动化办公的 12 个神仙用法
WORKFLOW · 办公提效。2026.09。还在自己手动填发票、憋日报。别把时间浪费在 杂活上。WorkBuddy 12 个神仙用法。自动日报 · 热点推送 · 发票OCR · 会议纪要 · 多项目管理。

![](https://mmbiz.qpic.cn/mmbiz_jpg/rPECmo1WwDMmCXN1OFcXibOoM1bQoqAandlHOEbiazAcFIPAkpuIKVnY4Tfs9olKntkCl6HbRH9kwmRNG7ibcY5EFXF5jyFgHAHUcZhu9bw1g8/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=0)

WorkBuddy 自动化办公实战指南。保姆级教程 附提示词。

最近翻到一份官方整理的办公提效案例库，里面汇总了大家用 AI 接管日常杂活的实战套路。我顺手在 WorkBuddy 里照着复现了一遍，发现只要配合它的技能和自动化任务，全部都能直接跑通。

这些场景来自真实打工人的日常，覆盖日常汇报、信息搜集、发票处理、会议纪要、多项目进度管理。这篇就带你逐个过一遍，顺便把在 WorkBuddy 里怎么让它在后台替你干活这件事讲清楚。

每个用法后面我都附上了开箱即用的指令提示词，你可以直接复制到 WorkBuddy 里跑，或者存进定时任务。

## 怎么在 WorkBuddy 里把杂活自动化。
一共三步，很直白。STEP 01。找到或添加技能。在左侧找到「专家·技能·连接器」，点进去搜索需要的技能，或者直接找到「工作日报」技能添加。

![专家 技能 连接器｜我安装的 81](https://mmbiz.qpic.cn/sz_mmbiz_png/rPECmo1WwDP4pds1Dib1vn6BwC9oiaehicyibLfamDDkgJ0k0ic2c6rmZNhYIcOfA7ibtBSfRKNZf6ouVyWF2ib7icEyDDsNUqIB0A27iaiacoiaLs8Kkw/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*专家 技能 连接器｜我安装的 81*

— 找到对应技能，或者直接口述你的流程。STEP 02。配置自动化任务。

在左侧点进「自动化」，点击右上角「添加自动化」，给它定好名称、提示词（比如选工作日报技能，模型选 HY3 免费）。

![添加自动化｜专家·技能·连接器](https://mmbiz.qpic.cn/mmbiz_png/rPECmo1WwDPV9a5OjzaQKceIic2QibUyRleiaAJDbRk6Sfljqiako7S5lh6Cd2xBibQmWeWdahNw5icuaScJd4pZEiasl4Jj7FlGibXjhI4w1P9OTico/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*添加自动化｜专家·技能·连接器*

— 配好定时触发与提示词，不用天天催它。STEP 03。绑定通知并保存。设置好执行频率，并勾选推送渠道（比如推送给微信小程序或企业微信 bot），点击确定。

![发现应用√｜添加自动化√](https://mmbiz.qpic.cn/mmbiz_png/rPECmo1WwDORDO3CQNrS2u4NhjB9yYriavwLRjibwnv31fExcyf8L5jWoia9vS8ZshArb2icsyLk0oarbYURyeTuzR1qKLfQibMoPDlib9th15icWU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*发现应用√｜添加自动化√*

— 跑完自动推结果，你只管看成品。配好之后它就在后台待命。到点自动干活，你合上电脑或者去开会，它该跑的步骤一步都不会落下。SHOWCASE。

## 12 个高频办公神仙用法拆解。
NO.01。自动总结工作日报告别“周三忘周一”。打工人最怕每天下班前对着空白屏幕憋日报，周三就记不起周一干了啥，漏写了还容易被当成没干活。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/rPECmo1WwDOciaBqeicia4bE8Hqt0IhaQxH7toekUMLHKLDebzPPDaGI2ZEfM6KicZDeuuupvtpQhocbwt8n3AicxNia4WgGcnwncokJqKLFfwyNU/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=4)

— 一句话生成清单 + 每天定时自动汇总。

- 来源：迟迟（医疗行业全栈开发）
- 它解决什么：每天下班痛苦回想做了啥，容易遗漏关键成果
- 适用场景：个人工作记录、每日日报汇总、周五周报一键合并
- 亮点：固定读写同一个文件，提示词不用变，自动闭环记录与推送

指令 A：周一生成本周任务清单（写入桌面固定文件）。. . . prompt。读取我口述的内容，为我生成一份本周工作任务清单：

1. 开发 PACS 系统改造，先对接厂商 A 设备，再推广全院区。
2. 优化现有的 CRM 体系，重点改善 APP 端录入卡顿。
3. 公众号增加 AI 对话助手，导入客服知识库。
4. 小程序增加分销裂变专属分享页，统计转化数据。

- 结构清晰，包含【本周目标】、【每日计划】、【优先级（P0/P1）】和勾选框。
- 写入桌面固定文件路径：`~/Desktop/本周任务清单.md`。

指令 B：设置每天 22:00 的日报自动汇总（配置到自动化任务）。

读取 `~/Desktop/本周任务清单.md`，检查今天标记为已完成（[x]）的事项，并结合今日代码/文档修改记录：

1. 汇总为一份结构化的工作日报，分为【今日完成】、【推进中卡点】、【明日计划】。
2. 保持语言精炼、结果导向，带有量化成果。
3. 生成后追加到 `~/Desktop/本周任务清单.md` 的底部【每日总结】区域，并触发机器人通知到我的工作群。

NO.02。定时推送 AI / 行业热点每天上班直奔重点。想每天跟进圈子里的新动态，但自己去刷论坛、推特又极度碎裂，一不小心就摸鱼半小时。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/rPECmo1WwDNknib0tRRDx66QVg7ggrKoBiaTPRbcdWMDfiaysIzpXlqpSBOpKPXEOGicdEyicICaI6Vg09UmYZJvqnJ74ibblvJhxicibqYPEgwI4Uk/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=5)

— 后台自动联网巡检，提炼核心干货。

- 来源：Oh_my_God_L_C
- 它解决什么：手动刷资讯耗时耗精力，容易分心耽误正事
- 适用场景：AI 圈动态跟进、竞品资讯监控、行业早报制作
- 亮点：每天只需 2 分钟扫一眼群消息，全网重点尽在掌握

提示词参考：每天 08:30 自动巡检推送。作为行业情报分析助手，请执行今日资讯巡检任务：

1. 联网搜索并浏览过去 24 小时内关于【AI 应用、大模型、办公提效】的高热度讨论（优先关注官方技术博客、Hacker News、主要开发者社区）。
2. 筛选出最具技术价值或业务启发性的 5 条新闻/动态，坚决过滤纯公关通稿与标题党。
3. 按照如下格式整理输出：

- [核心事件标题]
- 核心看点：用 1~2 句话讲透本质与突破
- 对日常办公/开发的启发
- 原始出处链接

1. 整理完成后，推送到预配置的钉钉/飞书群机器人，标题注明：【今日 AI 要闻内参】。

NO.03。批量开具与上传发票月底报销救命神器。月底财务报销，几十张订单需要逐个登后台开票、下载、改名再传到报销系统，纯粹是消耗人生的机械活。

你把包含订单号的表格甩给 WorkBuddy，它在后台调用浏览器自动登入开票后台，批量填单、获取 PDF，再按「日期_姓名_金额」规规整整地改好名，最后批量传到报销系统。

![](https://mmbiz.qpic.cn/mmbiz_jpg/rPECmo1WwDPkhV1nXvU9tGficuIp1yy0vvEMdXHNRSn71bxDibX6wH0TZvO3923mI56UiaM4zjjxgpRAhKcfDFcjYQ7N4Siclf1SUY2WJxgwCicw/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=6)

— 自动登后台、自动开票下载并重命名。

- 它解决什么：枯燥重复的网页表单点按与文件重命名
- 适用场景：月底集中报销、客户批量开票、电商订单发票开具
- 亮点：把一个小时的手工点按，变成点一下之后去冲杯咖啡

提示词参考：批量驱动开票工作流。请读取本地表格 `~/Desktop/本月待开票订单.xlsx`，按顺序执行批量开具与归档：

1. 打开浏览器并访问发票服务后台系统（已登录状态）。
2. 遍历表格中的每一行记录（订单号、抬头税号、金额、项目类别）：

- 自动在开票表单中填入对应字段并提交；
- 等待开票完成，下载对应的电子发票 PDF 文件到 `~/Desktop/发票暂存/`。

1. 批量对下载的 PDF 文件进行规范重命名，规则统一为：

```
开票日期_购买方名称_金额元_订单号.pdf`。
```

1. 全部执行完成后，在界面弹窗报告处理结果：共成功开具 X 张，失败 Y 张（若有失败记录给出具体订单号）。

把这些零散素材全部打包扔给 WorkBuddy 的会议整理技能。它会自动剥离废话口癖，对齐不同人的发言观点，提取核心结论，最重要的是把待办事项（Action Items）按负责人和截止时间清清楚楚列出来。

![](https://mmbiz.qpic.cn/mmbiz_jpg/rPECmo1WwDObmWUcRFVfzRxOYomu0zxvU2XUCq94ew9ZXBicfhIFcmcD7ic5F4Mjp127DWibugnJ3oPpoY1SOL8ZhkM7ZIouEicBib3ECvbATQlY/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=7)

— 零散素材一键变成带责任人的结构化待办。

- 它解决什么：会议材料散落各处，梳理纪要极度费脑耗时
- 适用场景：项目碰头会、跨部门评审、头脑风暴讨论整理
- 亮点：发言人观点对齐 + 待办任务精确排期，发到群里领导挑不出毛病

提示词参考：零散会议材料结构化清洗。以下是我刚开完的项目碰头会的杂乱素材（包含现场速记片段、群讨论记录与白板文字识别）：[粘贴或附上你的会议零散文本]。请帮我整理成一份严谨、专业的【会议纪要与行动看板】：

1. 提取基础信息：会议主题、时间、参会人。
2. 提炼【核心共识与决策项】：用精炼商务语言列出达成一致的关键决策，剔除扯皮与客套话。
3. 梳理【待办事项清单（Action Items）】：必须以 Markdown 表格输出，字段包含：序号、任务内容、负责人、交付标准、截止时间（明确到具体日期）。
4. 整理完成后，另存为 `~/Documents/会议纪要/2026-XX-XX_项目评审纪要.md`。

NO.05。后台持续处理长任务不用再盯着进度条发呆。

有些活动辄跑半小时以上，比如批量转几百张图片、清洗海量杂乱表格。普通 AI 对话框经常超时断掉，报错了还得重头再来。

依托 WorkBuddy 的长任务执行机制，它在后台按步骤独立跑，每一步都有执行和检查机制，遇到偶尔的报错会自动重试。你尽管去开会或者干别的，全部跑完它会主动给你发一条回执。

![](https://mmbiz.qpic.cn/mmbiz_jpg/rPECmo1WwDMicBMa7TXDeY74ouDZADUutXS9qRPUZHeNGLyBIDKKvJUcuia9mzNgosicO1ibeby4laoPgwiaaNjqxeu9OKdBpPxALzVMd3V1vkOo/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=8)

— 自主分步推进，后台静默执行不卡顿。

- 它解决什么：长流程任务耗时长、容易中断，需要人肉盯盘
- 适用场景：海量数据清洗、批量文件格式转换、长链条自动化爬取
- 亮点：长任务托管机制，合上电脑也能跑，彻底解放注意力

提示词参考：长任务分步托管模式。

我需要对 `~/Documents/RawData/` 目录下的 300+ 份杂乱 CSV 数据表进行批量清洗与重构，这是一个耗时较长的长任务：

1. 请进入自主执行长任务模式，分批次处理，每批 30 个文件，记录各批次的执行日志。
2. 清洗规则：
