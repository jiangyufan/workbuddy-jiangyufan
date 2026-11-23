---
title: "DeepSeek不限额的用法，都在这里了 | 附指南"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/755"
type: "tool"
chars: 3102
sections: 3
figures: 0
chapter: "09-我要省模型成本"
---

# DeepSeek不限额的用法，都在这里了 | 附指南
![](https://mmbiz.qpic.cn/mmbiz_gif/dCG7OC48IfLW7ndIkrUw5dj1V1xPqOLKGBDdFO65h7CWibNjeT9xuXvFB9fhkGPmkGqTLHoG7dRibpR37FwHEe7JvVrIXSzsVuMSa0sAKOmSs/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

DeepSeek，开始限制使用了。

过去两天，越来越多人发现，自己用了快两年的免费 DeepSeek，突然开始弹出「使用额度已达上限」。有人的长对话无法继续，有人聊了不到两个小时就触发限制。

![①关于我们｜DeepSeek限额，激起的反弹比想象中还大](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfJ2I4hJGNcxWRke0b3iatHqlzecxeFdopojAIUaUje5h4oHXkjce259sxdZmicbz0a0necusAfIhFR74nAhLqIyYBWrhBLQAw4OA/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*①关于我们｜DeepSeek限额，激起的反弹比想象中还大*

用户彻底怒了，甚至涌入应用商店给 DeepSeek 打下差评，并表示自己在DeepSeek 聊天窗口里已经积累数十万字，一起和 AI 完成连续几周的故事就这样不能继续了。

目前，免费对话的 DeepSeek 存在的主要限制包括：长对话无法续聊：超过 7 天不活跃的长对话不再支持，系统会提示导出历史数据。输入字数限制：单次输入文字上限缩短至 4 万字左右。每日额度上限：限制每日对话总次数，达到上限后提示「服务器繁忙」，需次日恢复。

好消息是，如果你真的愿意花钱继续用 DeepSeek，其实有个「不限额」的用法，不是邪修，正儿八经的官方渠道。

今天，APPSO 就来手把手教大家，即便从来没有接触过 API 这个概念，普通用户也能学会花钱接入，把之前的聊天记录一起搬过去，给 DeepSeek「开会员」。

## 调用 API 并不麻烦。
大多数的网友可能听到 API 就觉得复杂，它的全称是 Application Programming Interface 应用程序接口，我们可以简单地把它理解成我们使用 DeepSeek App 要输入的登录凭证，即手机号和密码/验证码。

此前用于登录 App 的手机号，可以理解为 DeepSeek 给每个手机号分配了一定的免费额度，而 API 的额度，则是需要我们自己去充值。

充值的方式也很简单，在 DeepSeek 的官方网站找到「API 开放平台」，点击之后，使用手机号或者直接微信授权登录。

![探索未至之境｜问点什么，一起探索](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfKjicSG29ribFrZLDeibVuichRSkVhH4TN9zckKB1TxGkP4FJ4ZFARRLzUyZNJfcHp9azeAscFXITFicHseuEib2k68G0LfvplZxGfyQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*探索未至之境｜问点什么，一起探索*

在 DeepSeek 开放平台首页，左侧边栏依次是检查每日使用情况的「用量信息」、「API Keys」、「充值」、「账单」，以及底部的 API 接口文档和产品定价等信息。

![deepseek 开放平台｜B 接口文档](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfI7CYYb2gsGNjSibfb91ITYZy1TYM4pWBk571sUPjxT2eGCfXh8FPfDKuqNsfaf2CSLZhAocz9wRGibE2IzRYglzcicqbxOaIuOUo/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*deepseek 开放平台｜B 接口文档*

如果你还没有创建过 API，第一步可以是到充值页面，使用微信支付或支付宝充值对应的金额。

![deepseek 开放平台｜金额将充入当前帐户 (136********33)](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfJooLTWseFAVyHXcmyKwXSokzyNMYszyLM4fs7WqAoibicn7nHvzialmTfBDrlZDQQdSu656hLpXNsOmwNVbxMWyibCUdtIpBzKGyY/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*deepseek 开放平台｜金额将充入当前帐户 (136********33)*

根据当前 DeepSeek Flash 和 Pro 模型的定价，Flash 模型的版本为 DeepSeek-V4.1-Flash-1017，Pro 模型的版本则是 DeepSeek-V4-Pro-0813。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfLHiboO5cbveQicnSic12QRcVN3QInNzpJdiciby04ia9icwYDqeyZplpMmrqOlfNXvnOybupdCJxlnQDsyYsAFERajoiagY0SzRGuMsXQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

以在高峰时段使用 DeepSeek Flash 模型为例，我们在 DeepSeek 官方的 Agent 平台内把推理等级调到最大的 Max 档位，发送提示词「帮我深度研究最近市面上在卖的笔记本，有什么比较推荐的，6000 块左右的，给我一份网页报告。」。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfKvJEYrSfjxMMUUeLKCxGRZpKibib589JSxRQbjJeCFmPEgcVyZFO1w4Yrjcy3NZl4fyVuX3LcEAiaFjWGdOPcad7fR6N2lolEjibo/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

DeepSeek 最后花了 19 分钟，一共消耗了 5564 万 Tokens，其中 99.3% 累计 5504 万 Tokens 都是缓存命中，未缓存命中的输入是 38.1 万 Tokens， 输出 20.9 万 Tokens，因此按照每百万 Token 的定价，计算的花费则是 （输入 38.1 * 2 + 输出 20.9 * 8 + 缓存 5500 * 0.04）/ 100（百万单位） = 4.634 元。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfJvdrwn2iaCaXtwTE5SakiaoicnAdicsIB2pk0hHCE0AWNlARW0wN7RwDcnjzeG93vamfGu0ibdsvr7juQrFgjbBlMaNkqLh2V62IRc/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

在开放平台也能看到消耗的金额在 4.92 元，其中还有 tool-search 等费用。目前联网搜索（文字、图片）和网页抓取均按次计费，一次 0.005 元，我们在这轮测试中使用了 38 次 tool-search，即 0.19 元。

这就是大多数人第一次用 API 的感受，「为什么我只是发了一句你好，后台就显示扣掉了几毛钱。」。

如果你充值 50 块，类似的深度研究任务大概只可以完成 10 次。模型的输入不仅仅是我们发送的提示词，还包括随请求发送的历史对话等上下文，而 Tokens 也不等于中文字数。此外，还有缓存命中会降低输入成本，联网搜索等工具费用则另计。

![开启新对话｜帮我深度研究最近市面上在卖的笔记本，有什么比较推荐的，6000块左右的，给我一份网页报告](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfLG1PSZKQgxjpsGg2hictDrXb2WnALL6FOA394JhiceibnS5VuibMKoNBcGP1ozRxicCibAhv4AD8wvmxQMZVMdrA3g2Lgor64HyaEy8/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*开启新对话｜帮我深度研究最近市面上在卖的笔记本，有什么比较推荐的，6000块左右的，给我一份网页报告*

而如果我们只是想在对话里面使用，并不涉及到 Agent 等流程，Token 的消耗会大幅减少。同样的问题，我们在问答的 DeepSeek 内，它只是用了 6s 就为我们生成了答案，花费 0.17 元，其中 tool-search 16 次花费 0.08 元，消耗 Token 67038 个花费 0.09 元。

Token 计费为（输入缓存命中 3.17 万 * 高峰期 0.04 + 未命中缓存输入 3.15 万 * 高峰期 2 + 输出 0.31 万 * 高峰期 8）/ 100 = 0.089 元。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfJAOc1bw1R9xicj9hIdrnoOcb86QcDnu6c8uMFU0bsYEZoneh9hhGAA2TtJvU4gjElHuichPdmDvC2ZD8uRSgpr1L6Kbf2sBa9ic0/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

![输入(命中缓存)｜输入(未命中缓存)](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfJ2THAgMy0mv8NtVLXicnXdicicCqOsvR3mtfh9wuFq7ktgNv8IYHuzctxf8H1T0x2sCSggEXcPYiby7afelS2pcFS1BPFkUo63rwk/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*输入(命中缓存)｜输入(未命中缓存)*

因此，单纯想复刻此前的 DeepSeek App 或者网页版内的使用体验，50 块钱可以支撑我们将近 300 次这样的提问，并且是开启了「深度思考」和「智能搜索」的情况下。

搞清楚 API 的收费规则之后，我们就可以放心去充值了。DeepSeek 账户有余额的情况下，创建的 API Key 就可以正常使用，API Key 就像是你的登录密码一样，是一串由 sk- 开头的密码。

一旦 API Key 泄露，被有心的人使用，就有可能把我们刚刚充值的金额全部消耗光。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfJcuN7SKDibzFGL7hvhacWEGwibVbHqrBo4GauyXZUzGkI7YdFbw0lwaCIhakcmZCt9eicILqF4WVSWaNFibDLJibxTNpVGZJQMGTT8/640?wx_fmt=png&amp;from=appmsg#imgIndex=11)

API Key 只会显示一次，不过即便不记得了也可以重新再创建一个，把之前的删除。目前 DeepSeek 开放平台最多支持保留 300 个 API Key，足够大部分人的使用。

## 官方的电脑版 App。
有了 API Key 后，最简单的方法，是直接下载 DeepSeek 官方的 Agent 平台，DeepSeek Harness。

![现在，开箱即用｜无论处理日常工作、编写代码，还是构建自己的 Harness，都可以从这里开始。](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfKUvpJ5emMbicjzc0I3FQp87dHkPmCGWhN1NwbdhrALTfa3Pbaunfpr5WZia3r6OyGex0picd2ic80tkqxhTOKMicBkngYI8hCictPMQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=12)

*现在，开箱即用｜无论处理日常工作、编写代码，还是构建自己的 Harness，都可以从这里开始。*

目前，DeepSeek Harness 也支持直接登录 DeepSeek 开放平台的账号，并使用开放平台的余额。登录之后，我们在设置的「账号与余额」里面，就能看到对应的在 DeepSeek 官方开放平台充值的金额。

而在 API Keys 的管理界面，也会有一条显示是「App-managed」，由 Harness 管理的 API Key。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfLbjHXnsz9ibYdbmXibibia7hLa9MscRS2qn9NjOTTLrURKSWUHM1wvfo5NgOcgPSOic3icHnpE33dSJZt0Lt5KH9Cu8WrTve001pzcw/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

选择不使用账号登录，我们也可以填入对应的 API Key，之后就能正常开启对话。

![浏览器太空探索游戏｜创建一个可直接在浏览器游](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfLsDFXwM8EIIvjDmYibfX0DicLTvRMhdibdXPeSrHuQ1ibWsYGCAQDpwWEO4YeQXHUZW7dECPvoQBME7WusYH6uwEREDJzKzVsZ8rI/640?wx_fmt=png&amp;from=appmsg#imgIndex=14)

*浏览器太空探索游戏｜创建一个可直接在浏览器游*

创建不同项目的工作区，在工作区内开启「新会话」，选择模型、推理等级，以及是否启用智能体团队协作等，我们就能像在 DeepSeek 网页版里面一样，不受限制（API 余额充足的情况下）和 DeepSeek 地开启聊天对话。

无论一起创作互动小说、文字游戏，还是让 DeepSeek 进行角色扮演和情感陪伴，现在都不会再受到官方 App 开启限额的影响。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfKLzUffr1TZ3evHq1Cg1jajxFib2IMhZvTdDuicIr9dq177WLOt16nCkjeSzCQpBb4U3NTKlCx9XeSClMe2ickuWyFj04AacguSJI/640?wx_fmt=png&amp;from=appmsg#imgIndex=15)

并且，最新版本的 DeepSeek Harness 也提供了一键导入 DeepSeek 会话的插件。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfJGwE7T77ZIeaNuPKT4rmVLNgiaX3iawm5A1r4vfQpZURVneZcyz8ISQOLgFgIhZ1NcicDYclwVpGEib9TvjMqPMqCa2zm2jzibXMu4/640?wx_fmt=png&amp;from=appmsg#imgIndex=16)

## 手机替代也有官方开源项目。
如果我没有电脑，我只是想和之前一样在手机上用 DeepSeek App 呢。

在限额事件发酵前几天，DeepSeek 就刚刚宣布开放全家桶应用 API。这次更新把联网搜索、文件输入、网页阅读和语音等功能开放给开发者。官方甚至表示，开发者可以用 API 复刻完整的 DeepSeek App。

同时，DeepSeek 还提供了支持导入历史聊天记录的开源聊天客户端。

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfJibk2d0TnUGr3jJdnkZXibIaF81icL37kaGXRn1CYJXIzZOQNdKExickRjf2OvzGk2TassHBbStUoL3m1E4vL0icAtYbHLC6UQLCWw/640?wx_fmt=png&amp;from=appmsg#imgIndex=17)

![](https://mmbiz.qpic.cn/mmbiz_png/dCG7OC48IfIGMhNz99TIOqVoF9Pk0S4RcOlIdsfPk1U06qOEK7H0erakrsdFQZZFQXwebOutpbQlLMiaC6E4O9OmJ08JVNicfETtjWicviaZfFI/640?wx_fmt=png&amp;from=appmsg#imgIndex=18)

DeepSeek 新上线的 Chat Demo 还提供了导入历史对话的功能，我们可以直接从 DeepSeek App 内找到设置里的数据管理，导出所有历史对话，再将导出的对话导入到新的 DeepSeek Chat Demo 中。

具体的方法如下，在原有的 DeepSeek App 内，点击导出对话之后，我们会得到一个下载链接，复制该下载链接到浏览器中打开，就会自动下载一个 ZIP 的压缩包。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfL4xzrB7Eo4W5RibRQtRQtgdsG4IDpdicjPRdKOgCudyC0qGDCSy026ly1XhNCDLzZS0LuRRkwiaFUxfrYWdI2hYLhJicDibiaeaWhvE/640?wx_fmt=png&amp;from=appmsg#imgIndex=19)

接着回到我们使用 API 的 Chat Demo 中，找到设置里的数据管理，将此前下载的压缩包导入，需要注意的是，上传的历史对话会覆盖当前所有对话记录。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/dCG7OC48IfIldQ8ahwjWV6UvDJp7o8Up0rl0ne7cohrIaVqPavl4W1N7lBjB2VHib1ib6XSwUicmztu2YgLEWgMW6cWng8c9dSiaO0pCEI2jbzg/640?wx_fmt=png&amp;from=appmsg#imgIndex=20)
