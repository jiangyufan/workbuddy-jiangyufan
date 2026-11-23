---
title: "我找到一个WorkBuddy省token的独家秘方！"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/710"
type: "tool"
chars: 2576
sections: 0
figures: 0
chapter: "09-我要省模型成本"
---

# 我找到一个WorkBuddy省token的独家秘方！
点击下方卡片关注「AI小白笔记」公众号。

话说前几天让AI帮我调整“每日AI资讯”Markdown文件的字体大小，折腾半天给我消耗了17个积分，这件事情让我耿耿于怀，后来研究WorkBuddy各个模型的优势和差异，写了这篇文章：别再Auto了，WorkBuddy选对模型既省积分又高效。

昨天又看到WorkBuddy里面让我很不爽的一个点：不管选择哪个模型，AI的思考过程竟然都是用英文表达出来的，请看截图：

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JeB8LAjhPIdSd35tlbLZEXjXZibJBUibYOPWiakAh80435tKC2UQtUdUNzXiaqYicmRAeOSEW2qicp07yjvrjvkgU2TyrpicjdpmMTqAdpwun1wIzs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

于是我的好奇心来了，明明都是国产大模型，为什么思考过程要用英文表达呢。于是我认认真真地去查AI思考过程会不会消耗token，不查不知道，查了吓一跳：AI的思考过程不但会消耗token，而且思考过程占token消耗量的比例非常高。

因为大语言模型本身是无状态的，它没有真正的 "大脑" 或 "记忆"。所谓的 "思考"，本质上是模型根据输入的上下文生成文本的过程。

思考过程可分为两个部分，第一部分叫显式思考，AI先生成详细的推理步骤，再基于这些步骤得出最终答案。这些推理步骤本身就是模型的输出，会被计入输出 token 消耗，这个过程用专业术语表达就是思维链（Chian of Thought，CoT）。第二部分叫隐式思考，即使你没有明确要求模型展示思考过程，它在生成最终答案前也需要进行内部推理，会产生大量用户见不到的推理 token，这些过程同样按输出 token 计费。

一个普通的任务，其自主思考与决策环节通常占总 token 消耗的30%-50%。AI接收指令后，它会自主拆解任务、规划步骤、评估方案，这个 "思考链" 本身产生的 token 甚至可能超过最终回答的 token 量。

一个复杂的任务，推理 token 的数量可能是可见输出 token 的3-5 倍。例如，Claude Opus 在进行数学计算和多文件代码审查时，推理 token 占比可达 75%-83%。

所以总结下来，AI思考过程的 token 消耗有几个特点：

1. 不可见性：大部分思考过程对用户是透明的，你只能看到最终的输出结果，但后台已经产生了大量的推理 token 消耗。
2. 比例高：推理 token 的消耗量可能是可见输出 token 的3-5 倍。
3. 占用输出配额：思考过程会消耗模型的最大输出 token 限制。比如GPT-5 有 128,000 个 token 的输出上限，一次高强度的思考可能会消耗掉其中的 80%，然后才开始生成可见的回复。
4. 失败也计费：即使模型的思考过程出现错误，或者最终没有完成任务，已经产生的推理 token 仍然会被计费。

既然这样，那么第二个问题就来了，思考过程用英文显示的token消耗量高，还是用中文显示的token消耗量高。

作为一个“牛人”（属牛的人），我脾气确定有点犟，又是一顿查资料，结果发现一个有趣的结论：国产模型用中文的token消耗量低，国外模型用英文的token消耗量低。

WorkBuddy内置的所有模型都是国产的，还等啥呢，一不做二不休，我立马通过提示词叫AI把思考过程全部改为中文。

![帮我把workbuddy的思考过程改成用中文显示｜完成了。以下是具体改动和说明:](https://mmbiz.qpic.cn/mmbiz_png/JeB8LAjhPIdMSNmz1OkyJ9wUDAA2pRZBShqBWibFGmB8QvCxSg9Ur2Lg89QgARdu6BWFZPfNokGwzb4X0sKcZYrbHiafYqe3gf5KdnXFJ7ye0/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*帮我把workbuddy的思考过程改成用中文显示｜完成了。以下是具体改动和说明:*

结果你猜怎么着。昨天改完了，今天惊喜就来了，我的自动化任务里面设置三个任务，看以下截图。

![codex知识入库 automation-2026-05-24-... 每天10:00｜每日AI资讯](https://mmbiz.qpic.cn/mmbiz_png/JeB8LAjhPIfG8oO3YLBJWQxtAEic0TdCuuqbT8wawkCXibk8NLyykhs8xficmcF5ySqUAdEC0pCArqXCsibAhiaJQezW6hwZpZiaXk2ZQdias5icaSc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*codex知识入库 automation-2026-05-24-... 每天10:00｜每日AI资讯*

以往这三个任务token消耗量在50个积分以上，今天我仔细核实了这三个任务的消耗量，跟各位朋友报告一下：AI资讯的积分消耗量为2，codex入库积分消耗量为6，学术搜索的积分消耗量为3，三个自动化任务的总积分消耗量为11，思考过程改为中文后，积分消耗量节省了约80%。

这三个自动化任务我都选择了DeepSeek V4-Flash版本。好了，各位朋友赶紧去把WorkBuddy的思考过程改为中文。

下面把国产模型使用中文消耗的token量低的原理简单解释一下，纯粹是学习时间，不了解也没关系，改好了出门左转。

根本原因是分词器（Tokenizer）的训练语料分布：

国外模型：英文天生占优，训练语料英语占比超过 90%，词表对英文词根、词缀、常用词做了极致优化，大多数英文单词可以作为单个 token处理（如 "equation"、"analysis"），例如：Thinking = 1 Token，process = 1 Token。但是中文的分词效率很低，中文汉字在底层会被转化为Unicode/UTF-8编码，由于中文字符集庞大，大部分常见汉字需要 1到3个Token 来表示，稍微生僻一点的字甚至更多。一个中文词语（通常2个字）往往需要 2-6个Token。例如：思 = 1~2 Tokens，考 = 1~2 Tokens，过 = 1~2 Tokens，程 = 1~2 Tokens。思考过程 可能需要 4~8 个Tokens。

直观对比：英文："Thinking process" ≈ 2 Tokens。中文："思考过程" ≈ 4~8 Tokens。所以国外的模型优先选择英文。

国产模型：训练语料中文占比更高，分词器专门针对中文词汇和表达习惯优化，常用中文词（如 "人工智能"、"数据分析"）可以作为单个 token处理，英文词组反而经常被拆分成多个子词，导致 token 效率下降。

中文："数据分析"≈ 1 Token。英文："data analysis" ≈ 2 Token。所以国产模型优先选择中文。以下是 2026 年 5 月最新的权威测试数据，基于相同语义内容的翻译对比：模型系列。中文 / 英文 token 消耗比。

平均差异。极端场景差异。Claude 3.5/4。

1. 11× - 1.65×

中文多 40%。商业新闻：中文多 64%。GPT-4o。

1. 0× - 1.35×

中文多 15%。技术文档：中文多 35%。DeepSeek V3。

1. 75× - 0.9×

中文少 20%。代码注释：中文少 25%。Qwen 3/Kimi。

1. 81× - 0.85×

中文少 17%。日常对话：中文少 20%。【小结】。综上，WorkBuddy在主流国产模型支持下，中文思考过程通常比英文更省Token。研究AI，真的很好玩。【往期精彩】。给你的 AI 装上 "万能 USB 接口"—WorkBuddy MCP 保姆级教程。

别再Auto了，WorkBuddy选对模型既省积分又高效。WorkBuddy + IMA 王炸组合：让你的知识管理效率翻倍。配置好这3个文件，让WorkBuddy越来越懂你。
