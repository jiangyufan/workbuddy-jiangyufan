---
title: "别再Auto了，WorkBuddy选对模型既省积分又高效"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/708"
type: "tool"
chars: 1629
sections: 0
figures: 0
chapter: "09-我要省模型成本"
---

# 别再Auto了，WorkBuddy选对模型既省积分又高效
点击下方卡片关注「AI小白笔记」公众号。

昨天看AI给我自动推送的“每日AI资讯”的时候，觉得字太小了，每次都要身子往前凑一下才看得舒服，于是乎，我让AI帮我把字调大一点，在点击发送提示词之前，猛然间想起来网上有人说WorkBuddy的积分消耗有点快，于是我记了一下当时的积分，然后才发送提示词，AI提示调整成功后，我再记一下消耗的积分，不记不知道，一记吓一跳，消耗真的快，就这么简单一个任务，你猜消耗多少积分。

![明天起每日AI资讯生成的Markdown文件字体稍微大一点，现在字体太小了有点看不清楚｜先看下当前自动化配置:](https://mmbiz.qpic.cn/mmbiz_png/JeB8LAjhPIexQQibxAxm3bLDViaXMQvEGEs0eUI5AGyrT6CynrHZ360QFfPQzqAKTqaQP74HIfP6wGwF9YgynNj2ZIbg07KNBEibAHAoKNMLAo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*明天起每日AI资讯生成的Markdown文件字体稍微大一点，现在字体太小了有点看不清楚｜先看下当前自动化配置:*

答案是：17个积分。

调整一下字体大小要消耗17个积分，感觉自己是个大冤总，瞬间觉得腾讯每天送我的150个积分不香了，后来终于搞明白原来是我这几个月一直用Auto模式，Auto模式的底层采用了一套多模型协同调度机制。

简单来说，Auto模式而是像一个智能大脑调度中心，会根据你输入指令的语义复杂度、任务类型，去自动分配任务给某个模型，甚至可能是多个模型协同工作。优点是可以不用费脑筋去选择模型，反正最后你把用户的要求完成就行了，缺点就是自动调度涉及到多个模型（尤其是高价分析模型）的反复接力，通常这时候比你手动选择模型时消耗的积分要多。

大家看一下workBuddy给出来的token消耗：

![](https://mmbiz.qpic.cn/sz_mmbiz_png/JeB8LAjhPIchRMYzFf718gAn30lx0uubkeHD2NWd408to6WKDX8aIB7DLNeVFXqiazRRUX3lPcmq3yDuWOthgKy9AnSicZ7YkXyOdfUlPJX7E/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

模型后面的数字表示价格倍数（相对于某个基准定价的系数），x 就是价格系数，0.40x 表示按基准价格的 40% 收费。简单说，数字越小，调用这个模型就越便宜。从以上截图可以看得出来，目前腾讯推荐使用HY3的力度很大，其次是deepseek-V4-Flash，折扣力度排第二。如果不想去费神研究各模型之间的差异，这段时间无脑选择腾讯的混元模型好了，因为这个最便宜，如果你觉得HY3没有deepseek强大，选择deepseek-V4-Flash也没有问题，一般的问题这两个模型都可以解决。

如果你担心“便宜没好货”，那就得好好去研究各个模型之间的差异了，俗话说“专业的事交给专业的人”，跟AI打交道，就要“专业的事交给专业的模型”，毕竟每个模型专长的领域不同，选错模型不但得不到好的结果，还会白白浪费时间和积分。下面给出一些选择模型的建议供各位朋友参考：

日常简单任务：HY3 或deepseek-V4-Flash，便宜够用。

长文档处理：deepseek-V4-Flash，上下文长度是1M，即可同时处理100万token的上下文，而且输出的最大长度是最大384K，即384000个token。

写代码、逻辑推理：deepseek-V4-Flash或deeseek-V4-Pro，根据任务的复杂程度选择Flash或Pro版本，不管哪个版本，deekseek的逻辑推理能力是毋庸置疑的。

润色改稿、创意文案、短视频脚本：MiniMax-M2.7。

重要的文案处理：GLM-5.0-Turbo，处理重要的合同，写重要的报告、大批量文件处理或文件格式转换。

图片或视频处理：GLM-5v-Turbo。

复杂任务处理：Auto或GLM 5.1，如果是以小时为单位的长程任务或多步骤规划任务，首选GLM 5.1。但是如果想省点积分，可以选择Auto。

当然，如果如果你自己有申请外部大模型的API Key（如第三方平台赠送的额度），可以配置到WorkBuddy的自定义模型里。这种模式下，模型生成完全不消耗平台积分，是最极致的节流方式。

模型没有全能的，只有分工明确的。选对模型，比你指令写得多好更重要。下次再打开WorkBuddy，别再Auto了，花3秒钟手动选模型，收获的是成倍的质量提升和积分节省。

【往期精彩】。WorkBuddy + IMA 王炸组合：让你的知识管理效率翻倍。别再手动搜论文了。用WorkBuddy定时监控，躺着也能追前沿。同样是AI，为什么别人10秒搞定的事你要半小时。配置好这3个文件，让WorkBuddy越来越懂你。
