---
title: "WorkBuddy免费大模型接入全攻略：5个方案，一个都不花钱"
source: "https://workbuddy.jiangyufan.com/index/hub/tool/438"
type: "tool"
chars: 2558
sections: 7
figures: 0
chapter: "09-我要省模型成本"
---

# WorkBuddy免费大模型接入全攻略：5个方案，一个都不花钱
WorkBuddy 自带的模型够用吗。说实话，日常够了。但如果你想白嫖更多更强的模型——比如DeepSeek的代码推理、智谱的中文写作、Agnes AI的图片视频生成——完全可以在WorkBuddy里接入第三方API。关键是：免费。下面5个方案，我全试过了，一个都不花钱。

## 通用接入步骤（先看这里）。
不管接哪个模型，在 WorkBuddy 里的操作都一样，总共三步：

## 第一步：打开设置。
WorkBuddy 左下角齿轮图标 → 模型设置。

## 第二步：添加自定义模型。
点击"+ 添加自定义模型"，会弹出一个配置框。

## 第三步：填三项信息。
- 接口地址（URL）—— 每个模型不同，下面逐个给你
- API Key —— 去对应平台注册获取，下面逐个教你
- 模型名称 —— 必须和官方名称完全一致，大小写敏感

填完保存，刷新一下模型列表，就能在模型选择里看到新加的模型了。

## 5个免费方案逐个拆解。
1️⃣ Agnes AI —— 全模态无限免费，最猛的一个。先说结论：这是目前我找到的最慷慨的方案，没有之一。

免费政策（截至2026年6月） 6月1日起无限期免费，文本、图片、视频三模态全部开放，无Token上限，不绑卡，不限次数。新加坡AI Lab出品，全球排名前十。

- agnes-2.0-flash（文本对话）
- agnes-image-2.1-flash（文生图）
- agnes-video-2.0（文生视频）

获取 Key 步骤。

1. 打开 https://platform.agnes-ai.com
2. 邮箱注册（Gmail/QQ邮箱都行），30秒搞定
3. 进入控制台 → 设置 → API Keys → 创建密钥
4. 复制 key（只显示一次，务必先存好）

WorkBuddy 接入配置。

- 接口地址：https://apihub.agnes-ai.com/v1
- API Key：粘贴你刚才复制的 key
- 模型名称：agnes-2.0-flash（文本）或 agnes-image-2.1-flash（图片）

⚠️ 踩坑提醒 • 视频模型稳定性一般，日常用文本和图片就够了 • 高峰期偶尔会慢，毕竟是免费服务 • 免费开放后首周调用超1万亿token，服务稳定性还在持续优化。

2️⃣ 智谱 GLM-4.7-Flash —— 中文最强，永久免费。

1. 打开 https://open.bigmodel.cn
2. 手机号注册（支持微信快捷登录）
3. 控制台 → API Keys → 创建密钥
4. 复制 key

- 接口地址：https://open.bigmodel.cn/api/paas/v4
- API Key：你的智谱 key
- 模型名称：glm-4.7-flash

⚠️ 踩坑提醒 • 接口地址末尾不要加斜杠 • 免费版限1并发（同时只能跑1个请求），个人用完全够 • 支持深度思考模式（Thinking Mode），适合复杂推理 • 中文长文本任务（摘要、改写、写作）效果最好。

3️⃣ DeepSeek —— 代码和推理的王牌，行业最低价。DeepSeek整体定价是行业内最低的。新用户有免费额度，用完后按量计费也极便宜。

免费政策 新注册用户送100万token免费额度（有效期30天）。用完后按量计费：V4-Flash输入仅0.14元/百万token，V4-Pro也才0.435元/百万token，比GPT-5和Claude便宜5到30倍。

1. 打开 https://platform.deepseek.com
2. 手机号注册
3. API keys → 创建新 key
4. 复制保存

- 接口地址：https://api.deepseek.com/v1
- API Key：你的 DeepSeek key
- 模型名称：deepseek-chat（对话）/ deepseek-reasoner（推理）

⚠️ 踩坑提醒 • deepseek-reasoner 是专门的推理模型，写代码用它 • 平台有时候需要实名认证才能创建 key • 接口偶尔会繁忙，等几秒重试就行。

4️⃣ 火山方舟 Doubao —— 字节家的永久免费。字节跳动的火山方舟平台，Doubao Lite 模型永久免费，无需付费。

免费政策 永久免费，QPS限制为2（每秒2次请求），个人用怎么都够了。每日免费200万token。

1. 打开 https://www.volcengine.com
2. 手机号注册（字节系账号通用）
3. 进入火山方舟控制台 → 在线推理 → 创建推理接入点
4. 选择 Doubao Lite 模型 → 获取 API Key 和接入点 ID
5. 左侧菜单 → API Key 管理 → 创建 API Key（格式：ark-xxxxxxxx）

- 接口地址：https://ark.cn-beijing.volces.com/api/v3
- API Key：你的火山方舟 key（ark开头）
- 模型名称：填你创建的接入点 ID（不是"doubao-lite"，而是控制台生成的 ep-2025xxxxxx 格式）

⚠️ 踩坑提醒 • 模型名称最容易搞错——是控制台里的"接入点 ID"（ep-开头），不是模型代号 • 控制台操作稍微复杂，第一次用要花几分钟摸索 • 注意区分两种密钥格式：API Key是ark开头，不是sk开头 • 除了文本，还免费提供语音转文字功能。

5️⃣ 商汤日日新 SenseNova —— 公测完全免费，不用绑卡。商汤的 SenseNova 目前还处于公测阶段，调用完全免费，不需要绑任何支付方式。 免费政策 公测阶段完全免费，每5小时1500次调用配额，无需绑卡，无需实名。

1. 打开 https://platform.sensenova.cn
2. 手机号注册，验证码登录
3. 复制 key（sk-xxxxxxxx，只显示一次）

- 接口地址：https://token.sensenova.cn/v1
- API Key：你的 sk-xxx
- 模型名称：sensenova-6.7-flash-lite

⚠️ 踩坑提醒 • 接口地址是 token.sensenova.cn，不是 platform.sensenova.cn（那是管理后台），写错了连不上 • 模型名称大小写敏感，必须一模一样 • 每5小时1500次配额，超了会报429错误，等5小时自动重置 • 公测结束后收费政策可能变化，趁现在先用上。

## 横向对比，选哪个。
Agnes AI。免费类型：无限期免费 · 中文：⭐⭐⭐⭐ · 推荐：日常全能首选（文本+图片+视频全包）。 智谱 GLM-4.7-Flash。免费类型：永久免费 · 中文：⭐⭐⭐⭐⭐ · 推荐：写作、翻译、摘要（中文最强）。 DeepSeek。

免费类型：新用户100万token，后续极低价 · 中文：⭐⭐⭐⭐⭐ · 推荐：编程、逻辑分析。4️⃣ 火山 Doubao。免费类型：永久免费 · 中文：⭐⭐⭐⭐ · 推荐：轻量日常、稳定耐用。5️⃣ 商汤 SenseNova。免费类型：公测免费（每5h 1500次） · 中文：⭐⭐⭐⭐ · 推荐：图文理解、尝鲜备选。

## 我的推荐组合。
如果你不想5个全折腾，按这个优先级来：

- 日常主力：Agnes AI（无限免费，全模态，先把它用起来）
- 中文写作：智谱 GLM-4.7-Flash（中文最好的，还永久免费）
- 写代码：DeepSeek Reasoner（推理能力一绝，价格还低）
- 轻量备用：火山 Doubao（永久免费，稳定耐用）
- 尝鲜体验：商汤 SenseNova（公测免费，趁现在）
