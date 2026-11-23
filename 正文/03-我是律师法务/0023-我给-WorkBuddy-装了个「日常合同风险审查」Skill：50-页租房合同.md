---
title: "我给 WorkBuddy 装了个「日常合同风险审查」Skill：50 页租房合同"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/385"
type: "skill"
chars: 1860
sections: 6
figures: 0
chapter: "03-我是律师法务"
---

# 我给 WorkBuddy 装了个「日常合同风险审查」Skill：50 页租房合同
## 你签租房合同的时候，真的从头到尾看完了吗。
大多数人——包括我自己——都是翻到最后一页直接签字。等退租被扣两千押金、水管坏了没人修、房东说涨租就涨租，才意识到：合同里那些"小字"，每一个都是坑。

我以前也这样。直到上周我给 WorkBuddy 装了个「日常合同风险审查」Skill，把一份 50 页左右的租房合同包（主合同 + 补充协议 + 家具清单 + 物业说明）丢进去，10 分钟出了一份风险报告，标出了 6 处我根本没注意到的坑。

合同里真正贵的，从来不是房租，是那些你没看的条款。这篇就讲这个 Skill 怎么搭、怎么用，指令我直接给你，复制就能跑。

## 一、为什么租房合同是"重灾区"。
租房合同有两个特点，专门坑普通人：一是篇幅长、条款碎，主合同之外还有补充协议、附件清单，看着就头大；二是信息严重不对称，房东/中介用的都是"模板"，很多坑写进去你根本看不出来。

![租房合同6大坑全景｜签字前必须逐条核对的 6 类高频风险](https://mmbiz.qpic.cn/mmbiz_png/6pFYpvgNaSUFibMgZAMM6YmUU1icibViaKe3psqq0UUocFPlYJ7kmIbIu1bEhJgjHicnmdHWVsqhak3aQWaWNuevNBI0ykmA41MeGVFOP2NDsa1c/640?from=appmsg&amp;watermark=1#imgIndex=0)

*租房合同6大坑全景｜签字前必须逐条核对的 6 类高频风险*

我把近几年高频纠纷梳理成 6 类，这 6 类不是我拍脑袋编的，每一类都能在《民法典》里找到对应条款：划重点：押金、维修、单方涨租、转租、违约金、费用分摊——这 6 处，签字前必须逐条核对。

## 二、3 步搭好这个 Skill。
WorkBuddy 现在能一键切换 Kimi K3、混元 Hy3 等多家模型。这份合同审查我特意用 Kimi K3 的 100 万 token 上下文——一份 50 页的合同包直接整本喂进去，不用拆。（Kimi K3 于 2026/7/26 开源，据 Moonshot AI 官方公告）。

![Skill 工作原理｜为什么一份50页合同包能10分钟出报告](https://mmbiz.qpic.cn/mmbiz_png/6pFYpvgNaSWnZde00BiaU823ibmQEibcLBOcAvllrmDmUybk1b0ic2qkzRpOYGfxMYC8BAJegxSlrQdvIqQZyicKibOUYHkKrRZRAL6WNiazHViaxDs/640?from=appmsg&amp;watermark=1#imgIndex=1)

*Skill 工作原理｜为什么一份50页合同包能10分钟出报告*

搭建只要 3 步：

- 打开 WorkBuddy，新建一个 Skill，取名「日常合同风险审查」。
- 把第三节的完整指令粘贴进 Skill 的 prompt 框，保存。
- 模型选 Kimi K3（长文本吃得下），把合同 PDF / 截图 / 文字丢进去，说一句"审查这份合同的风险"。

## 三、实测：50 页合同包，10 分钟挑出 6 个坑。
我拿一份脱敏后的真实租房合同包试了。以前这种活我得一下午，还容易漏；这次 AI 跑完出报告，标了 6 处风险：

![审一份 50 页合同包:人工 vs AI｜同一份脱敏租房合同包，两种方式实测对比](https://mmbiz.qpic.cn/mmbiz_png/6pFYpvgNaSUHcWCp2Am7nvXM8YWrmYQribeuwo29Qz9pyPmuKUpHP6Sa1eIV7u25iagdfI1rrxRZUVZDC5VSFJ3Xsicq0m4GG5tQJeCLB9ME6g/640?from=appmsg&amp;watermark=1#imgIndex=2)

*审一份 50 页合同包:人工 vs AI｜同一份脱敏租房合同包，两种方式实测对比*

风险类型。合同里怎么写的。为什么是坑。依据。押金不退。租赁期内乙方任何违约，押金一律不退"。无过错也扣光，显失公平。民法典 151、566 条。维修推给租客。房屋内一切维修由乙方承担"。本属出租人义务被转嫁。民法典 712 条。随意涨租。甲方可根据市场情况调整租金"。

单方变更无依据。民法典 543、705 条。二房东转租。未出示原房东同意证明。原房东可解除合同赶人。民法典 716、718 条。天价违约金。提前退租赔 6 个月租金"。畸高可请求酌减。民法典 585 条。费用无上限。其他费用由乙方按实际情况承担"。

物业水电无清单无封顶。民法典 708 条。❌ 以前：一下午看完，还是漏了 4 个坑 ✅ 现在：10 分钟出报告，6 个坑一个不落。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/6pFYpvgNaSWp33g8pdx5XeGgdMCicq9FZXRORszdeN6tbFlic4uhWhDCLS4TpnN8evKfpRZ5h2JGcstzW9AXDoc26VcpKH9UTFLN8TV5SRPuE/640?from=appmsg&amp;watermark=1#imgIndex=3)

AI 不是替你打官司，是替你把"看不见的坑"先标出来——剩下的判断，还是你做。

## 四、完整指令（复制即用）。
把下面这段直接粘进 Skill 的 prompt 框，保存即可。它定义了审查逻辑、6 类风险、输出格式：

你是一个「日常合同风险审查专家」。当用户上传或粘贴合同文本。（租房 / 劳动 / 理财 / 买卖等），请按以下步骤审查：

1. 通读全文，识别合同类型与关键条款

（标的、金额、期限、双方义务、违约、解除、争议解决）。

1. 逐条比对以下 6 类高频风险，命中即标注：

- 押金/保证金：是否"任何情况不退"或抵扣无上限
- 维修义务：是否把出租人维修责任全推给承租方
- 单方变更：甲方是否保留随意涨租、提前收回的权利
- 转租风险：二房东是否出示原房东同意证明
- 违约金：提前退租赔偿是否畸高、远超实际损失
- 费用分摊：物业/水电等"其他费用"是否无上限无清单

1. 每条风险输出：原文摘录 + 风险等级 + 法律依据 + 修改建议。
2. 最后给一页「签字前核对清单」。

约束：只做风险提示，不替代专业律师意见；结尾标注"AI生成，仅供参考"。

![照着做，下次签合同前10分钟搞定｜WorkBuddy里建「日常合同风险审查」](https://mmbiz.qpic.cn/mmbiz_png/6pFYpvgNaSXdnzmMkIUl9qekR978Bc70iaHYfLmicYvDezLmL6MjnUibERB2HOcNb2ibT08Q7pEXxFXSsEhn0Bnf8X1A3ekB8RiaYwIQWaIlJgNE/640?from=appmsg&amp;watermark=1#imgIndex=4)

*照着做，下次签合同前10分钟搞定｜WorkBuddy里建「日常合同风险审查」*

## 五、边界提醒（很重要）。
这个 Skill 是"风险预警"，不是"法律意见"。涉及大额、纠纷、公司合同，最终一定找专业律师过一遍。

但话说回来——对普通人来说，绝大多数租房、兼职、小额借款合同的坑，都逃不出这 6 类。AI 帮你先扫一遍，至少不会被"小字"闷头一棍。

我把这个 Skill 的指令和复现步骤都放在上面了。你照着搭一个，下次签合同前丢进去，10 分钟换一份安心。
