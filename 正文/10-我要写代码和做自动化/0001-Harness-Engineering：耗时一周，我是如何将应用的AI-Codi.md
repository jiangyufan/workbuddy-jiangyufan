---
title: "Harness Engineering：耗时一周，我是如何将应用的AI Codi"
source: "https://workbuddy.jiangyufan.com/index/hub/case/692"
type: "case"
chars: 6289
sections: 4
figures: 0
chapter: "10-我要写代码和做自动化"
---

# Harness Engineering：耗时一周，我是如何将应用的AI Codi
## 二、Harness Engineering 是什么。
1. 1 从 Prompt 到 Context 到 Harness：

三次范式跃迁。AI 工程实践正在经历三个清晰的演化阶段：

Prompt Engineering（2022-2024） 关注的是单次交互的优化——如何通过 Few-shot Learning、Chain-of-Thought、角色设定等技巧，让模型在一次对话中给出更好的回答。它的核心隐喻是"写好一封邮件"。

Context Engineering（2025） 向前迈了一步，关注的是"给 Agent 看什么"——动态构建的上下文窗口中应该填充哪些文档、对话历史、工具定义和 RAG 检索结果。Shopify CEO Tobi Lutke 将其类比为"给邮件附上所有正确的附件"。这一阶段的核心突破是认识到：模型的表现上限取决于上下文的质量，而非 prompt 的措辞。

Harness Engineering（2026） 则站在更高的抽象层次，它不再只关注"一次对话"或"一次上下文窗口"，而是设计跨越多个会话、多个 Agent 角色、多个执行阶段的完整系统架构。正如 OpenAI 工程师 Ryan Lopopolo 在其团队用 Agent 构建百万行代码产品后总结的那样："Agents aren't hard; the Harness is hard."。

一个完整的 Application Owner Agent 定义包含以下五个核心模块：

模块一：角色与项目背景（Role & Project Context）。开篇明确 Agent 的身份定位："你是某某应用的 Owner，是整个项目的第一负责人。"紧接着是项目的核心背景信息——模块结构、技术栈、关键中间件、核心业务约束（如价格字段类型、时间格式规范等）。这段信息控制在 20-30 行以内，提供"刚好够用"的项目视野，避免信息过载。

模块二：配置中枢索引（Configuration Hub Index）。这是"地图"的核心部分。用结构化的表格列出 .harness/ 下 Rules、Skills、Wiki、MCP 四大组件的路径、职责、触发场景和更新频率。Agent 通过这张索引表，能在任意阶段快速定位到需要加载的知识。例如 Skill 索引：

技能。路径。触发场景。request-analysis。.harness/skills/request-analysis/。需求分析阶段。coding-skill。.harness/skills/coding-skill/。编码实现阶段。expert-reviewer。

.harness/skills/expert-reviewer/。评审循环阶段。unit-test-write。.harness/skills/unit-test-write/。单元测试编写。unit-test-ci。.harness/skills/unit-test-ci/。

CI 流水线验证。deploy-verify。.harness/skills/deploy-verify/。部署验证阶段。

索引中还包含 Wiki 知识库的推荐阅读路径（快速上手、业务开发、数据对接、部署运维），以及 MCP 外部工具的集成配置。这种结构确保 Agent 不需要"全局扫描"来寻找知识——它始终知道该去哪里找。

模块三：七项核心职责（Core Responsibilities）。Owner Agent 的职责被精确定义为七个维度——需求理解与澄清、任务拆解、任务分发与协调、任务验收、质量把关、文档管理与知识库维护、知识问答与团队支持。每项职责都附带具体的行为准则。例如"任务拆解"要求明确每个子任务的目标、范围、输入输出、验收标准和依赖关系；"质量把关"要求关注变更对线上稳定性的影响，必要时主动要求补充单元测试或集成验证。

1. 2 为什么不能只靠模型本身

Anthropic 在其 Harness 工程博客中系统总结了 Agent 在复杂项目中的四种典型失败模式（Failure Modes）：

Failure Mode 1: One-shot Syndrome（试图一步到位）。Agent 拿到复杂需求后，倾向于在单个上下文窗口内完成全部工作。当实现进行到一半，上下文已被消耗大半，模型开始出现 Hallucination、循环输出、格式错误的 Tool Call。Anthropic 的经验数据表明，上下文窗口的 Sweet Spot 在 40% 以下的填充率；超过此阈值，输出质量快速衰退。

Failure Mode 2: Premature Victory Declaration（过早宣布胜利）。Agent 完成部分工作就宣布任务结束，核心功能尚未实现或验证。这在实践中极为常见——Agent 输出"编码完成"，但实际上编译都无法通过。

Failure Mode 3: Premature Feature Completion（过早标记功能完成）。Agent 认为功能已实现但未做端到端测试验证，部署后才发现关键路径不通。Anthropic 的解决方案是引入 Browser Automation（Puppeteer MCP）进行自动化的端到端验证截图。

## 三、AI Coding 的现状与挑战。
在进入实践之前，有必要正视当前 AI Coding 在企业级项目中面临的核心挑战。这些挑战不是某个特定项目的个案，而是所有试图将 Agent 引入存量代码库的团队都会遇到的系统性问题。

1. 1 大型存量代码库的认知负担

企业级 Java 应用通常具备以下特征：代码量在十万行以上，技术栈涉及 RPC 框架（HSF/Dubbo/gRPC）、流程编排引擎（LiteFlow/Temporal）、配置中心（Diamond/Apollo/Nacos）、分布式缓存（Tair/Redis）、数据库中间件（TDDL/ShardingSphere）等。业务链路层层嵌套，模块间的依赖关系错综复杂。

对于 Agent 来说，这种认知负担是灾难性的。它不知道某条链路是高频变更区（过去一年有数十次 XML 改动），不知道某个全局配置类在项目中有近百处引用，不知道某些字段有隐含的类型和单位约束——这些"隐性知识"（Tacit Knowledge）散落在团队成员的经验中、群聊的历史消息中、未入库的会议纪要中。

正如 OpenAI 团队在百万行代码实践中总结的：Agent 的知识边界等于代码库的文件边界（The agent's knowledge boundary equals the repository's file boundary）。如果某条架构约定不在代码库中以机器可读的形式存在，对 Agent 来说它就不存在。

在四要素架构的基础上，Harness 体系需要一个"大脑"来串联一切——这就是 Application Owner Agent（应用 Owner）。它是整套体系的编排中枢，直接与开发者交互，负责从需求接收到交付验收的全流程调度。

Agent 定义文件存放在 .harness/agents/ 目录下，是整个 Harness 体系中信息密度最高的文件，通常在 400 行左右，承担着 Anthropic 所说的"Index & Map"职责——它不是百科全书，而是一张精心设计的地图，告诉 Agent 在什么阶段该去哪里找到什么知识。

模块五：沟通原则与硬性约束（Communication Principles & Constraints）。最后部分用"必须做到"和"禁止做的"两张清单定义 Agent 的行为边界。"必须做到"包括：任何工作开始前必须优先读取规则文件、每次变更前先理解现有代码逻辑、任务验收必须有可验证的证据、代码变更必须同步文档。"禁止做的"包括：不在未理解需求的情况下直接动手、不跳过验收直接交付、不隐瞒执行过程中发现的问题、不做超出需求范围的过度重构。

这种 Agent 定义方式的本质是将一个资深开发者的工作习惯和决策逻辑编码化。它不需要 Agent "学习"如何成为一个好的项目 Owner——它只需要严格执行定义文件中的每一条指令。这正是 Harness Engineering 的核心理念：用外部化的结构约束替代对模型内在能力的依赖。

1. 3 上下文架构：分层加载，按需获取

上下文管理是整个体系的地基。我将项目知识按加载时机分为三个层次：

L1 — 会话常驻层（Always Loaded）。包括 Agent 定义文件（约 420 行，承担 Index & Map 职责）和三份 Rules 文件。提供全局视野和基本约束，但总量严格控制——遵循 Anthropic 的经验，避免上下文窗口填充率超过 40%。

L2 — 阶段触发层（Phase-triggered）。进入需求分析阶段时加载 request-analysis Skill；编码阶段加载 coding-skill 和 8 份分层编码 Spec（覆盖 Controller → Service → Domain → DAO → Adapter 全链路）；评审阶段加载 expert-reviewer。每个阶段只加载当前需要的知识。

L3 — 按需查询层（On-demand）。Wiki 知识库中的业务文档不会主动加载，Agent 根据任务需要自主查阅。这保证了上下文的"新鲜度"和针对性。

这种分层策略的核心考量是：让 Agent 在任何时刻都拥有"刚好够用"的上下文（Just-enough Context）。对于中间件繁多的企业级应用尤其关键——如果把 RPC 规范、流程引擎组件写法、配置中心规范全部一次性塞给 Agent，信息过载反而会导致注意力分散和幻觉。

1. 1 质量维度对比

维度。无 Harness。有 Harness。需求理解偏差。Agent 经常误解需求意图，编码方向跑偏。通过 spec.md + 用户确认点，偏差在评审阶段前被拦截。编码质量。语法正确但业务逻辑有隐患。评审环节拦截了渠道判断缺失等潜在线上问题。

测试覆盖。Agent 往往跳过测试或写形式化测试。实际需求产出 18 个有业务价值的测试用例，CI 全通过。过程可追溯性。无记录，改了什么全靠记忆。每个需求有完整的变更文档链，任何人可随时回溯。流程一致性。因人而异，因需求而异。10 阶段流程无论需求大小一致执行。

1. 2 AI 代码率：从 25% 到 90% 的跃迁

下面这组数据来自内部 AI 代码度量平台，分别取 Harness 体系引入前（3 月）和体系运转成熟后（4 月）的周度统计，形成了清晰的前后对比：

![](https://mmbiz.qpic.cn/sz_mmbiz_png/j7RlD5l5q1zW5vGkSgXJicIPN04QOcr6QR5Qy1raByyufIpKXPWEibc5F5qDszMuDsSNZGfj4Uyqh7xC2cDibmYIvGMLPcBO0O3viccSzcxDP68/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

## 一、为什么要聊 Harness Engineering。
2025 年是 AI Coding Agent 全面爆发的一年。Cursor、Claude Code、Copilot Workspace、Windsurf 等产品让开发者第一次真切感受到 Agentic Coding 的力量——Agent 不再只是补全几行代码，而是能理解需求、规划方案、跨文件编辑、运行测试，甚至发起 Pull Request。

Anthropic 在其《2026 Agentic Coding Trends Report》中指出，开发者在日常工作中已有约 60% 的时间在使用 AI 辅助，但能够"完全委托"给 Agent 的任务比例仅为 0-20%。这个巨大的落差揭示了一个核心矛盾：模型的原始能力已经足够强，但从"能力"到"可信赖的工程产出"之间，还横亘着一道系统性鸿沟。

当我们把 Agent 放进一个真实的企业级代码库——十几万行代码、多条业务链路交织、技术栈涉及 RPC 框架、流程编排引擎、配置中心、分布式缓存等中间件——很快就会遇到一个普遍的困境：Agent 写出来的代码往往"语法正确、风格统一，但业务语义上存在微妙的错误"。它不知道某个配置项在全项目有 85 处引用，不知道某个链路是高频变更区，不知道价格字段必须用 long 类型且单位为分。这些散落在团队经验中的隐性知识，从未被系统化地记录下来。

Failure Mode 4: Cold Start Problem（环境启动困难）。多次会话间缺乏持久化记忆，每次新会话需花大量 Token 重新理解项目结构，真正用于编码的 Token Budget 被严重挤压。

这四种失败模式的共同根源是：Agent 缺乏外部的结构化约束（Structured Constraints）和反馈机制（Feedback Mechanisms）。Anthropic 进一步指出，Agent 存在一个根本性的能力缺陷——"Agents are incapable of accurately evaluating their own work"——它们无法准确评估自身产出的质量。Harness 的作用，就是通过外部化的控制系统来弥补这一缺陷。

1. 3 四根支柱

综合 Anthropic 的长时间运行 Agent 工程实践和 OpenAI 团队用 Codex 构建百万行代码产品的经验（3→7 人团队，产出 ~1M LOC，1,500 PRs，人均 3.5 PRs/天，效率提升约 10 倍），Harness Engineering 可以归纳为四根支柱：

支柱一：上下文架构（Context Architecture）。Agent 应当恰好获得当前任务所需的上下文——不多不少。OpenAI 团队早期犯过一个典型错误：将 AGENTS.md 写成了百科全书，结果"所有内容都重要 = 没有内容重要"。后来他们改为将 AGENTS.md 控制在 ~100 行，作为索引和地图（Index & Map），指向更深层的 Design Docs、Architecture Specs 和 Quality Criteria。上下文分层加载、按需获取，是 Harness 性能的基石。

1. 3 对未来的展望

Harness Engineering 仍处于快速演进的早期阶段。以下方向值得持续探索：

Harness 的自我进化（Self-evolving Harness）。当前 Harness 的优化依赖人工发现问题和手动修改规范。未来可以让 Agent 自动分析历史失败案例并提出规范改进建议，形成 Closed-loop 的自我进化能力。

跨项目的 Harness 模板化（Cross-project Harness Templates）。当前 Harness 是针对特定项目定制的，但其中大部分设计（10-Stage Pipeline、Review Loop、Change Management）具有通用性。将其抽象为可参数化的"Harness Template"，能够让新项目快速复用。

更精细的 Agent 角色矩阵（Agent Role Matrix）。随着模型能力和 Harness 的成熟，可以引入更多专业化角色——Performance Auditor、Security Scanner、Documentation Sync Agent 等——形成 Multi-agent 协作体系。

存量代码库的渐进式 Harness 引入（Incremental Harness Adoption）。如何为有着十年历史的遗留代码库引入 Harness 而不被海量技术债告警淹没，是行业公认的开放问题。渐进式、模块化的引入策略值得深入研究。

1. 4 结语

AI 编码的兴起并没有取代软件工程的工艺——它抬高了工艺的门槛。当模型能力越强、所能触达的复杂度越高时，对 Harness 的要求也越严格。正如 Anthropic《2026 Agentic Coding Trends Report》所预判的：未来的工程竞争力将不再取决于谁的 Prompt 写得更好，而是取决于谁的 Harness 设计得更精密、更可靠、更具可演化性。

## 四、Harness Engineering 实战。
下面进入最核心的部分——我在一个真实的企业级 Java 应用（代码量 10 万+行，技术栈：Java 1.8 / Spring Boot / LiteFlow / HSF / Diamond / Tair）中，如何从零构建起完整的 Harness 体系。
