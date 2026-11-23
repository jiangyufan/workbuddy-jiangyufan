---
title: "WorkBuddy 保姆级教程开源了！600 多篇 Agent 资料一次性放出"
source: "https://workbuddy.jiangyufan.com/index/hub/case/611"
type: "case"
chars: 3202
sections: 8
figures: 0
chapter: "01-刚装好还没跑通"
---

# WorkBuddy 保姆级教程开源了！600 多篇 Agent 资料一次性放出
大家好，我是汤师爷。如果你最近在学 AI Agent，大概率有过这种感觉。教程刷了不少，提示词也收藏了一堆，可真要自己动手，还是不知道先学什么。WorkBuddy、Codex、Skill、工作流、知识库、MCP，一个新名词接着一个新名词。今天跟着视频做一个案例，明天换个平台又要重新学。收藏夹越来越满，手里的完整项目却没多几个。

我把这件事重新整理了一遍，做成了一套开源的 Agent 学习指南。

这套指南目前包含 23 篇 WorkBuddy 内容、37 篇 Coze 内容，以及 628 篇编程与架构文档。后续还会持续更新Codex、豆包工作、千问办公等Agent教程。

你可以从第一次认识 Agent 开始，一路学到办公实战、智能体搭建和企业应用开发。不绕弯子，先把地址放出来。

建议两个都收藏。平时学习直接看网站，想查源码、提建议或参与维护就去 GitHub。

![Agent 学习指南｜从入门到真正让AI帮你干活](https://mmbiz.qpic.cn/sz_mmbiz_jpg/zTBLgCayWtcuEV9KU6p0USR5xSbUdTnf4Ba87GSRpGL26FbRJog0agtAWltAFFQDt6H8ElcSvu5hBkCoy4Nicibeyw5ibic4a6qibDTMdofawDNs/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=0)

*Agent 学习指南｜从入门到真正让AI帮你干活*

## 为什么建议收藏。
现在缺的从来都不是 Agent 教程。网上随便搜一下，安装教程、提示词模板、工具测评一抓一大把。麻烦在于这些内容通常各讲一段。有人教你如何问豆包，有人教你写提示词，还有人上来就讲复杂工作流。每篇单独看都能学到东西，放在一起却接不上。这份 Agent 学习指南把三段路连在了一起。

- 第一段让 AI 帮你完成电脑里的日常任务。
- 第二段教你搭建能够调用知识库、插件和工作流的智能体。
- 第三段继续补编程、数据库、中间件和系统架构，让做出来工程化的 Agent 可以接进业务系统。

你不用先想明白自己要不要转行做 AI，也不用一上来啃完所有概念。先挑一个眼前就能用上的任务，做完以后再往下走。

这条路线对小白友好，对已经在做项目的开发者也有用。

![Agent 学习路线｜不用一上来就学所有工具。按照下面四步边学边做，很快就能完成自己的第一个 Agent。](https://mmbiz.qpic.cn/sz_mmbiz_jpg/zTBLgCayWtcuKxFffuvk3K4KsyWiccmtb52QicEtL6BdPD2y53T9dC63Zt1JOXIVLrs7vicnb5ZjMJrKicRXB3VhXPWZVpFwG8hR2k8HmuTGbAs/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=1)

*Agent 学习路线｜不用一上来就学所有工具。按照下面四步边学边做，很快就能完成自己的第一个 Agent。*

## 第一部分先学 WorkBuddy，让 AI 接手具体任务。
普通聊天工具最常见的用法，是人把材料复制进去，AI 给出一段回答，剩下的操作还得人来完成。

WorkBuddy 可以进入用户授权的工作空间，读取本地文件，理解任务要求，调用工具处理材料，再把结果写回指定目录。接上连接器以后，它也能访问腾讯会议、邮箱等外部服务。

项目里的 WorkBuddy 指南没有停在功能介绍。目前整理的 23 篇内容，从工作空间、安全边界、专家、专家团和 Skill 开始，很快就进入真实工作任务。

![认识核心能力，掌握 Skill、文件、连接器、数据分析、移动端和自动化任务。｜自媒体案例](https://mmbiz.qpic.cn/mmbiz_jpg/zTBLgCayWtcKAeTgd3AXBZlvxUCMem2n9Fu6A2ooicPle3jpqy9ZIjUd4CzrsHVoBZemQKxQgPyAFK0Q2PmH8Ff3taTXCl7JPxOVWJoE5k7I/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=2)

*认识核心能力，掌握 Skill、文件、连接器、数据分析、移动端和自动化任务。｜自媒体案例*

你可以照着教程整理图片、归档发票、生成会议纪要、分析销售明细、制作 PPT、整理资讯简报，也可以继续学习定时发送邮件、手机远程控制和自动化任务。

![WorkBuddy 常见问题｜WorkBuddy 和普通聊天机器人有什么区别?](https://mmbiz.qpic.cn/mmbiz_jpg/zTBLgCayWtcm7VDH6Ur9P6Vl1icZBQrBHrzrpy16YSbMibe8q4P3rR9hkoyTot7C7RolNCtDMAeLOtGG3ibvULn9eqJlFe2rqC1ONnTHe0lLb4/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=3)

*WorkBuddy 常见问题｜WorkBuddy 和普通聊天机器人有什么区别?*

对自媒体创作者，项目还单独整理了一条内容生产路线。

从知识库检索、选题、大纲和文章复核，到小红书图文、标题、标签和 60 秒短视频脚本，整套流程都能找到对应案例。

这部分最适合边看边做。先拿一个自己的文件夹或一张表格练手，任务跑通以后，再把步骤整理成 Skill。下一次遇到同类工作，可以直接复用。

## 第二部分学习 Coze，搭出自己的Agent应用。
会让 AI 回答问题以后，很多人会继续追问。怎样给它固定的人设和规则，怎样接入自己的资料，怎样调用外部工具，怎样让一项复杂任务按照步骤自动执行。这正是 Coze 部分要解决的问题。

目前项目中有 37 篇 Coze 内容。前面的 AIGC、大模型和 Agent 基础，负责把概念讲清楚。

后面的提示词、插件、知识库、记忆、卡片、工作流和发布渠道，负责带你把智能体搭出来。

![AI基础知识｜Coze基础入门](https://mmbiz.qpic.cn/sz_mmbiz_jpg/zTBLgCayWtd9AvFSwg6wZialRiakzxDKk9liaWHJloW9znhvibedp0l7Jn2kX0Cuxhh968INCLE6Zriap5mLt5DHPGIUP0o1EqnVEVAkLAhLCA6w/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=4)

*AI基础知识｜Coze基础入门*

学完功能以后，还有内容改写、数据分析、热点监控和视频生产等案例。

![AI基础知识｜Coze基础入门](https://mmbiz.qpic.cn/mmbiz_jpg/zTBLgCayWtfAogG2f5mjeXfa3PrbU0evoXECB9xnKnJ5kesRkfOiadFIbuF9zZ5wxdQESsiceiboBf9ZZLy9tVOnkEciagn54wKDOCJiaTVsvFME/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=5)

*AI基础知识｜Coze基础入门*

这些案例的价值在于，你能看见一项任务怎样被拆开。用户提供什么信息，知识库负责什么，插件在什么时候调用，工作流怎样安排先后顺序，最后又怎样检查结果。

以后换到别的 Agent 平台，界面可能变了，这套判断仍然能继续用。

## 第三部分补工程能力，把 Agent 接进业务系统。
很多 Agent 教程做到演示成功就结束了。

可一旦进入公司环境，问题会马上多起来。数据放在哪里，接口怎样调用，缓存怎样设计，消息怎样可靠传递，用户量上来以后系统能不能撑住，出了问题又该从哪里排查。

这也是我在项目里保留完整编程与架构专题的原因。

这一部分目前有 628 篇 Markdown 文档，覆盖编程、设计模式、MySQL、Redis、Elasticsearch、常用框架、中间件、业务架构、应用架构、系统案例和开发规范。

![Java 基础、集合、并发、JVM与Netty，建立扎实的后端编程能力。｜理解创建型、结构型和行为型模式，提升复杂代码的可维护性。](https://mmbiz.qpic.cn/sz_mmbiz_jpg/zTBLgCayWtf1jf62DI4R3mQzfdYKSvmKPp8cNMysMUnqWf4HNO1VEqmicWlD7YatsvBezeiabr8vib5wm54ebtia3r3yUvWEa11949wmn1wANXI/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=6)

*Java 基础、集合、并发、JVM与Netty，建立扎实的后端编程能力。｜理解创建型、结构型和行为型模式，提升复杂代码的可维护性。*

开发者没必要按照目录从第一篇读到最后一篇。准备做知识库，可以先看数据库和搜索。准备接入已有系统，可以去看框架、接口和应用架构。项目碰到什么问题，就回到对应章节补什么。Agent 做到这一步，才有机会从个人演示进入稳定运行的业务应用。

## 不同的人，学习顺序也不一样。
如果你第一次接触 Agent，可以先看 AI 基础，再从 WorkBuddy 的图片整理、会议纪要或 PPT 案例中选一个。

先完成一次任务，比连续看十篇概念更有用。

- 如果你是职场人、运营人员或内容创作者，可以直接进入 WorkBuddy 的办公与自媒体案例。找到自己每周都在重复的工作，照着案例跑一遍，再根据手里的资料修改任务要求。
- 如果你想搭建智能体，可以先学 Coze 的提示词、知识库、插件和工作流，然后完整复现一个案例。
- 如果你是开发者或架构师，可以把 Coze 当作 Agent 入门，再按项目需要进入 Java、数据库、中间件和架构专题。

这套指南没有要求所有人走同一条路。你现在卡在哪里，就从哪里开始。

## 谁在维护这个项目。
汤师爷，长期专注 AI 智能体方向，目前在大厂从事 AI 架构工作。

过去 14 年，我先后在华为、阿里巴巴等公司参与大型互联网系统建设，也受邀担任过 QCon、IAS、A2M 等大会讲师，出版过畅销书《零基础搭建自媒体 AI Agent》和《SaaS+AI 架构实战》。

我熟悉企业系统怎样设计，也一直在研究普通人怎样把 Agent 用进日常工作。这个项目把两部分放到了一起。前面解决会不会用，后面处理怎样做成稳定应用。

## 为什么要把它开源。
Agent 工具更新很快，界面、模型和功能都会变化。一份固定不动的教程，用不了多久就会出现旧截图和旧步骤。把项目放到 GitHub，内容可以持续维护。读者发现问题，可以提交 Issue。手里有成熟案例，也可以通过 Pull Request 补充进来。

项目采用 MIT 开源协议。保留原始版权声明和许可声明以后，你可以使用、复制、修改和分发项目内容与源码。

在线网站已经做好顶部导航、分级侧边栏、文章目录、深色模式和移动端适配。普通读者打开网页就能看，不需要先安装开发环境。想研究网站源码或参与维护的朋友，可以从 GitHub 克隆项目。

本地站点基于 VuePress 2、Vue 3、Vite 和 TypeScript 构建，也提供了开发、构建和打包命令。

## 这份资料更适合拿来用。
Agent 学得好不好，最后还是要看它帮你完成了什么。整理一个文件夹，做完一份会议纪要，跑通一次数据分析，搭出一个知识库智能体，再把它接入自己的业务。这些结果会一步步带你理解提示词、上下文、工具调用、工作流和系统设计。所以，别急着一次读完 600 多篇内容。

先打开网站，选一个今天就能动手的案例。遇到看不懂的概念再往前补，任务跑通以后继续做下一个。如果这份指南对你有帮助，欢迎去 GitHub 点一个 Star。发现写得不清楚的地方，也欢迎提 Issue。项目地址再放一次。从一个具体任务开始，比继续往收藏夹里塞链接有用得多。

最后的最后，一定要记得 star 哟~。
