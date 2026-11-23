---
title: "用 Qwen4-Max 拆完一台 iPhone，我发现了阿里大模型进化的秘密武器"
source: "https://workbuddy.jiangyufan.com/index/hub/case/739"
type: "case"
chars: 2778
sections: 2
figures: 0
chapter: "09-我要省模型成本"
---

# 用 Qwen4-Max 拆完一台 iPhone，我发现了阿里大模型进化的秘密武器
![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfIw02SLqNGDiaOzMNlF59iasQicInpuvRGkpYHWlQZGpXwfuk7QODctBKGXp4nUhHVs7KcAvmEZrRc4FmBvnTehq0WJIELF2Oibnh4/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

最近 AI 大模型的神仙打架，似乎和国模没太大关系。

Claude Fable 5.2 刚刚刷屏，Gemini 4 也一周发更新几款模型，GPT-6.2 Astra 也曝光了不少测试，相比之下，国产旗舰这边安静了不少。

今天上午，阿里正式交出了破局之作——新一代旗舰模型 Qwen4-Max。这也是刘大一恒执掌 Qwen 大语言模型后发布的首款旗舰。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfLXkSzv6IaoQFZTbY49oWscAElhojjx4FEvu42g7KtEHzRb11I895XjhTsqfZrO6etIhrhzdEiaEYYlTDChvCEJ5oRvYjzTruKY/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

APPSO 在发布前也已经体验了一段时间 Qwen4-Max，看看它能不能再次回到国模顶流行列。

在提前上手体验了一段时间后，我们发现它的发力点非常务实，把长周期任务的成本打下来，并真正走进重型专业软件里「干活」。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfLGEIneyhv7WIicQwIrk740VoBaMdqEtVk8x81K4yVewY790b2AL4Dvwgu24YdxdPHEBqQEO68FqBk73ibsKU85ibibwCwm5O1ZHR4/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

Qwen4-Max 换了一套全新架构，总参数 2.4 万亿，处理每个 token 时只激活其中的 710 亿，比同样规模的上一代 Qwen3.8-Max 少了大约四分之一。它有原生的视觉能力，支持百万 token 的上下文。

这样改动架构的目的就三个：长上下文算得更省，模型装得更多，训练更稳。落到用户身上，最直接的感受是一个字——省。

在编程评测 Terminal-Bench 4.0 上，它的 token 消耗比上一代少了将近一半，得分反而从 38.9 涨到了 48.5。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfLwxunicCYUnXGKahMS1sP4uTCyL4tbQcQloEuc7sznnwa4CUjibK4TQGmzPaaJR3SYNHZ0CS6ozGd44qXibaZjqYZWd1qJwickoZ0/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

国内 API 每百万 token 的输入价格从 12 元降到 10 元，输出从 36 元降到 30 元，缓存命中最低只要 0.5 元。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfIlHLZp8P1dD4BAVKlt2aPbo7HuH1EcXxibHcOmiaY6C8ibhbQP8A3MxTicAoq0ZpiavhdS4x6dGdVaY4ECqg3M5Lia9ibppcXKYTM7KI/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

在阿里自己的 Work360 评测里，完成一个任务的平均费用从 26.58 元降到 11.16 元，少了 58%。

![行业能力评测｜注：雷达图采用统一的分段刻度，外圈高分区间压缩显示。](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfJ5A6PFOk9hBJMhAPnd22liav86pGk50jpCJeR6Pt8TicCicnMQkzLIoGFBsYMBToxmtJ4hakKVPfbYVWzamf2KGreRMibwg14tPKw/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*行业能力评测｜注：雷达图采用统一的分段刻度，外圈高分区间压缩显示。*

在靠真实用户盲测投票的 Code Arena 网页开发榜上，Qwen4-Max 拿到了 1750 分，直接冲到全球第 6，前后夹着它的分别是 GPT-6 Astra 和 Claude Fable 5.1，Qwen4-Max 也是目前榜单上排位最高的国产模型。

当然，它离当下最强的旗舰模型 Claude Fable 5.2（1826 分）还有一段距离。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfIRYa8j4frzlEvXTf3278NwicRiaDCd81btibmI3AibzaCvFM3ATwwNPcMckBufbmSASiaeCC46NqFhXBXqnlZRiaeRHpYNibic52stqWY/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

在第三方评测 DesignArena 上，Qwen4-Max 在 PPT 生成榜排第 4，排在 GPT-6.1 Sol 和 Kimi K3.1 Pro 前面，在表格榜排第 5。

看起来这是个天选「打工模型」，办公才是 Qwen4-Max 的主场。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfJAE4oSiadwQxeAIty6Symewoe5Na8PIVvVQkFQfB7d9Lyhvg45JdclHHOfu52881ib1VR26p2LQ69FHJ5kWskNUWnzlLAX7MIEU/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

另外，Qwen4-Max 在长周期任务评测上力压 Claude Opus 5.5 和 Kimi K3.1 登顶。在需要连续执行几十步的复杂任务上，它不仅成功率最高，单任务成本还比前代砍掉了近六成。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfJMv0swfibYiaYFSnZZNYja7oKXEPQyUDZmqUdZMVfOYG01tr9VEvDf6NM7gS6DQ6sR6yrBxu4y4jjicVvbztzaHic2HGfzPmhhsn0/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

阿里展示了Qwen4-Max 在不同行业的应用，还给这种干活方式起了个名字，叫「持续交付」（Live Delivery）：先交一版能用的，再根据用户的意见一版版往上加。

他们举的例子是一个物理课堂科普网站，Qwen4-Max 前后交付了 14 个可用版本，最终扩充为一个包含3D动画、交互实验和原理详解的精致网站。

![边做边交付 方向全掌控](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfIaf427WY6qaVLuFCHM9ahaTInVs2uQqgySPE7cFkM5ibQRCkbWMynJ9iblHwkgCNichr1V8iaAJE0UIz0bOIQIVvYzjM2TqPUNj34/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

*边做边交付 方向全掌控*

目前 Qwen4-Max 已经上线千问 AI 平台，可以通过 API 或阿里的 Token Plan 调用，也能在千问办公、Qoder、千问 App 和 Qwen Studio 里直接用。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfKREsicZ9a3B722KIFPafnJutf68rlWjEDdpm5W33hvySq2PkX68iaIBsehNX1Jic21kvAjN9k2guTzNTbib1hNCHgibO71DhyRTpfA/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

至于大家关心的开源，这次的 Qwen4-Max 暂时还没放出来，要等后续 Qwen4 系列里小一点的模型陆续补上了。

## 我们让它拆了台 iPhone。
说了这么多，我们还是实测 看看Qwen4-Max 的真实表现。

我们围绕电路设计、机械建模、Blender 三维创作和游戏引擎进行了测试，跑的都是实打实的本地重型专业软件。

我们让它用 Three.js 给橙色的 iPhone 17 Pro 和特斯拉 Cybertruck 各做一个可交互的拆解演示，要能转视角、能拖动展开进度、还能合回去。

整个演示没有走捷径去调用外部 3D 模型文件，从螺丝孔位到金属拉丝质感，全靠代码从零构建几何体拼接而成。

第一版出来后，iPhone 外观还原得不错，就是拆开后的内部零件偏少。我让它接着细化，它直接基于原有代码继续迭代，很快补齐了内部结构。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfKFIG3br1t6KlS3yFa0UZnqluPuhyT602cpBMu5uBj7Qh7XicToaxlhxkZ4czLpJs781wibNiczNwbX2SvzZ1xzuW2GnUkQAADK50/640?wx_fmt=gif&amp;from=appmsg#imgIndex=11)

新版本里，随着屏幕缓缓让开，电池、托盘、排线和充电线圈层层错落排布，金属、玻璃和橡胶的质感也分得清清楚楚。所谓的三维空间理解能力，在这一刻算是有实感了。

同样的方式再拆解 Cybertruck，制动、悬挂和电池连接的错落结构也都具备了。把展开滑块推回零点，几十个零件全部精准归位，基本没有出现错位或穿模。

![CYBERTRUCK 拆解展厅·TEARDOWN｜长度 5682.9 mm - 宽度 2031.6 mm - 轴距 3635 mm](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfKbJwLFzWU1vMUlgCkmJIWaoNPFQzBbXjjOWuVhjeFAGtsE4S9Nias2KZ9GK3Wiase9ZE2iaBQfUSTaS3asVy3ibI5aVT82PiaJdIZ0/640?wx_fmt=gif&amp;from=appmsg#imgIndex=12)

*CYBERTRUCK 拆解展厅·TEARDOWN｜长度 5682.9 mm - 宽度 2031.6 mm - 轴距 3635 mm*

APPSO 发现「出初版—看画面提意见—原工程迭代」这样的思路更高效，算是把「持续交付」这套工作流彻底跑通了。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfIa5A5QxuzAby3PxZ5NyOj7bwYQQbLkcdAB3UiaOjNXhvUBcYcPuiad6VQdwBwicCs87uc7hEB2YiaLyfqKHLXuV2DrNPB9BSJCicvI/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

重度依赖 AI 干活的人大概都经历过盯着额度刷新倒计时的焦虑，甚至半夜还要爬起来续上任务。这次我干脆让它动手设计一个床头物理提醒器，额度一恢复就自动提醒。

这相当于让它一个人干了结构、电子和动画三个工种的活，先用写代码画工业图纸的 OpenSCAD 建出精准外壳，再用专业电子电路模拟器 ngspice 跑通内部电路，最后导入三维动画软件 Blender 完成整机装配与动态演示。

跨软件协作最大的难点在于三者必须严丝合缝地共用同一套物理尺寸，而 Qwen4 最终处理得相当到位。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfJIIuzwYPTwAibibTKoWH2UywXfYYVLhbVicjst9dad2wMZNssVVs8Yq03Bn5NB0bq7C6IEsia9KFsPHtO2EdYA1MKJhZicLaW0nwUo/640?wx_fmt=gif&amp;from=appmsg#imgIndex=14)

我们还让它在 Blender 里设计了一台叫 LOOP / 8 的掌上音乐合成器——巴掌大的机身，正面排满手感按键和调音旋钮，小屏幕上还跳动着实时声波，内部藏着好几层精密的电路板。

它先交出了静态的外观效果图，接着我们让镜头绕着机身转一圈，再把整机像拆积木一样分成四层展开、最后重新合拢。中间它自己改过一版脚本代码修掉小毛病，就把整段丝滑的工业级展示动画渲染了出来。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfId3obPJhLhv08ODfIqMISzDYMcGSPEkPT0lfAache60J6UEnFBwjzDfYLXKDC5k7sicpjjxtVtN5X76Xf5vuFpKMFerv8NKHOQ/640?wx_fmt=gif&amp;from=appmsg#imgIndex=15)

## Qwen4-Max 背后真正的秘密武器。
只看榜单，编程盲测排在第 6 的 Qwen4-Max，确实还不是最顶流，不过模型迭代速度之快，这些排名一个月就可能更迭好几次。

阿里这一代想讲的故事，也许本就不在跑分榜单上。

这要从 9 月的云栖大会说起。阿里当时提到了一个很热的概念——递归自我改进（RSI），简单说就是让 AI 参与进自身的迭代循环里。

上一代 Qwen3.8-Max 已经跑过雏形：全自动迭代 33 轮，甚至在芯片实验里连续调用上万次 EDA 工具，硬生生把芯片面积缩小了 42%。

到了 Qwen4-Max，这个自我改进的故事往前走了一步。架构上，它在总参数不变的情况下，让每次计算少动用四分之一的参数，先把自己变得更省。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfKdgykcn37FSFDPRiafjwd9HeibUFzEtRBfcBgibL0OM6icfDajrU0iaqiceW6x9rxbdJKeEolSAFHBznT85FY92MTkqWXX4EibcpjRxg/640?wx_fmt=png&amp;from=appmsg#imgIndex=16)

然后它被派去优化自己跑在上面的调度系统。模型写出候选算法，求解器打分，再改下一版，结果是标注任务的调度成本降了 10.42%，CPU 离线重调度快了 14.61 倍。

省下来的算力也没闲着，阿里在云栖大会上就预告过，后面的 Qwen 4.5 和 Qwen 5 要做到 5 万亿到 10 万亿参数，是现在的两到四倍。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfIXXKl0Zlf4iaydjdaDBQWBiczVVDZ5iaydoSZrIFZ6FbJcbWhTv4OupyNs2Tj3KicBdqicta5jbLeAvKgnxveiaV8fQkGMSQ61rRtsA/640?wx_fmt=png&amp;from=appmsg#imgIndex=17)

这么看，Qwen4-Max 的真实身位就清楚了，它未必是当下最聪明的那个，但它是整条进化回路里的关键一环。自己先学会省吃俭用，才能让后面的庞然大物造得起、跑得动。
