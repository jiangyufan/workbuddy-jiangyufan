---
title: "律师业这样用WorkBuddy就对了"
source: "https://workbuddy.jiangyufan.com/index/hub/case/577"
type: "case"
chars: 3310
sections: 4
figures: 0
chapter: "03-我是律师法务"
---

# 律师业这样用WorkBuddy就对了
![](https://mmbiz.qpic.cn/mmbiz_jpg/dMfDY1ub6d7keoEGUnEWj2FYiamb4gEywNI4Vsricz2sxwkN65np8ia7ic7wHKtgwsMfmhusVLJnVDicxhLePuSggcQ/640?wx_fmt=jpeg#imgIndex=0)

律师业包括了律师事务所以及法律服务，根据公开信息，全国的执业律师人数也在逼近90万，大体市场环境就是大型所寡头化，中型所逐渐消亡，小型所杂货铺。

这种行情下，竞争比的已经不只是专业功底，还有单位时间的产出效率。然而大部分律师的时间都是被一堆写不完、看不完的东西占据着。

想起21年的时候，老马接触过一个上海的律师机构，主任明确表示AI解决不了法律问题。一晃过了5年，如今的大模型早已不是当年的智障，我们也得用发展的眼光看待事物。

## 01 合同审查初筛。
合同审查初筛。

## 03 起诉状答辩状。
起诉状答辩状。

## 04 归档与纪要转待办。
归档与纪要转待办。01 · CHAPTER ONE。场景一：合同审查初筛。场景痛点。

合同审查是很多律师和律师助理都躲不掉的日常工作，一份几十页的合同逐条通读下来，半天时间就没了。其中大部分时间都花在逐条扫描、找要素、对格式这种体力活上。

在使用WorkBuddy帮我们进行合同的初筛审查之前，先别把合同一丢过去就说帮我审一下，那样得到的只会是AI生成的泛泛的格式意见。

更靠谱的做法是把审查工作拆分成几层，每一层只干一件事。先检查格式和完整性，再标注出关键条款位置，然后按我方的立场做一些风险分级，最后才输出修订的建议。

这样每一层的产出都能单独进行核对，错的地方也知道错在哪儿，也能随时暂停下来，人工进行二次的复核。实操方法。

在WorkBuddy新建个任务，最好是同时创建工作空间，把合同文件放在工作空间对应的本地文件夹里面。然后把下面的提示词模板，根据你的实际情况稍作微调，再发送过去处理：

. . . 提示词模板。你是一名协助律师做合同初审的助理。我方是一家设备采购方，先读取工作空间中的《设备采购合同》文件。

请你分三步来做：第一步先做格式和完整性检查，看看主体信息、签署页、日期、金额大小写这些要素有没有缺失或不一致；

第二步找出付款条款、交付与验收、违约责任、知识产权归属、保密义务、争议解决这几个关键条款，注明它们在文档里的位置；

第三步站在我方采购方的立场做风险排查，凡是单方解除权、无限连带责任、模糊的验收标准、对我们不利的管辖约定，都按高、中、低三级标注。

最后汇总成一张风险清单表格，每条写清条款位置、风险等级和理由。先不要改合同，只做标注和提示。

![日常办公 代码开发 设计创意｜开学新Buddy，事事都挺你，认证大学生尊享积分好礼](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTHadYwnLEvP0BfphT6FlDO2GHcGxOJhl3u14cuddnUjibOeafLE1Pgibul4FCXykbe2YhY6GCw2yOPsT0BKqMSMyrS5keA22BibGo/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*日常办公 代码开发 设计创意｜开学新Buddy，事事都挺你，认证大学生尊享积分好礼*

该场景下的需求推荐安装的Skill有两个，第一个是智能销售/采购合同审核Skill：contract-risk-reviewer，在WorkBuddy的专家技能链接器里面，切换到技能即可搜索到：

![专家 技能 连接器｜推荐 SkillHub 套件](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTFTr0ZHQU0yibtzz5pic0hfzqbVG1TUXK1QwrPGAmhL2M7eic6djkZlDW1QE1st2cojZjyTY1vxbanhYLxRuluVTRRcQ3MxvibE9zw/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*专家 技能 连接器｜推荐 SkillHub 套件*

但这个Skill支持的合同类型有限，虽然可以做到按红线条款、付款、违约做合同风险分级和修改建议。老马觉得你可以在这个Skill的基础上，改成支持其它合同类型的Skill，只不过这里面要给的规则和流程就麻烦一点。

好处是改后的Skill是你专属的，且只需要修改一次，后续可以直接复用。现在这个现成的Skill，就纯当成模板来作为参考。

第二个Skill是腾讯电子签合同AI助手，支持合同起草、审查、对比、签署、查看、法条检索、审查列表、对比列表八大能力：

![专家 技能 连接器｜推荐 SkillHub 100 套件](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTFYPd0SsLvgss0elLvsFyPSnDJEIK4mTAMZQVwBEQLDDFZhzb87BvnkBYy6icKjtU6k9eXq5Qr3QDdy7UcahT5Q5UYqU3zLXRuc/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*专家 技能 连接器｜推荐 SkillHub 100 套件*

这个Skill相对来说能力就全面一些，WorkBuddy的Skill Hub里面还是有非常多的法律类Skill的，挑选上需要花点时间，不建议同时装太多，可以测试后选择去留，以免占用太多上下文。

需要注意的重点是，AI的输出只是初筛和标注，不能构成审查意见。风险条款要怎么改，违约金约定多少合适，取决于交易背景和谈判地位。这部分的判断必须由律师自己做，另外合同属于客户敏感信息，在发给AI之前应该按照所在律所的保密规范事先处理，必要的话先做脱敏。

02 · CHAPTER TWO。场景二：类案检索。

办案前的类案研究是最耗费时间的工作内容之一，需要人工通读几百页判决，手动整理裁判规则，每次研究耗掉半天时间很正常。但这个场景最近多了一条新的高压线，AI编造案例。

湖北宜昌西陵法院今年7月份在庭审中发现，代理律师提交的案例材料大部分是由AI生成的不实案例，案号和案件对不上、法条被篡改，律师被当庭训诫。

这就有点尽信AI的感觉，AI不是案源库，AI可以作为检索的工具，帮你梳理好路线，但起码的案号还是得人工二次审核的。

使用AI梳理检索关键词，案由方向，相关法条和裁判规则思路，然后律师再拿着这份路线图去官方数据库按图索骥，对AI的使用要从搜索引擎化转向检索线索化。

在WorkBuddy中新建任务，参考以下提示词模板，把需求改成自己的实际需求，发送过去处理即可：我在办一起买卖合同纠纷，我方是卖方，争议焦点是买方以质量异议为由拒付货款。

请帮我做一份类案检索的路线规划：围绕这个争议焦点，列出可以用的检索关键词组合、对应案由，以及可能相关的请求权基础法条，。

再给我最近三年这类案件里值得重点关注的裁判规则方向，比如质量异议的提出期限、验货义务的分配这些角度。

注意：你只给我检索思路和路线，不要给我编任何具体案号，法条要注明现行有效的版本和出处，我会拿着这份路线图自己去裁判文书库里核实。

![日常办公 代码开发 设计创意｜致敬好老师，送你 Buddy 好搭档，认证老师尊享积分好礼](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTHxF3Kr6MiakyicJS3SwWP1ALofymicEgdFMxIFCaDauQrlG2StRiarHRibsEsHpP4AmvkWajXIzEINfCc011wogicdhibKH487yox8gw/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*日常办公 代码开发 设计创意｜致敬好老师，送你 Buddy 好搭档，认证老师尊享积分好礼*

拿到AI生成的路线图后，再人工逐条到中国裁判文书网、人民法院案例库这类的官方渠道进行核实，核对一条用一条。

Skill的话推荐安装legal-citation-verify，法条查询及多源核验,这个Skill技能就是专门查法条和核验条文的：

![专家 技能 连接器｜⑧我安装的](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTEs22LJoatjGQCyQsXgWWxribMjibtalUYxlvgboWl3LrnX0TtB2gxicaqWiccwQWrsbRXRZTNHmj7fnicSyxaRg00nc7wSvEpFjRh4/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*专家 技能 连接器｜⑧我安装的*

可以对法律条文和司法解释做多源交叉核验，标注出处，核查是否现行有效，还内置了反幻觉约束和法务场景的输入脱敏要求，等于是在AI和官方文本之间加多了一道核对工序。

与此同时还可以在专家里面搜索召唤法检Pro，这位专家会按法源位阶检索法规与类案，验证效力，评估相似度，并最终输出可溯源的报告。适合案值大，检索要求高的案子：

![专家 办 技能 0 连接｜专家 专家团](https://mmbiz.qpic.cn/mmbiz_png/iaC8bMtQHCTHf7ESEnbS1vks4bpX93gaGFQWbfaFmXdcKeA5c1J7yYxjy8qpv2hIoydbtL4ibdPlU1FZCVbU4iboXlgG4lL4ZFVFicAEzgia4Rtk/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*专家 办 技能 0 连接｜专家 专家团*

03 · CHAPTER THREE。场景三：撰写起诉状答辩状。起诉状、答辩状这类文书的格式固定，但每次从头开始写还是很折磨人，改个几版是常事，虽然有些可以套模板。

事实要素整理、格式框架、证据位置标注，这些内容可以交给AI处理，但法律论证和诉讼请求的最终设计，是律师的智识核心，必须得律师自己写。

最稳妥的流程是律师先把案件事实用条理清晰的方式整理好喂给AI，AI按照规范格式输出初稿骨架，律师检查事实陈述和证据对应关系，最后亲自把关论证部分。

在WorkBuddy中新建任务，参考以下提示词模板，把案件事实改成自己的实际情况，发送过去处理即可：

我现在要起草一份买卖合同纠纷的民事起诉状。案件基本情况是这样的：原告是我们公司，被告拖欠货款 38 万元，。

合同约定 2025 年 12 月 31 日前付清，逾期按日万分之五支付违约金，我们催讨过两次，都有微信记录。

请你按法院通用的民事起诉状格式搭好框架：当事人信息部分留出待填位置，诉讼请求把本金、违约金、诉讼费承担都列上，。

事实与理由部分按时间顺序整理成一段通顺的陈述。有两个要求：法条引用你只给建议并注明需要核实，不要直接写死；

事实陈述里每一处需要证据支撑的地方，都在旁边标注我们应当提交哪份证据，比如微信记录、合同原件、送货单这些。

![@ 代码开发｜开学新Buddy，事事都挺你，认证大学生尊享积分好礼](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTFyo1MUHuIMj5K8MibfZiaCV27SSwhE05iaYgCPRHXZOxvUp6LRKpiae7SWIkk6vmVxXicL44DaicMwc8fb5nF0uPp58yicUWJd2aVqak/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*@ 代码开发｜开学新Buddy，事事都挺你，认证大学生尊享积分好礼*

有关这个场景推荐的Skill还是不少的，legal-document-writer法律文书助手Skill，可以用于起草民事、行政、刑事的起诉状、答辩状等文书，内置了国标公文排版规范，一键输出格式规范的Word底稿：

![专家 高技能 连接器｜C.ral-document-write! × ☑ 我安装的](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTFIellicjJVspkrlAFgh2efmzW4960GNZjIogAzh9zakfjqjjL6ciaORCYh74sJLXEto0fibujibyGVWQN9lNnvXQobDeJcfvt8Qz8/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*专家 高技能 连接器｜C.ral-document-write! × ☑ 我安装的*

element-complaint-filler要素式法律文书一键生成Skill，它内置了最高法67类要素式示范文本（民商事、执行、行政、刑事自诉等），按案由自动匹配模板填写要素：

![专家 办技能 连接器｜推荐 SkillHub 1000 套件](https://mmbiz.qpic.cn/sz_mmbiz_png/iaC8bMtQHCTFB8Ottp6X4U1M8jEnLbaaBzjNFRRXSmcR1MYOY83ZSjLy3z3GQpick6qgUXNxFkkMeqMic1iclFeItQILobnZRws8ibmtbQfHFQ7c/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

*专家 办技能 连接器｜推荐 SkillHub 1000 套件*
