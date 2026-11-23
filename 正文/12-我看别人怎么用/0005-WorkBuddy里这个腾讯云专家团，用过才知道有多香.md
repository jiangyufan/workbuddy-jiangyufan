---
title: "WorkBuddy里这个腾讯云专家团，用过才知道有多香"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/393"
type: "skill"
chars: 3637
sections: 3
figures: 0
chapter: "12-我看别人怎么用"
---

# WorkBuddy里这个腾讯云专家团，用过才知道有多香
现在云上运维真的越来越难了，最近我就看到一个需求，某SaaS公司要做一次完整的AIOps评估，具体云上结构有一些复杂。

他们的业务同时跑在多朵主流云上，内部有4个云账号（生产、测试、合规、集团子公司账号），彼此权限隔离。IT 团队面对这个复杂的结构，想搞清楚当前架构的健康度到底多少分。风险点和整改路径怎么梳理。

![集团子公司｜应用层 数据层](https://mmbiz.qpic.cn/sz_mmbiz_png/wkNoAv8MEu3082bANSLLbmvZcTdlmxh5HApoXZDjCX10zibFTID5rrEH3U5EbYkUic15z2pV93lULMGOWjZvL51avia5ejjGCAtzicPW7hicpcXs/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*集团子公司｜应用层 数据层*

如果按传统做法，多云架构梳理、权限/计费/安全审计、风险识别和整改建议，哪一步都少不了，等完整报告出来，几天都过去了。

但我用CloudQ跑了一遍，10分钟就产出了一份专业度很高的评估报告。也正是这次体验，让我真切感受到AIOps正在改变企业IT治理的节奏。

![资料库·灵感｜你正在为一家中型股份制银... 5天前](https://mmbiz.qpic.cn/sz_mmbiz_png/wN8W4W5WQLH9oW16dHvicUnrmqR4LV9hc753DXWAicHKeF2Fuh55c8l51iaB2oXyj1ShnibRJOpGY1GH6J2Aib0gC9O2nyooCypnHPibYwLKRGMibw/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*资料库·灵感｜你正在为一家中型股份制银... 5天前*

## 企业AIOps中，CloudQ都能做什么。
CloudQ是腾讯云推出的多云AIOps专家，核心解决的是多云资源管理、根因分析和诊断、持续风险发现、多云多账号管理和FinOps优化等问题。

腾讯云把过去十几年沉淀的云上技术经验，沉淀到了CloudQ的专家能力中。它从企业云上治理视角出发，覆盖多个核心场景。

多云多账号管理：跨云、跨账号资源可视化，统一治理视角，拉通其他主流云环境的资源与风险。目前CloudQ已支持腾讯云、阿里云、AWS，其他等多朵云正在内测。

高可用：架构治理、风险评估、容量规划，把"事后整改"转成"事前预警"。FinOps：成本结构分析、TCO 测算、资源优化建议，让云支出有据可依。安全合规：风险面扫描、合规基线对齐、差距报告输出，把合规压力变成日常动作。故障应急：告警聚合、根因定位、预案联动，把 MTTR 从小时级压到分钟级。

上云规划：现状扫描、目标架构推荐、迁移路径设计，把上云 / 换云从拍脑袋变成有蓝图。下面就用开头提到的多云、海内外场景，看一下CloudQ的评估效果。

# SaaS 平台生产架构描述 ## 一、业务概况 - **业务类型**：面向企业客户的 SaaS 平台 - **业务范围**：核心交易、用户管理、内容服务、数据分析四条主要业务线 - **服务对象**：中大型企业客户，按行业划分（金融、零售、教育、制造等） ## 二、多云部署情况 业务按"业务条线"做了多云拆分，主要云环境为 **3 朵主流公有云**： | 云环境 | 主要承载业务条线 | 部署规模 | |---|---|---| | **云 A** | 核心交易 + 用户管理 | 主生产环境 | | **云 B** | 数据分析 + 内容服务 | 独立生产环境 | | **云 C** | 备份 + 容灾 + 部分边缘业务 | 异地灾备环境 | **网络互联**：云间通过专线打通，组成统一的企业内网，业务请求可在云间调度。## 三、账号结构 按"集团总部 + 集团子公司"口径做了账号隔离： | 账号 | 角色定位 | 权限范围 | |---|---|---| | **集团总部账号** | 集团统一管控 | 全集团资源可见，统一计费 | | **子公司甲账号** | 主营业务运营方 | 主营业务相关资源 | | **子公司乙账号** | 创新业务运营方 | 创新业务相关资源 | | **公共账号** | 共享资源管理 | 中间件、监控、日志等公共资源 | 账号之间**权限完全…

我给CloudQ的提示词很直接：

请基于以上生产架构，输出一份企业级AIOps评估报告，重点覆盖架构健康度评分、多账号资源归集、风险点清单、整改路线图和跨云一致性改进建议。整改路线按周维度给出动作节奏和主题即可，不需要列具体产品配置。

CloudQ已经在WorkBuddy的专家中上线，我们直接搜索“多云AIOps专家”就能找到，点“召唤CloudQ”就能开始使用。

![WorkBuddy 编辑 ( E 窗口 W ) 帮助(H)｜专家 专家服务](https://mmbiz.qpic.cn/mmbiz_png/wN8W4W5WQLG0MqX3bmtMXUkxox9bicN8x7DC84Nk0MZuiaReQsYBhHvQ4GQJAMnMJOsF5gIH8U3bTNdIjsibLlej0P7ql0yN4JubItVicahoouk/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*WorkBuddy 编辑 ( E 窗口 W ) 帮助(H)｜专家 专家服务*

我们直接将架构和需求发送给CloudQ，就直接得到了完整的评估报告，同时也在WorkBuddy中给出了核心信息的摘要：

![](https://mmbiz.qpic.cn/mmbiz_png/wN8W4W5WQLGz8SLel5ibI9J2QIlCqSLDiaEQEFR36COiaRib6EwTTnNeYBTYqU2HyciaVQLGFDas6cm4rthCC7uvS8l3qtJTpUmm55GfzTZEhmO0/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

除了输出MD格式的报告，它还支持生成多种格式的报告，比如我就可以让它生成HTML格式的报告。

![输出html格式报告](https://mmbiz.qpic.cn/sz_mmbiz_png/wN8W4W5WQLEx45I4Hnbiaye8cPkGY3ibyqua8yDBCicXkeXeiaKXanBLZwhsNUtMyicaA6SES7iabTZicrRtaANFNYwzfpXr2Zd3aVQk9Ztiag1icOg0/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*输出html格式报告*

![企业级 AIOps 架构评估报告｜SaaS 平台多云生产环境 —基于智能顾问 CloudQ 框架分析](https://mmbiz.qpic.cn/mmbiz_gif/wN8W4W5WQLFibAQd8DTeGp2icMKfNibWbia6k2S8oAwMd8qbnEbx2VBRNkYeCu7fkpIr42sBHr9Gf77gmibwsIlWUIIu40gxzIKSYeNrqyYwBIGk/640?wx_fmt=gif&amp;from=appmsg#imgIndex=11)

*企业级 AIOps 架构评估报告｜SaaS 平台多云生产环境 —基于智能顾问 CloudQ 框架分析*

注：多格式报告是WorkBuddy的能力，以上内容有WorkBuddy加工效果，具体呈现效果以具体使用的工具为准，但由CloudQ提供的核心内容不变。

这份报告最让我感觉专业的地方，是CloudQ不仅给出了评分，还给每个支柱的权重配了理由说明，方便业务侧判断评估是否合理。

整体来看，它的价值主要有三点：

指标明确，每个评分和风险都有依据；可执行性强，12周路线图能直接拆任务；实操性高，能把三朵云统一到一套治理方案里。

对企业来说，报告分数本身不是最重要的，关键是CloudQ能把评估结果转成可执行路线图，直接拆到项目管理工具里。

在多云多账号管理场景下，它可以拉取各朵云、各账号的资源数据，生成事前评估报告，提前给出架构健康度、关键风险点和整改建议。

![CloudD:多云AIOps专家｜多云多账号](https://mmbiz.qpic.cn/mmbiz_png/wkNoAv8MEu0NDLLNDf7icIhph83Fiasht0jaavboyrkiatmibH3ic8L8zGm7fv2NF66IJNn8HgcFRp3Oy0icAPoVyLe37QOPCcCov3zl4cYBjYsHk/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*CloudD:多云AIOps专家｜多云多账号*

## 单Q不成林。
真实云上场景不只有AIOps治理，还会涉及故障排障、迁移评估等不同需求。

在WorkBuddy的专家体系中，腾讯云还提供了「腾讯云技术支持专家团」能力，包括CloudQ、AndonQ和MigraQ三个独立Agent，分别面向不同技术支持场景：

CloudQ：面向企业级AIOps，重点覆盖高可用治理、多云多账号管理、FinOps 优化等场景。AndonQ：面向售后支持和生产排障，帮助用户在故障发生后快速定位问题、调用接口、推进处置。MigraQ：面向迁移评估和迁移实施，帮助企业完成跨云资源对标、TCO 测算和迁移路线规划。

三个Agent分别覆盖云上治理、售后排障和迁移规划场景，形成互补关系。

![腾讯云技术支持专家团｜上云前/中](https://mmbiz.qpic.cn/mmbiz_png/wkNoAv8MEu0T7nwPlQMg1ibmicdibFINia05w6eic4FyGSIGvWfickAGAG3qDqHtvwgDaNOIicg5WC30d8Wx6b1rSovViauFsDpS6drF1KReSlERcFQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*腾讯云技术支持专家团｜上云前/中*

## AndonQ和MigraQ能做什么。
看完CloudQ之后，我也顺着体验了专家团里的AndonQ和MigraQ，下面给大家简单介绍一下它们的作用。

CloudQ更偏事前治理和持续评估，但生产环境不可能完全没有突发故障。故障发生后，就更适合交给AndonQ来处理排障处置问题。

传统工单体系下，用户需要提交工单、等待人工客服响应，紧急情况下可能30分钟起步，甚至等待数小时。而AndonQ可以提供7×24小时实时答疑，对话体验更接近即时通讯。

![关于故障排查，清单太长了我看不下去，你直接告诉我我要怎样排查故障就可以了。｜好的，不需要看那份长报告，直接照下面5步做就行:](https://mmbiz.qpic.cn/sz_mmbiz_png/wN8W4W5WQLH0y7H9CMxEglSLibw318HHmAIfJYGkZQVTUcLkSO3F1LSKZDmP1KWqthuib4KPSRfFGzZ5GKibyUtMArEK1duJNOIrL2GhJgI160/640?wx_fmt=png&amp;from=appmsg#imgIndex=15)

*关于故障排查，清单太长了我看不下去，你直接告诉我我要怎样排查故障就可以了。｜好的，不需要看那份长报告，直接照下面5步做就行:*

同时，AndonQ不只是问答工具。

它可以结合腾讯云产品知识库、API示例和tccli能力，帮助用户查询平台事件、确认监控数据、检查实例状态。

它和普通AI客服的差异主要有三点：支持OAuth2鉴权和SSE实时流式问答、对接腾讯云全产品线知识库，回答可带出处和API示例、支持tccli全API自然语言调用。

不过AndonQ并不能完全取代客服，它更像是给客服团队提供一条7×24小时应答的AI通道。

![AndonQ不只是AI客服｜知识库带出处](https://mmbiz.qpic.cn/mmbiz_png/wkNoAv8MEu0pR2mw4rmGnwF4uHhXhvoRy09No9MO6oSSPIrXtO5y6ibTbcjFntsFvCJEibYr17ZCVOVC7JbOa80tXp5wQL2fknyVET82HygWI/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*AndonQ不只是AI客服｜知识库带出处*

CloudQ更适合回答“当前云上架构哪里需要治理”，MigraQ则更适合回答“如果要迁移或重构，怎么迁、成本多少、风险多大”。

企业在选择迁云时，通常要先调研、再选型、再做TCO、再排路线图。MigraQ可以根据企业现有资源和业务目标，生成迁移方案、TCO测算和阶段性迁移计划。

这里我让MigraQ生成了一份从某云迁移到另外一个云的迁移方案：

某在线教育SaaS公司在某云跑了4年，最近想评估迁到另外一个云的可行性与TCO，他们希望在不增加预算的前提下，同时提升性能和稳定性。

我还准备了一份资料清单：

# 某云资源清单（待迁移至XX云） ## 业务背景 - 某在线教育SaaS公司，日活50万，在某云运行4年 ## 资源清单 当前主要资源包括ECS、RDS MySQL、Redis、OSS、SLB、NAT网关和CDN； 月费用约12.7万元；课程视频和用户头像等对象存储约80TB； CDN月流量约150TB；跨云专线已开通1Gbps。## 业务关注点 - 迁移期间不能停服（影响 50 万日活） - 跨云专线已开通 1Gbps - 希望评估：能否在不增加预算的前提下提升性能和稳定性。

然后把资料清单以及需求发送给专家团，提示词为：

请基于以上某云资源清单，给出XX云迁移方案， 包含资源对标建议、TCO测算、迁移路径、RTO/RPO目标、跨云专线带宽评估，以及6个月迁移计划。

![WorkBuddy 本次会话预计消耗4.39 ~ 117.1 Credits｜◎已读取资料清单.txt L1-末尾](https://mmbiz.qpic.cn/sz_mmbiz_png/wN8W4W5WQLFC397MucMkmb7Md6VOGwbjoIWl9kXniajLR18VSBVicibaIibvLvorBiaMy1yqQ1vIf87MRziacVYf9PhfRPhlT0JjiccS3hH60hdnHs/640?wx_fmt=png&amp;from=appmsg#imgIndex=21)

*WorkBuddy 本次会话预计消耗4.39 ~ 117.1 Credits｜◎已读取资料清单.txt L1-末尾*

专家团把这项任务分配给MigraQ处理，并最终产出迁移计划。WorkBuddy还进一步用图表展示了相关数据，关键结论会更直观。

![阿里云与腾讯云月度 TCO 对比｜阿里云月费¥127,100](https://mmbiz.qpic.cn/sz_mmbiz_jpg/wkNoAv8MEu3VEvt7GWVdN0Uphs4K6oibNtIa9SgloIEuD9XKbdM2aicIEBXIV0PXwweicJxQX7UDnESnGrxY6mpIBwAyiaRW0h2UYibQnkVnOQAM/640?wx_fmt=other&amp;from=appmsg#imgIndex=12)

*阿里云与腾讯云月度 TCO 对比｜阿里云月费¥127,100*

![M1 环境搭建 & 数据同步启动｜VPC/专线/DTS/COS/CDN 创建·负责人: 网络工程师/DBA/运维](https://mmbiz.qpic.cn/mmbiz_png/wN8W4W5WQLFRn4Wtia3pt5EPFnyxJ6rZzibBAHfQGDbOTWP01x5Cpe9kNhVyicTiccfPiaCkqTqo06hSibAt0iae7GcN0Zz9TxuXubgxfRnxOptSM8/640?wx_fmt=png&amp;from=appmsg#imgIndex=20)

*M1 环境搭建 & 数据同步启动｜VPC/专线/DTS/COS/CDN 创建·负责人: 网络工程师/DBA/运维*

![跨云专线 1Gbps 带宽利用率分析｜专线容量1Gbps](https://mmbiz.qpic.cn/sz_mmbiz_png/wN8W4W5WQLGQmLib45iao8fk1Wopdic3SORCnQ1UiaTBD5nsSQMA7AFMbRJQfm6f257M0UfdAZLGZzia06pdhNVRdUUlSufZnMq2djl6Sb8B4hMU/640?wx_fmt=png&amp;from=appmsg#imgIndex=21)

*跨云专线 1Gbps 带宽利用率分析｜专线容量1Gbps*

MigraQ最终给出的方案里，最关键的结果是一年节省约32万元，并且给出了详细迁移计划和带宽测算。

比如面对50万日活、80TB OSS、MySQL、Redis全量同步这种组合，很多人可能会直接判断“需要升级到10Gbps”。
