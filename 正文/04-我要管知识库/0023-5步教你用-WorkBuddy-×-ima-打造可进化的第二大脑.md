---
title: "5步教你用 WorkBuddy × ima 打造可进化的第二大脑"
source: "https://workbuddy.jiangyufan.com/index/hub/case/615"
type: "case"
chars: 2721
sections: 6
figures: 0
chapter: "04-我要管知识库"
---

# 5步教你用 WorkBuddy × ima 打造可进化的第二大脑
之前写过我用 ima 打造我的第二大脑，没看过的朋友可以看一下：26岁，一人公司，我用ima打造我的第二大脑。它确实能基于知识库帮你检索、给出答案，能省不少时间。但实践下来我发现，只把知识库搭好根本不够。

大脑是需要持续去进化的。你投喂的资料可能是过时的，它却不知道。比如你知识库里都是 6 月份的，没有 7 月份的文章，你问它你最近写了啥，它还是基于旧知识库给你答。

细心一点的你会发现，这根本不对，不符合你最新的情况。问题不在 ima，在于我自己。知识库我只会取，不会回流。

建完就完事，从来不把我的过程物投喂回去，所以它越用越笨。说白了知识库是要定期维护的，我之前也没真理解它的定义。

知识库的学名，叫 RAG（检索增强生成），说白了就是给 AI 接上你的资料库，答题前先查你的资料。但光懂这个还不够，关键在下面这张图。

![知识库不是建好就完事，它要持续进化｜你持续投喂资料，它才会越来越懂你](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwhibKbvTooOdYqbibFjLaicGDkxeZaw6KoeSwSfOOkv5q6T3nkibBCjnvh2Sw1AgrvN1Zbl2TZRRiaEko0j0Xpf5LbZLy55YVk2ia2xk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*知识库不是建好就完事，它要持续进化｜你持续投喂资料，它才会越来越懂你*

## 01 建立个人知识库。
ima 知识库分三类：个人知识库、共享知识库、订阅知识库。咱们一人公司用，主要是个人知识库。

![ima 知识库分三类｜一人公司自用，主要用「个人知识库」](https://mmbiz.qpic.cn/mmbiz_png/s10v5MA2Lwia42PiaEHZjc7Ov4yibpTUVr7s9rvqiapuJBKQj3pDUQGkdicDhA19StSGYVXTGSg7ydjic7zUzZgAnHWutNtZgnd0Wl0CsnicZo8yko/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*ima 知识库分三类｜一人公司自用，主要用「个人知识库」*

它支持的格式挺全的，本地文件、文件夹、微信文件、网页链接、笔记、腾讯文档、录音这些都能直接上传，不用你重新整理一遍。

![本地文件夹｜个人知识库](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwjG73De4BjTcWrC3LicW1HWrmzPkNbqzMn2mzcJQUgE8R56Df4AohaXgzSSxlPMb9YzmfqUfholuSiatInNnYOOEVl7lPibKX3pHM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*本地文件夹｜个人知识库*

我自己建了一个阿坚知识库，下面按账号和用途分了几个子文件夹，具体怎么分仅供参考，你有自己的习惯就行。

![阿坚知识库｜个人知识库](https://mmbiz.qpic.cn/mmbiz_png/s10v5MA2LwhNDpHvDYia5BoL6I2ExZIIfIGaNmjIOKVkXvqybWdHyXQNrso1GpSxwvww7GPS0FNvX8gmoDNTrkDQvRVCu82Cz2FGPbEVC6ys/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*阿坚知识库｜个人知识库*

## 02 建立知识库索引。
知识库文章一多，如果不建立索引，AI 每次都得做同样的功课，重新来一遍，又慢又耗费算力。所以我们可以提前先把索引做了，这也是 AI 的逻辑。

![检索增强(RAG)·建立索引原理｜先离线把资料建成索引，提问时只语义召回相关片段再注入，不把整个库塞给 AI](https://mmbiz.qpic.cn/mmbiz_png/s10v5MA2LwgfZDlNAUVqnLTLajOO51DgFjMn6j9N6vVbNX7YgSMiblnm9SuDDZLXYibhT3HuH8WibBRkOulv6ZbpvwTFoREleiaql80YKEUMQvE/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*检索增强(RAG)·建立索引原理｜先离线把资料建成索引，提问时只语义召回相关片段再注入，不把整个库塞给 AI*

具体怎么建立索引，可以参考我下面这句话。

我需要你将个人知识库-阿坚知识库-阿坚AIGC（已发）里面的文章，按照发布时间降序去给我建立索引，以 md 的形式给我输出。然后具体的文章，每一篇都要以 md 的形式给我，就是索引和具体的文章都以 md 的形式输出，最终以压缩包的形式给我，给我下载链接。

![哈喽！我会帮你简化重复操作、提升执行效率。接下来，请放心把繁杂工作交给我就好~｜我来处理这个任务。先加载知识库管理技能，并规划执行步骤。](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2Lwia5kFibp5HDEjXyj4IAicibJHUKiaDmibmgr5OkZFInlGycVe4DhNeYGIxFtNdKNE98uR2ribO7OvCYXHPOS4ib8cJyFvGUS0E2z65hTg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*哈喽！我会帮你简化重复操作、提升执行效率。接下来，请放心把繁杂工作交给我就好~｜我来处理这个任务。先加载知识库管理技能，并规划执行步骤。*

ima 跑完给一个下载链接，点开是个压缩包，里面是索引文件加每一篇文章的 md。后面有新增文章，我再让它按同样的逻辑增量更新，不用全量重新来。

![下载链接 (72小时内有效)：｜包内结构 (139个文件)](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwjEufR7hBicgh7497TSomOkWvj14yhgUjQ5ibWRHyhicX0LZrSiaV61j57zulibIIaUpxZ21rNDHjkVq6z929gn1aFSLfEyCb539hTM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*下载链接 (72小时内有效)：｜包内结构 (139个文件)*

索引我也会让它以笔记的形式留在知识库里，方便随时调出来对照。导出来的这些 md，我会放进内容 OS 的 10_已发归档里，和文章放一起。

![内容(996) 阿坚AIGC (已发)｜AI工具评测](https://mmbiz.qpic.cn/mmbiz_png/s10v5MA2Lwia2Tf08QydictwCyib7wRqcicCW67dtucE02OCicVn6OazZkBrG4pkuMJYZ3RefTBDKvKIsPUmcVN8u7T2h7MdT09Gk4QZRdC2u5nw/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*内容(996) 阿坚AIGC (已发)｜AI工具评测*

![](https://mmbiz.qpic.cn/mmbiz_png/s10v5MA2LwiaZ0JuJq56TWTInkHYZz9QG8cmmxwDmjiaN33HaUA7vPLnacVjOiceH2lB94ZRcdOgxVlXXkxolHclKv3WuSUrXdvqPCXTs1asJo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

前面也说过：一件事如果要做 3 次以上，就值得把它流程化。建索引、按同样逻辑增量更新，每次都重新跟 ima 说一遍，而且它不一定记得住你上次的逻辑。做成 Skill 之后，下次直接调用，不用再重复做。

## 03 回流至知识库ㅤ。
很多人其实没这个概念：今天的事做完了，但过程中的交付物，并没有回流到知识库、也没沉淀成记忆。拿今天来说，我最终的交付物就是这篇公众号文章。如果我不把它回流到 ima 知识库，那知识库就不会进化。所以我们的过程物，都得回流进去。

回流说白了就是：你今天做的稿子、产出的方案、踩过的坑，别留在本地电脑的文件夹吃灰了。把它们回传到 ima 对应的知识库里去。

回流有几种方式。手动回流。一篇文章写完了，右上角点“上传到云端”，选 ima 知识库，确认，几秒钟的事情。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwiaklQCDeVP8ZTkTe9yfWtgdGFN04rLzBZLsu2bY8jtH35iaspmP3DoBNyRdHaicCDz43Lyq50ywPkJXM4NAOectW0mAsYH56BDso/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

![保存到ima知识库｜个人知识库](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwhH23SFujEQia0CibyuRibVy7v8s3KK7lDEeeicNLIyuKoBKRibT739BRy3lRcEZDlO9RyGXWIygD8DNOSbfpw3ibfiag8x4JLXXW9oSs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=10)

*保存到ima知识库｜个人知识库*

让 WorkBuddy 自己回流。你直接跟 WorkBuddy 说“把今天的过程物传到 ima 的哪个知识库”，因为它连着 ima 知识库，能做这个动作。它说已经回流了，记得去 ima 知识库验证。

创建 Skill，调用 Skill 回传。你也可以做一个归档 Skill，每次做完说一句“归档”，它就知道该回传到哪。

设置自动化任务，定时回传。我设了一个定时任务，定期巡检有没有遗漏的过程物，包括记忆、文件，有的话就自动传回对应的 ima 知识库。

这样你每天做的交付物都在知识库里面，你的知识库会随着时间持续进化的。

![](https://mmbiz.qpic.cn/mmbiz_jpg/s10v5MA2LwhgsAic7xLPTImrziansmgXa1vn5zvETszbmAYX5uXerlkuWIjWK8rib4CXSH1DoQQicarmRZrnFnGLsYtgCy3G2v6rYbVWR88dibic4/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=11)

知识库有文件了，分析谁来做。我倾向在 ima 里做。

原因很简单，ima 自带的 Copilot 写出来的东西文风更适合，不像 WorkBuddy 直接调底层那种容易跑偏。所以要分析语气、要生成那种我自己的文 vs 对标的文的对照表，让 ima 自己做就行。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwhL8AE2zHsibpuicz6s9YbYbOn8wEsnuDsF0RrjUdyFz1GYickSzVMsGATicqicDB04icwzv6zenGP9LgiamdZxeUQ44zsMy7rTkLDmyk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=12)

这一张表怎么出。我把自己最近一周写过的稿子全丢进 ima 的同一个知识库，再丢几篇我订阅的几个头部公众号近期文章进去，让 Copilot 出三样东西。

一，我哪些段落写得不错，风格和头部一致。二，哪些表达是头部有、我没用上的。三，我哪些习惯性的写法其实一直不对路。

![已 get 到的风格｜写得稳的那些写法](https://mmbiz.qpic.cn/mmbiz_png/s10v5MA2LwhTrHDKw2tWHBPb5ejxLh9TE8uRt490rP0SjScZ9TFSD2xA1ic9RzQaqp3A5tmn23aPr2hIaLqWQkLavNialPd3YL9ngseXdUDks/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=13)

*已 get 到的风格｜写得稳的那些写法*

出完这张表不是就结束了。下次再写新的稿件前，我就把这张表拿出来，对照着写。哪些点没 get 到或写偏了，就能及时看到。

![好，我把完整分析整理成 Markdown 文件。｜已编辑阿坚AIGC文章风格复盘.md](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwiaNE3O93LaDN8rVVPDqBhBrxLYT8eQgu0HRIx7keAicTrTGfibDUfRLNdhgzpFnOK55z5otibxxwDNGc7qoKQjG9nml4QibHjibXo9Q/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=14)

*好，我把完整分析整理成 Markdown 文件。｜已编辑阿坚AIGC文章风格复盘.md*

过程物都回流进来之后，我会固定用它来帮我梳理：如果对着标杆写，这篇文章该怎么写。我的语气、我的公众号选题，都能从对标里借鉴。说白了这也是我一个不断学习的过程。

光这一遍还不够。我每周会把公众号已发的内容也传上去，让 Copilot 基于前面的索引和分析报告做增量更新，看看这周我的风格比上周更进步了没有，再同步回 ima、也同步回本地。

![](https://mmbiz.qpic.cn/mmbiz_jpg/s10v5MA2LwhicG1v1JFmaOZO3ojygnYXhlJcIuQ7cNuF39qW1Nibcntym6ojq9XzalCrN3OcN93K4vuwtc5fAWQmRd9kZLxTvjz1f5gRN5WD4/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=15)

## 05 知识库持续进化。
上面四步你持续跑下去，会冒出一个感觉：它越来越懂你了。

这其实就是桌面 Agent 最大的好处。你前面做的建库、索引、回流、分析，说白了就是持续在给 WorkBuddy 一份不断认识你的档案。每次回流、每次分析，它都会越懂你，下次给你的交付物就越懂你。

但说到底，它只是个流程。真正让它在过程中持续进化的，是你自己持续的去跑、去发现。因为说实话，对我们所有人来说，还是得自己分析：今天的选题爆了没有，文章的语气该怎么学，针对性地去补短板。它帮你照镜子，但成长这件事得你自己来。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/s10v5MA2LwiaN7pRjiavDfy7vJLRtMxmnTwPEdicUtYbuiapl9CUnzvCrZzFGjIPlG6vs4JA3a4Gk81QNVD58WKUYTrO03nwR2DAoHoAUqvOeqo/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=16)

## 06 我的内容OS。
有读者看完前面会觉得我也要搭一套，但我从哪开始。我把自己的工作区分工画成一张图，仅供参考，不是标准。具体每个目录干嘛用的我就不一一列了，想细看的看图就行。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/s10v5MA2LwiaCm5weibiaPONtpACw1OvVlw135RE4ibXm2yGOnArzNZ878QiaJiczTcnwTFN9ribK4crGVEDH9YCxAW96zY8r2o8nwG9gO3PhNufy8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=17)

## 写在最后ㅤ。
这套工作流是我实际在用的，不是单讲概念，也不是在讲某个工具。工作流听起来可能挺简单，但真要见效，得靠日常去贯彻、去执行。

你如果也想搭一套，先把你已经在用的那些内容，按这套逻辑搭个能持续进化的知识库。最后用一张图总结全文。

![](https://mmbiz.qpic.cn/sz_mmbiz_jpg/s10v5MA2LwgnbRWFo9Dhna9lKNNWuyDaKgf0ibFljLrQCmoJTHjothvpYRWnOYXlpCrJOvWyKQeYbqMtqYMexvicB4NChNzmedWJCVdCXoBLU/640?wx_fmt=jpeg&amp;from=appmsg&amp;watermark=1#imgIndex=18)

- END -
