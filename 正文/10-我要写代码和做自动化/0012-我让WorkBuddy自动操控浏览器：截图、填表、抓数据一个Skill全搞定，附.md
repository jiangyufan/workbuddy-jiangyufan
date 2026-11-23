---
title: "我让WorkBuddy自动操控浏览器：截图、填表、抓数据一个Skill全搞定，附"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/394"
type: "skill"
chars: 3217
sections: 7
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 我让WorkBuddy自动操控浏览器：截图、填表、抓数据一个Skill全搞定，附
今年 WAIC 最大的关键词，不是模型参数，不是多模态——是「Agent 连接真实世界」。

支付宝发布 AHA 协议，让不同 Agent 在用户授权下互相调用服务。阶跃的手机 Agent 能自动打开飞书写 PPT、调高德地图导航。千问眼镜现场演示"看菜单 → 下单 → 结账"全流程。百度搭子直接内置了 Browser Use 能力。

所有大厂都在讲同一件事：AI 不能只停在对话框里，它得学会动手操作。而最通用的"动手"方式，就是操控浏览器。

不需要等大厂生态落地。现在，你电脑上的 WorkBuddy 装一个 browser-use Skill，就能让 AI 替你操作浏览器——截图、填表、抓数据，一句话搞定。

装完这个 Skill 之后，WorkBuddy 不再只是"能聊天的 AI"，而是能打开网页、点击按钮、截图保存、抓取数据的数字员工。

![浏览器操作Skill三大核心能力｜文本/下拉/文件上传](https://mmbiz.qpic.cn/mmbiz_png/6pFYpvgNaSXkKQBfwPFxIyOWKGTgFN12vnbWmjC6Uet1gb5WIbnMDGaicR7n8oaZoG6koeRqJ8KrBPFwnpIo2eJ7zyRItDJ9ibsFeP9XqicIv0/640?from=appmsg&amp;watermark=1#imgIndex=0)

*浏览器操作Skill三大核心能力｜文本/下拉/文件上传*

▲ 浏览器操作 Skill：截图、填表、抓数据三大核心能力。

## 这个 Skill 到底能做什么。
browser-use 是一个命令行浏览器自动化工具，专为 AI Agent 设计。它跟传统的 Selenium、Playwright 不同——不是让你写脚本，而是让 AI 直接用自然语言操控浏览器。

核心能力就三类：

- 截图 — 打开任意网页，全页截图或指定元素截图，自动保存 PNG。
- 填表 — 定位输入框、下拉框、文件上传控件，自动填写内容并提交。
- 抓数据 — 读取页面标题、元素文本、HTML 源码、甚至执行 JavaScript 提取结构化数据。

你只需要用自然语言说"帮我截一下微博热搜""帮我填这个表单""帮我抓一下这个页面的数据"，剩下的它全自动完成。

## 怎么装。1 分钟上手。
browser-use 已在 WorkBuddy 技能市场上架，安装方式跟其他 Skill 完全一样：

- 打开 WorkBuddy，点击左侧「技能」菜单
- 在搜索框输入"browser-use"或"浏览器"
- 找到 browser-use 卡片，点「安装」

装完之后零配置，直接在对话框里下指令就行了。WorkBuddy 会自动识别你的意图，唤醒 browser-use 去执行。

底层跑的是 Chromium 无头浏览器，命令之间浏览器保持打开状态（daemon 常驻），每次操作延迟约 50 毫秒。快到你感觉不到它在"用浏览器"。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/6pFYpvgNaSVOAbTibFDQWicf0vF715T0Dxv94eSu8Pnfhnpu5SDbfzicOLZ1qQmYmdMIWYeDbyygb4AaQHicNse5CqhOT8ICNQgey291NS55PRU/640?from=appmsg&amp;watermark=1#imgIndex=1)

▲ browser-use 命令能力一览：导航、交互、截图、数据提取四大类 30+ 命令。

## 实战一：一句话截图微博热搜，不用打开浏览器。
以前你要截微博热搜，得手动打开浏览器 → 输入网址 → 等加载 → 滚动页面 → 用截图工具框选。现在只需要在 WorkBuddy 对话框中发一句话：

帮我打开微博热搜页面，截个全页截图保存。"。WorkBuddy 接到指令后会自动执行以下步骤：

- `browser-use open https://weibo.com` → 启动无头浏览器打开微博
- `browser-use state` → 获取页面元素列表，定位热搜区域
- `browser-use screenshot --full weibo-hot.png` → 截全页保存

整个过程 5-10 秒，截图自动保存到你指定的路径。你没打开任何浏览器窗口，没碰鼠标键盘——AI 全自动完成。

如果你装了 Chrome 并且想复用登录状态（比如要截需要登录的内部系统页面），加一行 browser-use connect 就能连到你现有的 Chrome，保留所有 cookies 和登录态。

## 实战二：自动填表提交，表单多的场景直接解放双手。
工作中遇到最多的重复操作就是填表——日报、问卷、报销单、信息录入。browser-use 的填表流程非常简洁：

- `browser-use open ` → 打开目标页面
- `browser-use state` → 获取所有可交互元素的编号
- `browser-use input 3 "白同学"` → 在第 3 号输入框填入"白同学"
- `browser-use input 5 "13800138000"` → 在第 5 号输入框填入手机号
- `browser-use select 7 "技术部"` → 在第 7 号下拉框选"技术部"
- `browser-use click 9` → 点击第 9 号元素（提交按钮）

如果你需要上传文件，也支持：browser-use upload 12 /path/to/file.pdf 直接把本地文件塞进表单的文件上传控件。

## 实战三：抓数据导出，竞品分析、舆情监控的利器。
数据抓取是 browser-use 最硬核的能力。它可以用 JavaScript 直接在页面里运行代码，提取任何想要的字段：

- `browser-use get title` → 获取页面标题
- `browser-use get text 23` → 获取第 23 号元素的文本内容
- `browser-use eval "document.querySelectorAll('.hot-item').map(el→el.innerText)"` → 用 JS 批量提取热搜列表
- `browser-use get html --selector "table.data-table"` → 只提取数据表格的 HTML 片段

更骚的操作：抓完数据之后，WorkBuddy 可以继续调用 Excel Skill 把数据写进表格，或者用 PPT Skill 生成趋势报告。一条指令串联两个 Skill，全自动。

![浏览器操作核心流程｜五步法:拿到元素编号→交互→验证→循环](https://mmbiz.qpic.cn/mmbiz_png/6pFYpvgNaSUzibkrF1iaGicgrdtxPtADFwX5s8KczYtOSNx2hsyugNcJ118vEE4cxrrDsMpTYt1yCAPlxSBhVqYaMQFQ7ibBPYFEEd2YTWNLaJ8/640?from=appmsg&amp;watermark=1#imgIndex=2)

*浏览器操作核心流程｜五步法:拿到元素编号→交互→验证→循环*

▲ browser-use 核心操作流程：五步法搞定任何网页任务。

## 跟 Selenium / Playwright 有什么本质不同。
很多人听到"浏览器自动化"第一反应是 Selenium 或 Playwright——但要写代码、要懂 DOM、要处理等待逻辑。browser-use 的设计哲学完全不同：

❌ Selenium / Playwright 给人写的脚本工具 要写 Python/JS 代码 自己处理 DOM 解析 需要管理 WebDriver 定位元素靠 CSS/XPath ✅ browser-use 给 AI Agent 设计的 用自然语言下指令 AI 自动解析页面 CLI 一行命令搞定 定位元素靠数字编号。

最直观的差距：用 Selenium 抓一个页面数据，你要写 30-50 行 Python。用 browser-use，你只需要在 WorkBuddy 里说一句话。

browser-use 还有一个杀手级特性：多会话隔离。用 --session 参数可以同时跑多个浏览器实例，互不干扰。一个 session 在填报销单，另一个在抓竞品价格，完全不串数据。

![浏览器自动化:两种路线的对决｜给人写脚本用的](https://mmbiz.qpic.cn/sz_mmbiz_png/6pFYpvgNaSXGEl7ILCZxJuAHHAv5rA7SzkKwKuNfgAlCZDNUh3E3O3P4HMGr6sL2TIn1Gz0Eiayiaxb4I9FCgtmE19FStPoPmez4gibnVSKWq4/640?from=appmsg&amp;watermark=1#imgIndex=3)

*浏览器自动化:两种路线的对决｜给人写脚本用的*

▲ browser-use vs 传统自动化工具：设计哲学、使用方式、适用场景三维对比。

## 三步让你今天就能上手。
这个 Skill 的上手成本极低——不需要装 Python 环境，不需要配 WebDriver，不需要写一行代码。

- 第一步：安装 Skill

WorkBuddy 技能市场搜索"browser-use"，一键安装。2 秒装。

- 第二步：试第一条指令

在对话框输入："帮我打开百度首页，然后截个图"。浏览器会自动打开、加载页面、截图保存。你全程不用动手。

- 第三步：进阶——串联其他 Skill

做完浏览器截图或数据抓取后，紧接着说"帮我把截图里的数据整理成 Excel 表格"——WorkBuddy 会自动调用 Excel Skill 接力处理。一条对话链，完成截图→提取→整理→输出。

如果你需要操作需要登录的网站（企业内部系统、邮箱、后台管理），用 browser-use connect 连到你现有的 Chrome，所有登录态自动复用。

![三步上手，今天就能跑起来｜从零到AI替你操作浏览器](https://mmbiz.qpic.cn/sz_mmbiz_png/6pFYpvgNaSU4CWLsICBQZN4uibwoddjtukwwZJG5vLBm51ohbL4uEGnSjrrV4yibhPuQmya6TlzWibicfx5MX71wSWnh2ZInXVnTq6eqdXtPQTE/640?from=appmsg&amp;watermark=1#imgIndex=4)

*三步上手，今天就能跑起来｜从零到AI替你操作浏览器*

▲ 三步上手：安装 → 第一条指令 → 串联其他 Skill。总结。

WAIC 2026 定调了：AI Agent 的下一步不是"更会聊天"，而是"能动手"。浏览器自动化，是 Agent 连接真实互联网最直白、最通用的入口。

WorkBuddy 的 browser-use Skill 把这个能力做到了一句话级别——你不用写代码、不用配环境、不用懂 DOM。只要会说话，就能让 AI 替你操作浏览器。

截图、填表、抓数据。三步上手，今天就试试。
