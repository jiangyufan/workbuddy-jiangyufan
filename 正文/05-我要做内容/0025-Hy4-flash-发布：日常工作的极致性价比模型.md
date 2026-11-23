---
title: "Hy4 flash 发布：日常工作的极致性价比模型"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/916"
type: "tool"
chars: 1124
sections: 0
figures: 0
chapter: "05-我要做内容"
---

# Hy4 flash 发布：日常工作的极致性价比模型
![示意图](https://mmbiz.qpic.cn/sz_mmbiz_gif/7avdgR0YVzLKlLnusU7FydKF9unjxb20phmJMD4UKgEXJoE1m6Gb9WFc4jP80GQuWSXYbll4fhEcQSiaIZOiaENKzUQMsC2FNbNRurwMop78I/640?wx_fmt=gif&amp;amp;from=appmsg#imgIndex=0)

*示意图*

今天，我们正式推出 Hy4 flash，这是迄今为止最高性价比的 Hy 模型，总参数量为 224B（其中 64B Engram 参数），激活参数 12B，支持多模态和 1M 上下文长度，API 价格相比 Hy4 大幅降低。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzKQScLI1hC90TjxUL3AWGsedVjTln6VGiceOgSzfcBF4u8hyMHWILCSe8eW6x9QxO1BhWq9qVkrjFqTcd04siaFSjrttvFLg0ntI/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=1)

*示意图*

我们通过一系列工作在极致优化成本的同时兼顾智能水平和实用性：

在预训练阶段，Hy4 flash 加入了混合注意力、LatentMoE、Engram 等架构特性，KV cache 大小仅为 Hy3 的 1/24、Hy4 的 1/6，且通过大量 scaling ladder 实验确保效果符合预期；

在后训练阶段，我们通过自蒸馏 Hy4 获得了较强的综合智能水平，再通过强化学习使端到端任务输出长度降低 50%；

在评估阶段，我们构建基于 WorkBuddy 典型任务的内部评测集 WorkIndex，并结合人评，聚焦日常工作的产物效果、单轮输出长度、端到端用时，而非远离日常工作的公开榜单分数；

在推理阶段，我们结合 megakernel、4bit 量化、dflash 等手段极致优化，使 Hy4 flash 解码速度超过 150 tps，且可以大规模低成本部署运营。

最终，Hy4 flash 在综合效果上略优于 Hy4 preview；在 WorkIndex 上单任务成本仅为 Hy4 preview 的 1/13、Hy4 的 1/20、DeepSeek-V4.1-Flash-1017（ max 档位，忙时价格）的 1/8。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzL2epuK485PegvNssAKwHQWRERubP58Me784ibxxGPLlcAnV97VctN2zlGO4Fvu3iaicPQYgU4goBkqaCwkGoGmicWkuFyCgcMQ1Dk/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=2)

*示意图*

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzKn3Ugb4C95Q0C6uiazT5oTrEYleVeib0u9GkmQdgiaz4wU0APTwWwLQJe9GKCwbB1QquBdeaoibF7fzibmONeN8t3icvbWMudv6GJqc/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=3)

*示意图*

图 1：内外部任务上的性能和成本。其中 WorkIndex 包含 8 个内部评测集（ PPT 制作、PPT修改、PPT 人机双写、Markdown 人机双写、文档编辑、表格修复、音视频处理、视觉理解）；Open Benchmarks 包含 7 个公开 Agent 评测集（ DeepSWE、ProgramBench、Terminal-Bench 4.0、APEX-Agents、AutomationBench、HLE、OSWorld 2.1）。

![示意图](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzLj2pxaG6hRqtibGkJPEU2icKVoU5tmdkIiapgbhxqqfbHSgj8ZoGeZZrHZHSzGEb1UHmib4wfdkKWhb89JKicEIjZh5YgCAfHtdZw4/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=4)

*示意图*

**图 2：**在 WorkIndex 上的平均任务花费对比。

为了衡量真实使用体验，我们邀请了 85 位 WorkBuddy 内部用户在 27 类共 259 个日常工作任务上进行盲测。结果显示，Hy4 flash 的用户满意度接近 Claude Haiku 5.5，且单任务成本显著低于其他所有模型，任务时长也最短。

![示意图](https://mmbiz.qpic.cn/mmbiz_png/7avdgR0YVzJg0jlc6YabfkPhrr2gWovIcmQ9vDLviaLzicVLoXDIhAnQteDXsdwef2ZhUrSVFicSor1D47vXIqoyH9N3cCsQtHJ2tyhPN8ictiaw/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=5)

*示意图*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/mmbiz_png/7avdgR0YVzLpNoDPKLrxHXysWj5icJwxcqhMlpSRAx2OjBBnDArdjylE11bdwdR6touGmv39LXaCAaYexaFW21iaXNG4ibHKmOxoLye6gAdT9c/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=6)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzKS3SiaAoX9zNUqicDlquI4m7t7nrvQjBuS4ibu2DvGsWgUib36PSHV8sPYWnOom0ice6X1RCwNBzqxBCrm8eicg6SbicWknoSgThZMsM/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=7)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzKqtsr6aaIuzAM8Jb9b117a0gzncRcCyMrFVNzAnvmLowkfrtR7dxic4TqxTBWSbfxGYQqjGBerMV5XaBlKHticppz5yphvYcMKg/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=8)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzKfaG1rajT8JWc2xg0ZD9h4Jib3JpricicMg8ibnSsMMTGEmyqfPPye6CuNrakfFdSvcU0ljXbOYyxjyQKs3EpKE0atNVicfVJgGXJc/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=9)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzJRRPibIsBfZ94v18YgxRNbtPXO9MukReL9bqQWwK3GAgeLIUm25M7mgPLfRLlT32NUSFiabGm4L0U2WRAauz0Ov4UevbvHs91do/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=10)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/mmbiz_png/7avdgR0YVzIIrjF0T2MzUPvQejqGmPaUQzkObysCBjXEPjaiaKywXfsut1P1RkMP5ex31rl3LQTgKqeHyNP46ExrIMJaibicN0DneyJCSFVibyQ/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=11)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/sz_mmbiz_png/7avdgR0YVzIsoVTibL3shDRntLENEkN9KO3BD845bSyibv9ukzMEibxRlzG1tZpialRb82tjiavg3U3Je1EosBwgg0qcdSJiclZtGibAx0ROFSSO04/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=12)

*Marvis 算法工程师 Baihan*

![Marvis 算法工程师 Baihan](https://mmbiz.qpic.cn/mmbiz_png/7avdgR0YVzImGaiacfMhd7KPcqdmmHOFIUvn2LysfibxlpKpZGvarV0mS8V8a3C7sJ1DnT8ibuMtz2J2PLccpEU1hLZIlJNawkggcpNgvbs0XU/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=13)

*Marvis 算法工程师 Baihan*

**附录：**模型得分。

![示意图](https://mmbiz.qpic.cn/mmbiz_png/7avdgR0YVzLuW6OAibHGbiaLiakVjXibe7C4qaWctruhJ8b8iciav7OIfP26CiadRX4LxCOSQe1nKa1zUt24XSrjloQ2lUNuyfoMyRhB7foKr7NBKY/640?wx_fmt=png&amp;amp;from=appmsg#imgIndex=14)

*示意图*
