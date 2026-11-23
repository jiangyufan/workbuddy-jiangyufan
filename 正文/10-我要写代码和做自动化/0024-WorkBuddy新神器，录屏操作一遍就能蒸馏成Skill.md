---
title: "WorkBuddy新神器，录屏操作一遍就能蒸馏成Skill"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/383"
type: "skill"
chars: 2753
sections: 3
figures: 0
chapter: "10-我要写代码和做自动化"
---

# WorkBuddy新神器，录屏操作一遍就能蒸馏成Skill
![](https://mmbiz.qpic.cn/mmbiz_jpg/dMfDY1ub6d7keoEGUnEWj2FYiamb4gEywNI4Vsricz2sxwkN65np8ia7ic7wHKtgwsMfmhusVLJnVDicxhLePuSggcQ/640?wx_fmt=jpeg#imgIndex=0)

今天刷到一个挺有意思的开源工具，一开始以为是个 Skill，后来用 WorkBuddy 装完之后，才发现是个技能生成器的本地应用。

说到制作和生成 Skill 技能，一般情况下，我们会先安装一个生成 Skill 的 Skill，比如常见的 Skill-creator，再跟模型对话去生成新的 Skill。

传统用 Skill-creator 结合会话上下文生成 Skill 时，会话里的干扰信息多，需求又容易天马行空，导致蒸馏出来的 Skill 会有损耗，质量不是太稳。

而今天要给大家介绍的这个叫 Browser-BC 的工具，它是通过人手动在浏览器里把任务演示一遍，系统把操作轨迹蒸馏成可复用的 Skill，下次 Agent 直接可以调用，不用再盲目重复尝试。

## 01 它解决什么问题。
它解决什么问题。

## 02 四步工作流。
四步工作流。

## 03 实操录制 Skill。
实操录制 Skill。01 · CONTEXT。Browser-BC 到底是什么。

Browser-BC 的目的，是给模型一段干净且完整覆盖工作流的上下文，而录屏演示就是最自然的干净上下文来源。

「你不是让模型猜流程，而是把流程亲手演示给它看。」。

当然，从它的核心工作流上可以看出，有点类似于浏览器自动化沉淀为 Skill，但又不完全是为了自动化，更多是成为一种技能。

举个例子，现在网上也有自动发文章到某平台技能，这种 Skill 没错是用到浏览器自动化操作。但其核心在于，如何把这个标准流程给跑通。

浏览器自动化只是工具，可控的流程和约束才是重点。02 · WORKFLOW。四步把操作轨迹蒸馏成 Skill。根据官方的项目介绍，Browser-BC 的核心工作流可以总结为以下四步。

操作轨迹：用户在浏览器完成一次真实操作，比如登录、搜索、填表、提交。工具通过扩展完整记录页面快照、DOM、可访问性树、点击输入、页面反馈和最终状态。

能力提取：清洗噪声，比如误点、等待、隐私信息，再按语义切分连贯子过程。

能力归桶：把提取出的过程性知识组织起来，相似意图合并、特化，形成技能图谱，也就是 Skill Graph。

技能生成：大模型把轨迹转写成结构化技能卡，只保留意图、步骤、完成判据、避坑点，剥离坐标、DOM 选择器、临时 ID、登录态等脆弱细节。

03 · DESIGN。三个关键设计点。就像 Browser-BC 的项目文件中说的那样，它有以下三个关键设计点。

不是 RPA 回放：传统的按键精灵只会录制坐标，页面一改动就废了。Browser-BC 录的是语义级说明书，页面布局变了，Agent 也能举一反三。

蒸馏与执行解耦：强模型如 Claude Opus 蒸馏一次，小模型、便宜模型也能拿着技能去执行，WebArena-Hard 上成功率从 60.5% 提升到 81.4%，ClawBench 上从 32.9% 提升到 68.4%。

贴近 Claude Skills 体系：原生适配 ~/.claude/skills/，但也明确不限于 Claude，WorkBuddy 等桌面 Agent 可迁移复用。

首先，给 WorkBuddy 发送一句话提示词，让其安装 Browser-BC 这款工具。

![先说结论：这不是一个WorkBuddy Skill｜一句话:它是个"技能生产器"，产出的技能是给Claude用的，不是给WorkBuddy用的。](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTHwGRAoWI7vIGq1Bh3bEXIEELkUJcmibljOJFtBLgcmAdZVriaJN9StQNBVcQByU9oEBBr11YkiaQaURKwAos5ryF1KRSGhuobEVI/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*先说结论：这不是一个WorkBuddy Skill｜一句话:它是个"技能生产器"，产出的技能是给Claude用的，不是给WorkBuddy用的。*

老规矩，有可能会提示你安装失败，这种情况大概率就是你的网络访问不了 Github 网站。可以给老马的公众号发送“github访问”，根据回复的文字去操作。

Browser-BC 安装完毕后，正常会在你的电脑桌面生成一个工具的文件夹，名字叫 JourneyForge-Local。

如果没有，你就问一下 WorkBuddy，这个文件夹放在什么路径。不过找不到也没关系，后续安装浏览器拓展程序的时候，WorkBuddy 也会告诉我们路径的。

下一步是让 WorkBuddy 把它真正跑起来，并且写一个WorkBuddy 适配器，提示词就是这样的一句话。

![把它真正跑起来，并且写一个WorkBuddy适配器｜服务端已在后台启动，控制面板可访问:](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTHXS2uynGD2y9T6hibzsxFCibtMZ1p86PlJotMyE7HVWNXRS99lk112stZlf1dMWM9f5FsB9XrmMXXEiby9Q5wdGNoJ7KdY6jrIpc/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*把它真正跑起来，并且写一个WorkBuddy适配器｜服务端已在后台启动，控制面板可访问:*

跑起来后，WorkBuddy 会提示我们，需要把 Playwright MCP 接到 WorkBuddy 里面，并且你还得额外提供一个模型的 API，给 Browser-BC 对接使用。

什么意思呢。就是 Browser-BC 这款工具，它得单独接入一个模型。这就要求你有模型的 API 信息，比如你之前在 Deepseek 开放平台上已经开通购买了一个 API。

老马这里也是填写的 Deepseek 的 API 信息，模型使用 deepseek-v4-flash，把对应的 API 地址和 API Key 一并发送给 WorkBuddy。

![模型id:deepseek-v4-flash 填好 key + 构建扩展｜三件事全部完成，且都经过实测验证:](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTF6G9UpNGdOVKYR8nrqJfIuht0v5UvQDsx3tfKVnHumcJjeGhlTQUKqWwVsrAlOuWraiaUbfafHh9AGKeUicAcadKe6FHy5E8aOg/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*模型id:deepseek-v4-flash 填好 key + 构建扩展｜三件事全部完成，且都经过实测验证:*

然后为了后续操作方便，WorkBuddy 提示老马，要不要写一个一键录制→蒸馏→同步的 WorkBuddy 工作流，把这几步串起来。当然可以，直接开干。

![写一个「一键录制→蒸馏→同步」的 WorkBuddy工作流把这几步串起来｜编排器:确保服务在线、校验LLM key、轮询等新录制、等蒸馏完成、调sync同步](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTFHqkiccicQ9sLcY7XwskMhNZNTR5dXkJ1hxibAibypSaQpHsSvepfxvW8gN86blesaSIiaGHWGRCvJ1457kLbueU28d3yZkHOmLJCo/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*写一个「一键录制→蒸馏→同步」的 WorkBuddy工作流把这几步串起来｜编排器:确保服务在线、校验LLM key、轮询等新录制、等蒸馏完成、调sync同步*

05 · RECORD。安装浏览器扩展并开始录制。

这一步搞定之后，老马就发送了一句开始录制给 WorkBuddy。结果发现，谷歌浏览器的拓展程序还没安装。

![现在开始录制｜请按这一步录制](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTHdh38cDf83ia8kiaNia3F9kicPPh9qAFBrlZmaicN3m30jkKSY1HK87dUoYUw2SYeE8ib7zwPq58QUp59xibLiblEaNs9G5doFoFpd1ao/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*现在开始录制｜请按这一步录制*

按照 WorkBuddy 给出的提示，这个浏览器拓展程序是已经解压好的，是一个文件夹。一般路径位于：你的用户名/Desktop/JourneyForge-Local/extension/dist/chrome-mv3。

1. 在谷歌浏览器地址栏输入：chrome://extensions 键盘回车
2. 右上角打开开发者模式
3. 点击加载已解压的扩展程序
4. 选择 chrome-mv3 目录即可安装成功

![▶扩展程序｜▶加载未打包的扩展程序](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTHuk6deFhUBwmU6dSjow87TKTI91re1w1vfJo8c6CLVKwBzSt1rQqdVIYQBuvjRibzpjSMRPDg6SDdVVLflH94mcXBib6dSeuYJU/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*▶扩展程序｜▶加载未打包的扩展程序*

开始操作之前，在浏览器里面找到我们刚刚安装好的 Journey Forge Local 拓展程序，一般在浏览器右侧的拼图图标点开，列表中就能看到。

![不需要任何访问权限｜这些扩展程序不需要查看和更改此网站上的信息。](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTEtrCV7oF1hGYiaHVbmYTv0P76xjwsbhiaefkDVo05aynTz6pKu7Scia6siaMt8BYiaYJ7IPwxy6qy72JYsYFpSia07OHTNbONwGkoDY/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*不需要任何访问权限｜这些扩展程序不需要查看和更改此网站上的信息。*

06 · DISTILL。从录制到导入 Skill。

回到 WorkBuddy，给它发送一句话，说录制已经完成并且上传了。WorkBuddy 就会去查你刚才上传的文件，整理导入成可以用的 Skill。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTEvEBsIjrUzdicb7Gpq1DfHia67TQz8ZX9TOD2K87ViaqMFicl2eW15Ed8BDxRQv4ibNBITkAo79T3I50brcelWkkKTKwJ8jhniadFiaI/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

∞ · POSTSCRIPT。这种方式更适合复杂流程。

Browser-BC 的整个操作过程可能略显复杂，但比单纯用 Skill 去制作生成 Skill 来说，这种工作流会更靠谱一些。

当然，WorkBuddy 配合 Hy3 模型效果不是最好。如果你发现录制后的 Skill 实际运行起来有问题，建议把模型切换到 GLM-5.2 或 Kimi K3 重新录一遍。
