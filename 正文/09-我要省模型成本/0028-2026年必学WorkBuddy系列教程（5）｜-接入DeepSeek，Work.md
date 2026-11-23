---
title: "2026年必学WorkBuddy系列教程（5）｜ 接入DeepSeek，Work"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/440"
type: "tool"
chars: 2255
sections: 7
figures: 0
chapter: "09-我要省模型成本"
---

# 2026年必学WorkBuddy系列教程（5）｜ 接入DeepSeek，Work
## 二、第一步：去DeepSeek申请API Key。

![](https://mmbiz.qpic.cn/mmbiz_png/93as19DjlrwMLjHu9ZWTL132zauP9x2Q7sna0icsdUDIyXm8J9Q4c2dMbwbc1srLcNFM3HZyazPwjZstokm5icKbqQX8Q4tkwyFZTyx4xiawib8/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

如果你还没有账号，先注册一个，。用手机号注册就行，全程中文，不到2分钟。注册完登录，。左侧菜单有个 "API Keys"，点进去，。点击右上角 "创建API Key" → 给Key起个名字，。随便写，比如"WorkBuddy专用"→ 点创建。

打开WorkBuddy，。看左下角——有个设置图标（齿轮形状），点它，。在设置面板里找到 "模型配置"。

![本地配置文件｜+添加模型](https://mmbiz.qpic.cn/mmbiz_png/93as19DjlryYianqKlvSZCdSTO25Pwiaw45lvuWNQsmfpwDRVibA9qVbiaiaoXIxQhJuPkzVOj40t57lGJhibdtHVgQdeibQ2m0Dmiap0UVSu91bvTk/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*本地配置文件｜+添加模型*

跟着做，别跳步：

## 第1步： 点"添加模型"。
第2步： 在"模型类型"里选 OpenAI兼容（OpenAI Compatible）。为什么选这个。因为DeepSeek的API接口是兼容OpenAI格式的，。WorkBuddy通过这个选项就能直接连DeepSeek。

## 第3步： 填写以下信息：
提供商：选择"深度求索/DeepSeek"。API Key：粘贴你刚才复制的那串 sk-xxxxx。模型名称：DeepSeek-V4 Pro或 DeepSeek-V4 Flash，。

## 2026年必学WorkBuddy系列教程（5）｜ 接入DeepSeek，WorkBuddy效果飙升还省钱。
在互联网上，简单的问题，问微子，复杂的问题，问AI，不知道怎么使用AI，问微子。大家好，我是微子，自由职业者，社群成员10000+，在【微子的AI实验室】里，带大家一起研究、实践、用好AI。AI时代不焦虑，轻松入局AI。

前面四篇，。你已经把WorkBuddy装好了，。知道了三种工作模式的区别，。也开始试着跟它对话了。但有个问题你可能还没意识到——你现在用的，是WorkBuddy自带的模型。不是不好，。但如果你每天用得频繁，或者对回答质量有要求，。其实你可以接一个自己的模型进来，体验和成本都会好很多。

所以今天就手把手教你接入DeepSeek，。为什么选它。因为它目前是"效果强+性价比极高"的代表。

![![](24,109,48,129) 用量信息｜![](192,673,211,696) 联系我们](https://mmbiz.qpic.cn/sz_mmbiz_png/93as19DjlryMvzpBEkdsiaHEXCDyZ8RVWBJ3FVNlyOSC6PSp5IXkbqEibLORAjG2Sib5D2s4jId4nJFP2KWC9zDlANRtxvQCKVQuEdeBuDhUf0/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*![](24,109,48,129) 用量信息｜![](192,673,211,696) 联系我们*

注意： 这时候系统只显示一次你的API Key（类似 sk-xxxxxxxxxxxxx 这样的字符串）。

立刻复制。保存到记事本里。关掉这个页面之后，你就再也看不到这串Key了，只能重新创建一个。我第一次申请的时候，点击快了，没复制，关了页面才发现，。DeepSeek的API按Token计费，。但价格非常低，。你跟它聊一万字，成本不到1毛钱。对个人用户来说，接DeepSeek基本上是"免费"的体验。

## 三、第二步：在WorkBuddy里配置。
好了，。你手里有了API Key，。接下来在WorkBuddy里把它接进来，。

![微子·私人号｜本期:专家能量包](https://mmbiz.qpic.cn/mmbiz_png/93as19DjlrxTiaOlqt0NibuqiaLx2nWCpgNZNTAmAovWdyOgdUIcwGjoaX8Asy5WSrQichYOIKekYghbj4ibtga1CbG7Gh4nlUI1x0VqOQWJWQJY/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*微子·私人号｜本期:专家能量包*

这两个有什么区别。

DeepSeek-V4 Pro,是旗舰版，最强大脑，最稳妥，适合搞复杂的编程、数学题、长篇论文分析、企业级应用；

DeepSeek-V4 Flash，是效率版，最省心、最快、最便宜，适合日常随便聊聊、写写文案、整理资料。

第4步： 保存。配置完之后，。回到对话界面，。模型选择下拉框里就能看到DeepSeek了，。选中它，跟WorkBuddy说句话试试，。回答来了，配置成功。

## 四、多模型切换，不同场景用不同模型。
配置完DeepSeek之后，。你其实可以在WorkBuddy里接多个模型，。根据任务类型随时切换：DeepSeek-V4 Flash： 日常对话、写作、总结、翻译，极便宜；DeepSeek-V4 Pro： 深度推理、代码、复杂分析；混元： WorkBuddy自带，开箱即用，消耗平台额度；

Kimi（Moonshot）： 长文档处理、超长上下文；GLM： 中文创作、学术写作；

建议用法是：日常任务用DeepSeek-V4 Flash，需要深度思考切DeepSeek-V4 Pro，处理超长文档切Kimi。

在WorkBuddy里把这些都接进来，。对话界面随时切换，。比你每次打开不同的AI网站高效得多。模型配好了，。WorkBuddy的底子算是真正打好了。从下一篇开始，。我们要进入真正的核心功能——技能系统（Skills）。这是WorkBuddy跟其他AI助手最大的区别所在。

装了技能之后，。WorkBuddy能做的事情，。会从"聊天"变成"真正干活"，。比如操作你的电脑、读写文件、联网搜索、甚至控制其他软件......。我们把这些技能系统彻底搞懂，。下一篇见。

## 一、自带模型 vs 自定义模型。
WorkBuddy安装完后，。默认用的是腾讯自家的混元模型，。你打开就能用，不需要任何配置。但混元有个问题：它有时候太"乖"了。你让它写点有锋芒的东西，它可能给你四平八稳的官方腔，。你让它帮你做个有创意的方案，它可能偏保守。而且如果每天用得多了，WorkBuddy的算力是有限制的，。

虽然目前对个人用户还算宽松，。但哪天你用它来跑自动化任务、批量处理文档，额度蹭蹭往上飙。所以我的建议是：可以接一个自己的模型进来。好处有三个：

1. 成本：

自带模型消耗WorkBuddy算力额度，。接DeepSeek按实际调用量计费，便宜到可以忽略。

1. 效果：

自带模型偏保守，适合通用场景，。DeepSeek-V4 Flash适合创作，DeepSeek-V4 Pro适合深度推理，自由选择。

1. 隐私与稳定：

接自己模型直接连模型厂商，理论上更可控，。不受WorkBuddy平台状态影响。接自己的模型，基本上是全方位更优，。唯一的"门槛"是你需要去申请一个API Key，。但因为我会教你，所以这个门槛也几乎可以忽略。接下来我们就开始操作：
