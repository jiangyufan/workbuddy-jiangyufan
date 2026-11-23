---
title: "刚刚，Claude Fable 5.2 登顶世界第一，一夜斩杀 Opus 5.5"
source: "https://workbuddy.jiangyufan.com/index/hub/case/766"
type: "case"
chars: 3023
sections: 4
figures: 0
chapter: "09-我要省模型成本"
---

# 刚刚，Claude Fable 5.2 登顶世界第一，一夜斩杀 Opus 5.5
![](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfLXWpdfjdXZuhCsMbibbNxT64Uwjrgf0uppVLd9uEx1k8SEVcjl9YTBaibn3GFrickTicUYgNqTRo8vENOuaqJyBuFSszknzzJMQTk/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

1000 个 AI Agent，30 小时完成费马大定理的形式化证明，连续工作 8 天，从零造出一套能在笔记本电脑上运行的操作系统。

就在刚刚，Anthropic 正式发布 Claude Fable 5.2 和 Mythos 5.2 两款新模型。除了上述成果，新模型还解决了两个黑洞物理难题，生成速度最高提升 30%，API 价格降低 20%。

![他们在许多领域都能胜任雄心勃勃的项目，并且在编码、推理和视觉等方面都有所进步。｜上午2:57·2026年11月10日·338.6万查看](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfKiaKIhgE3zTJKEr3nf8rtibTY6rbGIFQkbUuVOkkZK33X1w58m9XOZLVA2jA4icxYsR3D70Mw70Qszu9qcMRYvLXu3MMInUHvPMI/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*他们在许多领域都能胜任雄心勃勃的项目，并且在编码、推理和视觉等方面都有所进步。｜上午2:57·2026年11月10日·338.6万查看*

有意思的是，距离 Anthropic CEO Dario Amodei 公开呼吁放缓 AI 开发速度才过去两个月，Anthropic 就再次推出了更强的前沿模型。与此同时，Anthropic 正筹备估值高达 1 万亿至 1.5 万亿美元的 IPO。

一边呼吁放慢 AI，一边冲刺万亿美元 IPO，Anthropic 这次究竟拿出了什么新东西。

## 1000 个 Agent 连干 8 天，从零造出一套操作系统。
按照 Anthropic 的定位，Claude Fable 5.2 和 Mythos 5.2 是专门面向复杂技术挑战的旗舰模型，重点提升了编程、推理、视觉理解以及科学研究等能力。

两者采用相同的底层模型，主要区别在于安全限制。Fable 5.2 增加了针对网络安全和生物研究的防滥用机制，面向普通用户开放；Mythos 5.2 则保留了更完整的专业能力，主要向通过审核的机构提供。

从官方公布的基准测试来看，新模型的表现相当亮眼。

在衡量 AI Agent 编程能力的 FrontierCode 2.0 测试中，Fable 5.2 获得 49.1% 的成绩，超过 Claude Opus 5.5 的 45.5%、GPT-6 Astra 的 42.8% 和 Gemini 4 Carbon 的 41.1%。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfK2G22B3NCPZrnW8GCZlf6xFD4rsG6EXlEWRSGlWH5JX5MeHkeu4ojNoib6eYZxbiaWtcaya6zvYx85PHqKicLZDenAGosjAD4zmA/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

在 FrontierSWE v2 软件工程测试中，Fable 5.2 得分达到 69.9%，相比上一代提升 13.6 个百分点。而在 FrontierCode 2.0 测试中，Fable 5.2 以较低的推理强度取得了接近 Opus 5.5 最高推理强度的成绩，单任务成本约为后者的一半。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfJtc0qMYAdqbqibCmNLwBwl5iaUFzIKvrfT4NW9RnOjicTbKIIx84WLRYVdasY541zwMk1ExB9CCwNhtmBcYLtXueqJ4zY8zw5wEo/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

第三方评测机构 Artificial Analysis 的最新榜单也印证了这一点。

Claude Fable 5.2 以 65 分登顶 Intelligence Index v5，领先 Gemini 4 Carbon 5 分、Claude Opus 5.5 6 分，并在 9 项测试中的 5 项取得第一。主要优势集中在科学推理、知识理解和编程能力上。不过，最强推理模式下的平均单任务成本达到 26.5 美元，约为 Opus 5.5 的 2.6 倍。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfKH79eciac5OdfibFYqXP3q5vmV6cFSQxsIqXzIeFKAuVr2bpkwxcgxlG0tcOK5cZKM4licjAWpJ3f1lJ6WRSFC2AvV5pEe4TK4YQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

不过，比跑分更值得关注的，是 Anthropic 展示的实际工程案例。

一名工程师向 Fable 5.2 提出了从零设计操作系统的要求。模型从一个空文件夹开始，自主协调超过 1000 个子 Agent，连续工作 8 天，完成代码编写、测试和审查。

最终，Claude 成功开发出一套能够在笔记本电脑上启动运行的操作系统。

按照官方展示，该系统拥有自己的内核，支持磁盘、键盘和网络驱动，还具备文件存储、窗口界面、登录屏幕、安装程序以及内置 Claude 功能。

虽然仍属于实验性质的原型系统，但 AI 已经能够自主协调上千个 Agent，完成如此复杂的软件工程项目，足以体现其能力的变化。

![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfKd4ehSX3M2fgPEJwjFhgCeb3HtJ33fqL2aHCjncmhpBWHwGmlIahgzJJBF1NgfjviaHLraf9XT9Q4Fl0IdWRrbQp3Lo7TqDNQE/640?wx_fmt=gif&amp;from=appmsg#imgIndex=5)

另一项实际案例中，早期版本的 Fable 5.2 还将 Anthropic 一项关键生产服务从 Python 迁移至 Rust，使其启动速度提升至原来的约 26 倍。

发布后，AI 创业者 Matt Shumer 评价 Fable 5.2 是自己用过的最强模型，甚至能够完成过去其他模型难以实现的复杂项目，但它有时又「过度负责」，连正常的工作任务都要横加阻拦。

![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfLrAqtjmPpvI7Sxicy6hm4ATydmj1Nr0T5gAX25ibf9ksIuCYqkGeyOHnYI3LibE6iaLsCs5uFHtKokaV43UJR1kTOJd3QgS1HiceSk/640?wx_fmt=gif&amp;from=appmsg#imgIndex=6)

网友 Kevin Ngo 也晒出了一款由 Fable 5.2 制作、可以直接在浏览器中游玩的 3D 游戏，玩家能够乘船穿越 8 个梦幻世界；

![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfInNwzrDsg1aXfFYP1KNH98LLBzc1peYT4RiciaJ4mCCGkjcmTJibnVHIDv6GVRoMm0HWhZg5YFETI2SP4vpOPvjSfiaTzekzmiaJcM/640?wx_fmt=gif&amp;from=appmsg#imgIndex=7)

另一位开发者 Flavio Adamo 也展示了模型生成的 3D 作品，直呼其三维创作能力强得惊人。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfLias680ibRpUTuDKtf4YgJJ8cgOkjYI0ZYibIwJogfL2Ve7YTr7ibtnXnYYz25agyLURzBEASmOLG6Wvbo2KKO4iaHLXyt5EbOCaCQ/640?wx_fmt=gif&amp;from=appmsg#imgIndex=8)

此外，网友 Synopsis 还用经典的「鹈鹕骑自行车」测试挑战 Fable 5.2，晒出模型生成的作品，并直接称其为新一代 BOSS。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/dCG7OC48IfIdpGiaO5XGEFdVMXWIVS7d343Rt3dhYbBAL1iauOMnnqjNfJhM6YC4z67DtZb7azZ44gOJIEcjXNdibWTltxhKeRQIA2GYictFy9g/640?wx_fmt=gif&amp;from=appmsg#imgIndex=9)

Anthropic 同时透露，目前公司核心代码库中，超过 90% 被合并的代码变更都由 Claude 在人类指导下编写。

从修复简单 Bug，到自主规划和执行持续数天的大型工程任务，AI 编程正在逐渐具备独立承担复杂项目的能力。

## 30 小时完成费马大定理形式化证明，还解决黑洞物理难题。
如果说编程能力的提升还在预期之内，那么 Anthropic 公布的科学研究成果就更加令人意外。

费马大定理是数学史上最著名的难题之一，虽然数学家安德鲁·怀尔斯早在上世纪 90 年代就完成了证明，但要将其转换成计算机能够逐步验证的形式化证明，仍然是一项极其复杂的工作。

Anthropic 此前使用尚未发布的 Claude 研究模型，在人类研究人员指导下耗费 11 天才完成相关工作。

如今，由 1000 个 Fable 5.2 Agent 组成的团队，仅用 30 小时就完成了费马大定理的形式化证明，而且几乎不需要人工干预。

模型在实验中自行建立协作机制，生成的证明长度缩短至此前的七分之一，消耗的操作 Token 也降低至原来的三分之一。作为对照，相同配置下的 Claude Opus 5.5 运行 30 小时，仅完成约 27% 的证明工作。

![费马大定理证明的形式化｜完成进度随时间变化](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfKFTmyPzyBxkyj2lEAxyXCVJTu4FnVujyCZhkyxfaEon7ibg1eeWYGA1utIGuSgYJ50FDk09Lm4g1GlC5JMKkDaEUKm1PibLE9sE/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*费马大定理证明的形式化｜完成进度随时间变化*

除了数学，Fable 5.2 还解决了两个与黑洞有关的理论物理开放问题。

Claude 基本自主完成了此前长期未完成的计算，得到了相同的突变结论。另一项研究中，模型则确定了一种量子引力理论分析方法的精确适用边界。

与此同时，Mythos 5.2 还结合两种现有的开源蛋白质结构预测模型，开发了一套预测完整病毒衣壳结构的新方法，并在测试的 34 个衣壳中，成功准确建模了其中 28 个。

![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfJ55ZfKYnE8UdcicexblFztTosvwgbiahMIySBx9pbd55ft4JMVibbFS1aprcotibwcamRHVAUVJRsYsKSq3aA6WFxcg8RHmgsEicho/640?wx_fmt=gif&amp;from=appmsg#imgIndex=11)

虽然相关科研成果仍需要进一步验证，但从数学证明到黑洞物理，再到蛋白质结构预测，AI 已经开始参与更多专业研究任务。

## 一口气设计三款电子设备，机器人也开始听懂指令。
Claude 的能力还开始延伸到现实世界中的硬件设计。

在 Anthropic 与电路板设计制造公司 Diode 合作的一项实验中，研究人员仅使用一段提示词，就让 Fable 5.2 设计出三款能够实际运行的电子设备，分别是家庭语音助手中枢、USB 会议扬声器和掌上电子宠物。

整个过程中，Claude 自主编写产品规格、选择电子元器件、设计四层 PCB 电路板、建立 3D 打印外壳模型，并开发配套软件。

据 Anthropic 介绍，每款设备的电路板设计都在不到一天内达到可制造状态，Diode 完成制造后，Claude 又指导工程师进行测试和装配，最终三款设备均成功运行，无需修改电气设计。

![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfJO4dRAicibtKenXzCjVT512cS35iaVYdIEAhzklPpRaaR7nOjiaHQ1FdrWRIicQ57UEIUpDQFeg667XrgOOjzQsAxu8FKd1ic4xT1F8/640?wx_fmt=gif&amp;from=appmsg#imgIndex=12)

机器人控制方面，Fable 5.2 的进步同样明显。

在 RoboDojo Sim 双臂机器人模拟测试中，Fable 5.2 的成功率达到 64.9%，超过上一代 Fable 5.1 的 27.6%，以及 GPT-6 Astra 的 29.8%。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfK3YQib4ovfFQF6PRBXL3GBAUXjnzWEkYssPeDlzjiawZV7pIzFsOslWJia5hURibmN3JB3RvCJomgcIWQ3XlsKKgJrp7xP9Xx2orc/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

官方演示中，由 Claude 控制的实体机器人还完成了拧开瓶盖、还原魔方、绘制机器人图案等任务。

![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfJ7eQ5ibgqx36v4QugrfDWYlfMXpUeEPpZg5VwnsQCXSlVXSiaCKdGiaZichDTnF0t1NSjrCGmj9v4H5gcKeUxlFRyeokRPBicy8l0E/640?wx_fmt=gif&amp;from=appmsg#imgIndex=14)

巧合的是，网友 Tekon Burns 也拿出了一个真实魔方考验 Fable 5.2，仅上传 6 张照片，模型就给出了一套步骤极少的解法，而且没有遵循人类常见的先拼白十字、再还原白面的解题思路。

从屏幕上的文字和代码，到现实中的电路板和机器人，Claude 正在尝试将自己的推理能力转化为实际的物理操作。

## 网络安全继续升级，却主动限制 AI 研发能力。
