---
title: "在WorkBuddy里白嫖Qwen 3.6：100万上下文，一分钱不花"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/673"
type: "tool"
chars: 1506
sections: 4
figures: 0
chapter: "09-我要省模型成本"
---

# 在WorkBuddy里白嫖Qwen 3.6：100万上下文，一分钱不花
![白嫖百万上下文境大模型｜WorkBuddy配置Qwen 3.6免费教程](https://mmbiz.qpic.cn/mmbiz_png/2tmmBsrhXa0JnaHb7SibLP1Sc0iaHD8orNNXlVImTgjMqFwV4EkH6FicPY4XwhliacRUHkkNRpuv4EPa3kLtia3vA17htgqVMHAb2p947fJtItFk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*白嫖百万上下文境大模型｜WorkBuddy配置Qwen 3.6免费教程*

Qwen 3.6 Plus Preview 昨天上线了 OpenRouter，免费，100万 token 上下文。

我试着配到了 WorkBuddy 里，能用。记录一下过程，三步搞定。

## 第一步：去 OpenRouter 注册，拿 API Key。
打开 openrouter.ai，右上角 Sign Up，支持 Google 或 GitHub 直接登录，不用手机号。

登录后，左侧菜单点 Keys，然后 Create Key。名字随便填，比如 "workbuddy"，权限默认就行。

把生成的 Key 复制下来（以 sk-or-v1- 开头）。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/2tmmBsrhXa3SPvOZcZT2LFDDficvlib0BjWP3icK4Mrkkk4NJLzOufCWYvZeInRsMQzWCe0Mmpf5n2c3oNEia4rYxpfWtYt7GpJwzsYsHfDzbSU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

别关页面，马上要用。

## 第二步：写 models.json 配置文件。
WorkBuddy 的自定义模型配置文件是 models.json，放在用户目录下：~/.codebuddy/models.json。

也就是 C:\Users\你的用户名\.codebuddy\models.json。如果 .codebuddy 文件夹不存在，手动建一个。

也可以直接在workbuddy里说，。

![](https://mmbiz.qpic.cn/mmbiz_png/2tmmBsrhXa0ujT4l0P1F0kf6lU7I2t9pDiaeTanW6U1eDVR5mVaSglOv2tgiaaJx4TiaBkW1jx4YHJrDBtNn4grWiaM6BcAjEAVd7hkQ4Qiabk1k/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

文件内容这样写：

几个容易踩的坑：

模型 ID 必须带 :free 后缀。qwen/qwen3.6-plus-preview:free，少这个后缀会走付费通道。

API Key 不要带多余空格。复制的时候经常多带一个空格，肉眼看不见，接口直接拒绝。

url 必须写到 /chat/completions。只写到 /v1 不够，WorkBuddy 需要完整的端点路径。

API Key 建议用环境变量。别直接把密钥写进文件，改成 "apiKey": "${OPENROUTER_API_KEY}"，然后在系统环境变量里设置 OPENROUTER_API_KEY 的值。安全得多。

也可以手动配置模型，具体可以参照我的实测截图：

![仅支持 OpenAI 蒸容协议 API｜工具调用 ▶](https://mmbiz.qpic.cn/mmbiz_png/2tmmBsrhXa3tx6KiaJ5GrxYibJU8GDibMTlbj9epu1Ao3Vo0t5AhIGUUwwUMLSjMa2Qsczo9FdfhaiamCBGmsNtaXThpxzks4TkjqibIZVpoVDmg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*仅支持 OpenAI 蒸容协议 API｜工具调用 ▶*

## 第三步：重启WorkBuddy，切换模型。
配置文件保存后，重启 WorkBuddy。打开模型选择下拉列表，你应该能看到 "Qwen 3.6 Free"。选中它，发条消息试试。这里有两个模型id，其实是一个带推理，一个不带推理的快速响应模型；

![自定义模型｜+配置自定义模型](https://mmbiz.qpic.cn/mmbiz_png/2tmmBsrhXa1c0CVxVbvMRvDNMMcjd4IKHZngxjMl4PicPTqibpGWJvx1t92oYosgq1ShAZ1cOsW6icUfIOMcgsCiaTtlk3rf3PonZEuXYLFvV64/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*自定义模型｜+配置自定义模型*

正常回复就说明配好了。如果报错，按这个顺序排查：API Key 写错了。——最常见的原因，回去重新复制一遍。模型 ID 拼写不对。——检查有没有漏掉 :free。JSON 格式错了。——逗号、引号、括号，任何一个不对都会解析失败。网络问题。

——OpenRouter 国内访问不太稳定，可能需要代理。

![WorkBuddy配置教程｜三步白嫖百万上下文大模型](https://mmbiz.qpic.cn/mmbiz_png/2tmmBsrhXa3kDqsdwpOgpBtibY2el6o2uqia6BzrBlcmiaV3hVeicV3chJsCJUXfcazjcic0CocEHpblPxGJNGibzQvb2A1p2o9ynyV7cdf8dD0Gk/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*WorkBuddy配置教程｜三步白嫖百万上下文大模型*

## 免费模型的几个特点。
配好之后，有几件事你应该知道：100万 token 上下文。大概相当于 75 万中文字。一本《百年孤独》塞进去还有富余。

擅长编程和推理。Qwen 系列写代码一直不错，3.6 在代理编程和复杂问题解决上又提了一档。写代码、debug、解释技术文档，效果挺好。

免费但有频率限制。OpenRouter 的免费模型有调用频率上限，具体数字官方没说，正常使用不会触发。批量请求不适合用免费通道。

数据会被用于模型改进。OpenRouter 页面上写了，这个模型会收集 prompt 和 completion 数据用于训练。敏感内容别往里放。

预览版，可能随时调整。今天免费不代表明天免费。别把所有依赖都绑在这个模型上。就这些。2026年3月31日，WorkBuddy + Qwen 3.6 Free，实测可用。以下就是使用。

qwen3.6-plus-preview:free模型生成的封面提示词，粘贴到文生图模型中即可生成封面。

![](https://mmbiz.qpic.cn/mmbiz_png/2tmmBsrhXa1Jd7Z3ZdcibrYaaGoFYAA1O9memkC7AfR7TIvUxYjafBoWQG67ibBzbyLOqUsrV8icqibV3HBKXxKvPCIyvLGHImmKWcXTqbc0p1s/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)
