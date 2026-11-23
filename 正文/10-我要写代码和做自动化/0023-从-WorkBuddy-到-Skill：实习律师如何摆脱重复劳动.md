---
title: "从 WorkBuddy 到 Skill：实习律师如何摆脱重复劳动"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/401"
type: "skill"
chars: 2768
sections: 4
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 从 WorkBuddy 到 Skill：实习律师如何摆脱重复劳动
- 得理：open.delilegal.com/personal/skills

![专业的法律技能，让你的AIAgent开始懂法律共11个技能｜案例检索技能](https://mmbiz.qpic.cn/sz_mmbiz_png/OoQcGCictMqU5vcjwsa1Xq55FQk0NCvbg84icX8HD0Dat8G39JqNEs8abCKFVq0eGaherq1cn7FLfmFrjJUAGoZ4rZGJ98wNOmgibd8WXFp8KQ/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*专业的法律技能，让你的AIAgent开始懂法律共11个技能｜案例检索技能*

GitHub 也值得推荐。作为最大的开源网站，可以学习很多开源项目的架构思路，有时也能看到一些意想不到的项目。

1. OCR 文档识别 Skill

这是最基础、最常用的 Skill，常见的Skill数据库应该都有已经成熟的OCR Skill，不用自己制作。这个配置很关键，尤其在处理扫描件、图片版 PDF、病历材料、证据材料时，没有 OCR，AI 很难识别具体内容，后续整理时间轴、证据目录、法律意见都会受到影响。

1. 委托手续 Skill

适合处理授权委托书、律所函、送达地址确认书、法定代表人身份证明等材料。重点是主体替换、格式统一、易错项复核。由于委托手续往往高度依赖律所模板，建议自己制作。

1. 人身损害赔偿 Skill

1. 案件时间轴 Skill

适合劳动争议、买卖合同、医疗纠纷、股东争议等事实较复杂的案件。可以要求 AI 按照“时间—事件—涉及主体—对应证据—法律意义—待核实问题”输出，帮助律师更快看清事实结构。

1. 合同审查 Skill

适合买卖合同、服务合同、租赁合同、和解协议、常年法律顾问合同等常见合同。重点是固定审查顺序，例如主体、标的、付款、交付、违约责任、解除条款、争议解决等，避免每次从零开始。

当你成功搭建起了自己的某项Skill，这项基本功也就扎实了。结语。很多人讨论 AI，总是关注哪个模型更强、哪个工具更新、哪个产品又发布了新功能。

但我更想说的是：我们不必把 AI 焦虑化，目前AI 本质上仍然是服务于工作的工具。对新手律师来说，重要的不是追逐每一个新概念，而是学会借助 AI 反过来整理自己的工作方法、提升工作效率：把零散的任务沉淀成稳定的流程，把一次性的工作变成长期复用的资产。

当然，也要避免另一种倾向：AI 依赖化。Skill 不是让我们跳过基础工作，也不是让 AI 替代律师判断。相反，它要求我们先理解一项工作应该怎么做，再把流程写清楚、把标准定明确、把风险边界划出来。只有这样，AI 才是在辅助我们成长，而不是替我们思考。

未来的新手律师，依然需要做基础工作。只是我们不应该永远停留在机械重复里。

做一遍，拆解一遍，沉淀成 Skill，再迭代打磨。这可能才是 AI 时代，新手律师真正应该学习的工作方式。

## 二、Skill 怎么来。
Skill 大致有两种来源：一种是使用别人写好的 Skill，另一种是制作自己的 Skill。

1. 使用别人写好的 Skill：参考，避免盲用

别人写好的 Skill，好处是上手快。你可以先参考它的结构，看看一个 Skill 是如何拆任务、写流程、定格式的。

WorkBuddy 内部的技能市场，已经有一些已经调试好的通用 Skill，可以直接安装或作为参考。

![WorkBuddy 编辑(E) 窗口(W) 帮助(小)｜推荐 SkillHub 菜单](https://mmbiz.qpic.cn/mmbiz_png/OoQcGCictMqVyh11gOYO2SmvAAakD3PdMXDRibCbbcRuZVdpGrnlNjdOMQKCfv6ic00WUfUzISIibYhLFh96CaVRADw5avnxAJcpkpCpUZfUrKc/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*WorkBuddy 编辑(E) 窗口(W) 帮助(小)｜推荐 SkillHub 菜单*

## 一、为什么推荐 Skill。
Skill 更像一个固定技能包：把重复、明确、稳定的工作步骤打包起来。

当然，Agent 是更能解放生产力的工具。你告诉它一个目标，它可以自己拆解任务、调用工具、推进执行。但问题也恰恰在这里：当新手律师自己的工作流程还不够成熟时，未必能判断 Agent 拆得对不对、有没有遗漏关键风险、输出结论是否全面。

而 Skill 不一样。Skill 不是让 AI 自由发挥，而是先由用户把一项工作拆成明确步骤，再让 AI 按照固定流程执行。比如制作委托手续，可以拆成：识别主体、加载模板、替换信息、复核易错项、输出文稿。对于主体替换、格式检查、批量生成、固定字段复核这类机械性工作，AI 往往比人更稳定，也更不容易因为疲劳出现低级错误。

更重要的是，写 Skill 的过程本身，就是新手律师在训练自己的工作方法。你必须先想清楚一项工作应该怎么做、哪里容易出错、最后应当输出什么，才能通过Skill的方式把它交给 AI 执行。

1. 自己写 Skill：把自己“蒸馏”出来

笔者更推荐新手律师尝试自己写 Skill。法律工作比较特殊，因为律所模板不同、老板偏好不同、业务领域不同，输出标准也不同；涉及客户信息、案件材料和合同文本时，还要注意脱敏和保密。

当工作频繁出现某一类重复性很高的任务，就可以考虑把它制作成自己的 Skill。这一步很像把自己“蒸馏”出来。也就是，你要把自己脑子里那套“我平时是怎么做这件事的”，拆成清晰步骤，交给 AI 反复执行。

依旧拿委托手续举例。律所的委托手续通常都有专属模板。签客户的时候，实习律师需要做的事情主要是把主体信息替换进去，再打印、签字、盖章、扫描归档。不用一开始就被 description、script、reference、assets 这些技术词吓住。写 Skill 的关键不是先学会所有底层结构，而是先把一项工作讲清楚：它要解决什么问题、按照什么步骤完成、最后输出什么格式、哪些地方必须复核。只要这些内容足够清晰，后续的技术结构workbuddy都会自己调整。

这个流程可以拆成：步骤。具体动作。Step 1。识别客户主体信息，判断是自然人、法人还是其他组织。Step 2。加载律所委托手续模板。Step 3。替换模板中的主体、案由、授权事项、法院或仲裁委等信息。Step 4。二次复核主体名称、身份证号、统一社会信用代码、日期、法院名称等易错点。

Step 5。输出可打印文稿，并提示签字、盖章、扫描、归档事项。

![gen_weitu.py 执行层内部流程｜㉛加载模板](https://mmbiz.qpic.cn/sz_mmbiz_png/OoQcGCictMqWSkxefjMYcVbnJ8HJ79YoTYyoPE3r2tpOuEnzDWbvJTDVmRgibUte87p2Q4NaHzC69iaJsYqktFgJxnahbg9sGdgEd2f2f0BzUI/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*gen_weitu.py 执行层内部流程｜㉛加载模板*

图 2：委托手续 Skill 的执行流程示例。

这样一个 Skill 做好以后，以后每次制作委托手续，就不需要从零开始，甚至可以批量生成。它解放的不是某一次的十分钟，而是长期重复劳动中的注意力。

## 三、推荐几个实习律师好用的 Skill。
如果刚开始做 Skill，建议不要一上来就追求复杂系统，可以先从高频、明确、可检查的任务入手。

## 从 WorkBuddy 到 Skill：实习律师如何摆脱重复劳动。
现在 AI 越来越热，腾讯也在持续加码 AI 办公赛道，推出的WorkBuddy在“PC端AI原生办公智能体”中脱颖而出，成为腾讯力挺的“新太子”。

但落到实习律师的日常工作里，核心问题其实很朴素：它能不能帮我们少做一点机械重复的活，把时间留给真正需要判断和学习的事情。我的答案是：能。但对实习律师来说，最值得优先学习的，不一定是看起来强大的 Agent，而是更稳定、更适合重复性工作的 Skill。

Skill 的价值，是让 AI 按照你拆好的流程，稳定地完成一类工作。图 1：WorkBuddy 技能市场示例。

对于法律人来说，如果想找更贴近法律场景的 Skill，也可以参考法律元力、得理等法律类 Skill 平台。在安装Skill时笔者推荐先阅读技能包的内容详情，方便后续做更适配自己习惯的配置。

- 法律元力：https://yuanli.ailaw.cn/

![法律人民的智能体加速器｜热门智能技能](https://mmbiz.qpic.cn/sz_mmbiz_png/OoQcGCictMqVaDjUIic0nepkBS2yARv7W8js2mmPIHMvaAbcUK6GhrLlcK54icUGl9pwtdHnKg9yv4yIsGZ8HGFjiaAyAvAWYYagr2ibSQWNGicjI/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*法律人民的智能体加速器｜热门智能技能*
