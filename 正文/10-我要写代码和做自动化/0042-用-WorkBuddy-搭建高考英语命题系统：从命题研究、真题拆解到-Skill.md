---
title: "用 WorkBuddy 搭建高考英语命题系统：从命题研究、真题拆解到 Skill"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/337"
type: "skill"
chars: 1786
sections: 0
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 用 WorkBuddy 搭建高考英语命题系统：从命题研究、真题拆解到 Skill
![让 WorkBuddy 学会像高考命题人一样思考｜从命题研究、真题拆解到 Skill 固化，搭建一套可复用的英语阅读命题系统。](https://mmbiz.qpic.cn/sz_mmbiz_png/W41dM10xkaC5AU12uX7o7hoLVeWzxAPkZehwdf5sXiaHfmv7reZBtlCsXGW6K3CibY1kqOSQyNhWhmPrFLOvVg4xF7qBwdRdWXmNR2erLXTVc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*让 WorkBuddy 学会像高考命题人一样思考｜从命题研究、真题拆解到 Skill 固化，搭建一套可复用的英语阅读命题系统。*

以前做英语阅读命题，我觉得最耗时间的往往不在写题目，而在反复琢磨一些更靠前的判断。这篇文章到底要考什么，正确选项要通过怎样的一种转述才算成立，干扰项怎么设计才具备相应的迷惑性，又不至于出现两个答案都说得通的情况。

后来慢慢意识到，只是把文章丢给 AI 让它生成四道选择题，这套流程没有把问题真正解决掉。它出题确实快，往往一下就把题目给出来，可这些题里有些只是对原文做了较为简单的复述，有些干扰项跟文本的关联明显脱开，甚至连考查的重点都没抓准。

![先建立命题研究资料库｜资料先归档，后续分析、检索和命题才有统一依据。](https://mmbiz.qpic.cn/mmbiz_png/W41dM10xkaBd77afjPuj12JicNFCfo2uHnSI9iarpzRHCvuDlstSMx1nIAPKz6eG4rcCPoqTetM5mib0FwP0gfawQibCLS7iauiah4gmEaGNerJVs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*先建立命题研究资料库｜资料先归档，后续分析、检索和命题才有统一依据。*

所以后来我换了一种思路。出题这件事先往后放，优先让 WorkBuddy 对高考命题的内在逻辑形成一定程度上的理解，等它有了相对稳定的判断，再去承担具体的出题任务。

第一步是建立命题研究方面的资料库，把正答转述、干扰项设计、语篇分析以及历年真题分门别类做了整理。这里有个细节比较关键，不要把资料一股脑丢给 AI。不同类别的论文、真题和自己积累的错题最好分开归档，来源和原始文件都保留下来，否则后面要查某一种命题技巧，各部分很容易混在一起。

![先让 AI 独立命题，再用真题校准｜真正的训练，不是让 AI 背答案，而是让它先出题，再和高考真题逐题对照。](https://mmbiz.qpic.cn/sz_mmbiz_png/W41dM10xkaAniblUdKeuvBuibEEKggI8xESdXCjR39iaDo7NkBm1Iao67dc5Qaz6gmkgBZKnOeQxa9Dk0qf6RtwFREeX0OKLia40292nkjE7frY/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*先让 AI 独立命题，再用真题校准｜真正的训练，不是让 AI 背答案，而是让它先出题，再和高考真题逐题对照。*

第二步，我先让它独立完成命题的动作，再把结果跟原版真题做对照，没有让它一开始就去模仿真题。这一步很值得花时间走一遍，相当于给它安排一次有参照物的练习。

比如给它一篇阅读文章，先要求它把文章结构、段落功能以及关键信息分析清楚，再独立设计题干、正确选项和三个干扰项。完成后逐题检查，考点抓得准不准，正确选项在原文里能不能找到对应的依据，那几个错误选项是不是用了真实信息，却在对象、范围或者逻辑关系上出现了相应的偏差。

我自己的感觉是，一道阅读题最后的质量高低，很大程度上就落在这些细节上。

![高考阅读命题五步法｜先让文章说话，再给考点穿上题型的外衣。](https://mmbiz.qpic.cn/mmbiz_png/W41dM10xkaAkvsN6G6hC9258MUXv0y294Uia35Huwyg8CXnQAefVMhJ2PESDUukeEFU9X7ibI9cPljqqyLYYXQicdU3JSZR5Fic0zjTSP62YR9M/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*高考阅读命题五步法｜先让文章说话，再给考点穿上题型的外衣。*

整个流程我归纳成五个步骤，先把文章的骨架读出来，再找出关键的断层位置，接着匹配相应的题型，然后设计选项，最后完成一遍质量上的自检。

干扰项这一块尤其要留意，没必要为了提难度就故意写得复杂。相对有效的思路是在原文里找那些可以被利用的信息，再通过因果倒置、张冠李戴或者范围扩大这些方式把错误选项设计出来。这样出来的题目迷惑性才比较合理，不至于变成单纯考学生认不认识生僻词。

![在 WorkBuddy 里如何完成一轮命题任务｜从资料调用到结果输出，把命题研究真正跑成一套工作流程。](https://mmbiz.qpic.cn/sz_mmbiz_png/W41dM10xkaAteWxKLhJNibF3tlxgkjpuQAzgiaibUY8a4cbbWBiaHGr2eb22vpnx0Zib1wIFsl8syQmtAZqVibme4ibxTFialN0MWRzv94sg6sWrQp4/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*在 WorkBuddy 里如何完成一轮命题任务｜从资料调用到结果输出，把命题研究真正跑成一套工作流程。*

![实战示范：用一篇深海阅读文章出题｜从文章结构出发，而不是先凑题型数量。](https://mmbiz.qpic.cn/sz_mmbiz_png/W41dM10xkaDkmKyxIMfZkhD11bqBtSegxkfCqYctzUB56zcJkjK0EzROpyrHicdGTClJAdbg09n65lROeySgyfj5DAnpbMrAiassT1K7DTpzo/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*实战示范：用一篇深海阅读文章出题｜从文章结构出发，而不是先凑题型数量。*

深海阅读那个案例，我也是按这套思路拆的。从开篇太空与海洋的对比，到不同深度海域里生物适应机制的情况，再到热液喷口以及全文主旨，先把结构梳理一遍，再确定下来七个考查点。按这个顺序生成的题目，文本依据就比较清楚，也不会为了凑题量到处找句子。

最后一步是把比较成熟的方法沉淀成 WorkBuddy 的 Skill，我认为这是整套流程里最值得长期积累的部分。把命题原则、执行步骤、输出格式以及检查标准写进去，以后再遇到新的阅读文章，就不必每次都从头解释要求。当然，Skill 建好也不能直接当成成熟产品来用，还要拿不同体裁的文章反复做测试，发现问题再改规则。

![选项设计，决定题目的高考味｜正答有锚，错项有影，难度来自信息关系和思维加工。](https://mmbiz.qpic.cn/mmbiz_png/W41dM10xkaAYicEnCSTRInJEicDl7fEybUV6hfp4edIqIFicdkEY9AcWm7zAzRt5iaWTD4dpCGs7xyVFaQIrVpuXpny10eSiaRXianhNsorOQicMVk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*选项设计，决定题目的高考味｜正答有锚，错项有影，难度来自信息关系和思维加工。*

![把命题方法固化成可复用Skill｜一次研究，多次调用，让成熟的命题流程真正沉淀下来。](https://mmbiz.qpic.cn/sz_mmbiz_png/W41dM10xkaDZqAIicibxKvyURwicKAaTBoicYt9ltPuCHNljnPve3hHSLNBGGDQRTgueYGXjIsTRJ4RG94RBjaGE4yu7MCoeUicFXWOichWadABiaA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*把命题方法固化成可复用Skill｜一次研究，多次调用，让成熟的命题流程真正沉淀下来。*

这套方法给我的一个启发在于，AI 办公真正值得投入精力的地方，很大程度上落在把长期积累的专业经验逐步转化成可以被重复调用的那种工作流程上。一次性能完成多少任务，反而比较次要。

对英语教师来说，AI 能帮我们整理资料、分析语篇、生成题组，也能完成一些初步的检查，可是最终的命题质量，仍然需要教师结合课程标准、学生水平和真实的教学情况来作判断。

先让 AI 学会方法，再让它承担任务。与其每次都重新教它怎么出题，不如花时间建立一套自己的命题 Skill。

![知识库手册·2026｜高考英语阅读](https://mmbiz.qpic.cn/mmbiz_png/W41dM10xkaA7hSYG4u6v09ENAt8ymaKRHRXC6KNc3nRpIBzGQepTJlZicEW5I66ttazMILUebBHeAAtrjgRGK5dPbRUk1BPyHx3icsKeAibwjE/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=8)

*知识库手册·2026｜高考英语阅读*

![](https://mmbiz.qpic.cn/mmbiz_png/W41dM10xkaBBUpppf3icdpu1WzqwvqcicLSZAIvGbZeK8LYk7fnVl2zLOO7K7niaZcdHmvVj9QyYEiapJzdZiaxXeAudUJW2KaCcvAAiaHhOgcoRs/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=9)

#Workbuddy #AI #高考 #真题 #错题 #复习 #学习 #教师 #知识库。
