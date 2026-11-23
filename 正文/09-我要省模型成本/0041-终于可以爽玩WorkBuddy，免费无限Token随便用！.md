---
title: "终于可以爽玩WorkBuddy，免费无限Token随便用！"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/669"
type: "tool"
chars: 1336
sections: 0
figures: 0
chapter: "09-我要省模型成本"
---

# 终于可以爽玩WorkBuddy，免费无限Token随便用！
过去一段时间，我都是在用Codex+GPT5.5，钱包终于受不了了；前两天又换成国产顶流的 WorkBuddy + DeepSeek pro方案，维持一下。讲真的，Token烧的还是有点凶，积分蹭蹭往下掉。Agent任务启动，就像一台大型发动机，一轮就烧掉几百上千积分。反复几遍后积分就干没了。

刚好最近朋友又推荐了个好东西：Agnes AI全模态模型免费用。不像别家需要花里胡哨的注册、参与活动啥的，这家注册即用。而且文本、图片、视频都免费。经过我的两天实测，确实可以用，不会因为免费沦为玩具，而是真正能用上的。下面就推荐给大家，手把手在WorkBuddy配置，从此不再花费一个积分：

1. 注册得到API key

![来自全球AI实验室 Top 10免费API｜前沿模型 免费畅用](https://mmbiz.qpic.cn/sz_mmbiz_png/rKQDFflVrsvPjNo5FYwsZdwdYLzSoHHWnLb6Z92bNsRkg4hmhhgLjYhfgzFZdQvDPxsjiamfzUDySR1NKr5GLjkn1XyTWGaG95auG9W1kSTw/640?wx_fmt=png&amp;watermark=1#imgIndex=0)

*来自全球AI实验室 Top 10免费API｜前沿模型 免费畅用*

登录成功后，点击创建新的密钥，并复制好等会用：

![重新启动部可更新｜请勿与他人共享 API 密钥，或在浏览器或其他客户端代码中泄露。](https://mmbiz.qpic.cn/mmbiz_png/rKQDFflVrsvYc0Oyg8LbqiaQ6TPrQ0HllCPibgxaMBSN8YyAOmUt1uv1y6hYhK1xZCvmPVwiaZALuSSywNF8NqSZWWic9ucGFvNRrX17zbmdXKs/640?wx_fmt=png&amp;watermark=1#imgIndex=1)

*重新启动部可更新｜请勿与他人共享 API 密钥，或在浏览器或其他客户端代码中泄露。*

就这两个操作，你就能在任意的Agent平台使用了。

1. 在Workbuddy配置

点击模型选择按钮，选择配置自定义模型：提供商一直往下拉，选择自定义/Custom：

![© 系统设置｜▶智能体设置](https://mmbiz.qpic.cn/mmbiz_png/rKQDFflVrstZFY6xH7mV5S54CVfL8JwatSIuiciaXgsOxr9R8l0NGvDRVV8HAw0mnNWNbWovzeLKjicSVQAOUK7F0C7HOhQkL3hXygP5QaSemo/640?wx_fmt=png&amp;watermark=1#imgIndex=3)

*© 系统设置｜▶智能体设置*

![仅支持 OpenAI 兼容协议 API｜智能体设置](https://mmbiz.qpic.cn/mmbiz_png/rKQDFflVrstT0R8m6M6AcQBN14BAxqtPqOzkUdgVdTQllL2zQic9FwTNS2ibtJKIJibtSHfeRnfdgC2jfmhXS2eicyfurZq8cHYJicgO1Sn9gsUc/640?wx_fmt=png&amp;watermark=1#imgIndex=4)

*仅支持 OpenAI 兼容协议 API｜智能体设置*

这样文本模型就配置好了，进入一个任务，就能选择自定义模型：agnes-2.0-flash了：

![Hy3 preview ① High 限时折扣｜资料库·灵感](https://mmbiz.qpic.cn/mmbiz_png/rKQDFflVrsuv0BvAbribDNFjkgwUrp3uo07KIJicRmm6SaGwxzKAIjUUllibribkibt3sDt1j5R6BINUibfia2a9PTbNTAytpFnlk0QA75WicnQGcLM/640?wx_fmt=png&amp;watermark=1#imgIndex=5)

*Hy3 preview ① High 限时折扣｜资料库·灵感*

美，以后用的话再也不担心积分消耗了。

1. 图片生成

Agnes 确实可以支持图片生成，我也试了很多，但说实话：不如豆包。例如我使用难度比较大的流程框架图生成来测试，我使用下面提示词：

生成图片：专业扁平化系统架构图，矢量简约风，纯白背景，2K清晰，无3D、无阴影、无多余装饰。圆角浅灰模块，蓝色规整连线，布局整齐不交叉。从上到下五层结构，文字清晰可读：

1. 用户交互层：网页前端、API接口、Prompt编辑器、批量任务面板
2. 调度Agent层：语义解析、参数校验、任务调度、负载均衡、状态监控
3. 核心推理层：扩散底模型、LoRA适配器、ControlNet、采样器、降噪模块
4. 辅助工具层：图像超分、水印压缩、画质质检、格式转换
5. 资源支撑层：GPU集群、缓存数据库、文件存储、日志服务

数据流：自上而下传输，质检不合格回流至调度层重生成，合格正常输出存储，标准工程架构图。然后让agnes-image-2.1-flash模型生成得到的图片字体大小不一、甚至有错字：

![用户交互层｜批量任特器](https://mmbiz.qpic.cn/sz_mmbiz_png/rKQDFflVrsvw6cleyP6RxnM4JNJRH5IxzJceSLtjNFaypCFGeKcIUic1JyatorfN835QjYn7dGicFTgoJHDswxdvjW3cjgCQc6iblPL86cM9hc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*用户交互层｜批量任特器*

同样的提示词，豆包生成的：

![网页前端、API接口、Prompt编辑器、批量任务面板｜语义解析、参数校验、任务调度、负载均衡、状态监控](https://mmbiz.qpic.cn/mmbiz_png/rKQDFflVrsuq22PFRYtzxyKIBFBZW9l8hXgV5d2lPauacicibTpttT637jKwdQNYFUQ2TY0SaM8ZC7UOgXXggwUcFia8kzyWON9GXTiaoIfB7kc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

*网页前端、API接口、Prompt编辑器、批量任务面板｜语义解析、参数校验、任务调度、负载均衡、状态监控*

我看到很多文章在说图片生成很好，但是实测下来并不太行，还没有豆包好。所以并不推荐使用这家的多模态模型。

另外，Agnes官网说本周将灰度上线最新模型，比如文本模型的上下文长度将会从 256K 直接升级到 1M，图片模型升级后会新增 4K 输出档位，这就更香了。

最后提醒一句。

Agens 模型不是只能接入 WorkBuddy，OpenClaw、Codex、Claude Code、Hermes 等等智能体都是可以接入的。

每个接入方式都写得很清楚的操作手册，根据自己的需求去接入就行。
