---
title: "豆包工作悄悄上新功能，把我多Agent记忆整合的焦虑治好了"
source: "https://workbuddy.jiangyufan.com/index/hub/case/927"
type: "case"
chars: 2363
sections: 0
figures: 0
chapter: "13-产品更新与判断"
---

# 豆包工作悄悄上新功能，把我多Agent记忆整合的焦虑治好了
现在Agent越来越多了，各家都在卷。我想把一个老问题解决了，怎么让新Agent适配我们的工作习惯。

以前的做法，要么是建一个项目文件，放一个agent markdown，让Agent去读取。要不是发一段提示词，让ChatGPT把最近对你的了解全部输出一遍，复制到新工具默认的记忆配置里面。

但这些都不够。

Skill，connects（可以理解成一些视频生成代码管理可以通过这个连接），还有你在项目文件里没总结到文件里的实际经验和工作进度，在迁移过程中全丢了。

哪怕今天看到某家模型出了一个超级大升级，受限于它的Agent没有导入选项，还是需要很长时间来手动迁移。或者就只能先让它去做一些信息收集这类通用性任务。

所以当我看到豆包工作上线了一个AI 资产一键迁移新功能的时候，它基本上是把跨Agent迁移的损失降到了最低。具体来说，它支持从ChatGPT、Claude Code里，把我们的AI资产导入到豆包工作继续使用。资产这个词听着有点虚，翻译成人话就是三样东西。

对话。技能。记忆。

对话是你跟AI聊过的所有历史。技能是你教会AI的那些本事，比如你在 Claude 里配的各种skill和connector，你在 ChatGPT 里设的 custom instructions。记忆是 AI 在跟你协作过程中积累下来的经验，它知道你喜欢什么风格的代码，讨厌什么格式的文档，哪些坑踩过不用再踩。

这三样东西加在一起，就是你和一个 AI 之间的「默契资产」。操作很简单。在豆包工作电脑端设置里的数据导入与同步，它会自动检测你本机装了哪些Agent。

![暂无可导入内容｜导入其他AI应用](https://mmbiz.qpic.cn/sz_mmbiz_png/VNz1x8bH8Fxs0RF5U0WInT8tZ0YB45ic0ZAtXIDUh3SoO6ChA1u7dal4rzia62VdDzYBnYNGtYIN1ftNh9V97pVuB9opeUxQVbYbMjVVXWGJk/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*暂无可导入内容｜导入其他AI应用*

我这台机器上Claude显示有240项可导入，ChatGPT有682项。选择导入内容分两类。一类是工具和设置，对应技能、连接器和记忆。一类叫项目和会话，对应历史对话。

![选择要导入的项目｜导入后，数据将会自动同步至云端](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FwmnzBTS6R9xtqMMLmX4yxSeFaHNmicDs2BicfQS2VK65Nviaiaat2hWqEcqVM1NXibKjJicECaO0DxxarYrFJeiaNAn2sezx5TMulT7I/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*选择要导入的项目｜导入后，数据将会自动同步至云端*

我两类都勾了，直接all in。大概一两分钟就完成了。然后我做了一件事来验证效果。打开了一个从codex导进来的历史会话，直接在豆包里继续问了一句。它很自然就接上了。上下文是连着的。之前聊到哪里，它知道。之前定下的方案是什么，它也记得。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/VNz1x8bH8FyPCKxc5Kxx4CSE6kWQaF6eRLaiaUicOl6NibuKAU5nynM8XQ9LuZg9aB3oFo6TQFia0JrHF8oasDDdw6KapnibXqZXA4H5kpCHcvTw/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

但有一个限制我要说清楚。

它只能同步本地内容，就是你PC端客户端留存的数据。如果你一直在浏览器里用ChatGPT从来没装过桌面端，那些对话存在OpenAI的服务器上，豆包是读不到的。

![启用后，同步范围内的数据将会每日自动导入。](https://mmbiz.qpic.cn/sz_mmbiz_png/VNz1x8bH8FxVduYm7YITXsOSu2tBOYq2Bvr2TAPjXoZGeGBAS42APTF6uqeOqTAQLcJezEibzCJn5F7ygjYV3ZTlbgzDNvXq0TyUZGiaeW60E/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*启用后，同步范围内的数据将会每日自动导入。*

PS，我们还可以选择要不要自动同步和范围。搬完东西之后我就开始好奇一些边界情况。

假设我在Claude里写了一条偏好，说我讨厌蓝紫色 UI。在Codex里写了另一条，说我喜欢紫色UI。这两条一起导进豆包，会打架吗。

直接跑去问了豆包团队。答案挺有意思的。导入的只有工作记忆，就是跟具体会话和项目绑定的经验积累。用户的个人偏好不导入。其实是有道理的。

codex也有一个把claude code导入的功能不知道大家有没有用过相当粗暴，直接对话拉到codex里但是如果你用的是第三方api的claude code导进来的对话一是会影响本身的排序二就是对话对应的文件点开会连路径都打不开。

![要同步的内容｜适用于所有已连接的来源和项目](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8Fw3Tz4Py22YprFoAKzibwEiam4qu2wDH23hSrQ9aVwHgOS9kcXUicia3NokYVblCBgbEpicNdzIIhZibqBS1YUpfb1uIibztEzicwLiaib9k/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*要同步的内容｜适用于所有已连接的来源和项目*

如果粗暴地把所有平台的偏好全倒进来，大概率就是一锅粥。

所以豆包只迁移最有价值的部分，跟具体工作绑定的经验和上下文。偏好在豆包工作里重新设一份就好了。它有单独的工作任务偏好指令入口，也是支持从其他 Agent导入的。

![爱沃茨科技｜订阅与额度管理](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8Fy4grPTCakEVF5Cps3lv3UH8M8Oj5MSxicnsbw24Lw8vh5oyv45XeeIBibOjt1Geiak6zh8b69IkJPTuO6SzWejXgLecU815eIcpI/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*爱沃茨科技｜订阅与额度管理*

我还追问了凭证的问题。Claude Code里的AGENTS.md里记录了全局生效的 API key地址，比如Supabase数据库的连接串，豆包能不能也读到。目前还没支持，主要是担心多平台凭证冲突。这个我举双手赞同，密钥这种东西，大家真的不要怕麻烦。像DeepSeek，我之前每次导出API key都是随便起的名字，后面根本不知道费用花在哪了。有一段时间让GitHub自动部署的次数太多，一两天100块就没了，但完全找不到对应的平台。

顺着再提几个豆包工作同期上的能力，都是我在codex上使用频率很高的。

在新对话中继续，从某条消息分叉出新对话，上下文自动带过去，原对话保留。你聊到一半想换个方向的话就不用重新贴一遍上下文了。

![](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FzINEMtWhQoUtOia2Esicsc0rnXZCUOpIAVUTawzBGr5Vs7dq9Q8SybbXvPGcgrwBdIf0KeiavseEJTF853G4BHYrjCSnMticMDfbE/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

消息注释，选中回复里的某段话直接加注释追问，多段一起发送。不用写一大段关于你上面说的第三点是什么之类的。

![任务已派给搭子(Codex后台作业)，现在在跑。汇报一下拆解思路:｜任务:ai-news-radar每条新闻的正文获取初版](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FyvB8GHg5L91BlO0oRgbR3cw68G8nb4mCOeahppOL9KgZmTk7H8YmhRKPeNSDtG3P0aC6aIHnDX2FK3lBrqocnrxz6loYZmvhk/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*任务已派给搭子(Codex后台作业)，现在在跑。汇报一下拆解思路:｜任务:ai-news-radar每条新闻的正文获取初版*

对话摘要侧栏，把当前对话里的任务、产物、技能全列出来。聊了十几轮不用从头翻。

![团队工作台-业务数据现状（飞书表格）｜兰:团队工作台-业务数据现状(飞书表格)](https://mmbiz.qpic.cn/mmbiz_png/VNz1x8bH8FyjvnH2ldWibOgYUXFokTic6L7pjhapiczvhClJrmec4HBWAkSj0DfFumKSvA2lxR8oHrXEo7zvKESuMtfTg2dX7QXfW3NYictLoTQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*团队工作台-业务数据现状（飞书表格）｜兰:团队工作台-业务数据现状(飞书表格)*

PS，右边这个是我用REA逆向出来的vibe coding小工具合集，现在已经让豆包接手去验证，看能不能把任意一个应用一键做成4:3那种最舒服的观看状态。这样哪怕是13寸屏，也能够展示多个Agent的界面。

这几个功能单独看都不算大更新，但放在一起你能感觉到豆包在努力让 AI 对话从一个一次性消费品，变成一个可积累的知识资产。

最后的最后，。

作为一个程序员，我经历了比较长时间从终端转移到可视化界面的过程。我一直觉得 Codex 的界面做得不错，说真的在可视化这件事上它卷得比其他竞品都好。如果不是Opus 5.5这个模型实在好用，Claude桌面端已经被豆包超过十个版本了。我就等着豆包工作的模型再好一点，到时候直接原地开香槟，甚至可以取消一些订阅了。

飞书文档在这个形态上能够存多媒体，比Google Doc更好，。甚至如果你想做视频剪辑，lark cli还有相关视频理解能力支持。

![真人博命高](https://mmbiz.qpic.cn/mmbiz_jpg/YEhakvKZjXmCDLEEW1wClZOVGFURjmibJmciaYLNhp0N55Y6mPiaCj01eV8yzACqDvWDhicbPm07Wu7bboATuKgAbA/640?wx_fmt=jpeg#imgIndex=9)

*真人博命高*
