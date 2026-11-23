---
title: "从一张Figma模板到能跑的电商App：把设计稿直接变成代码并推上Gitee"
source: "https://workbuddy.jiangyufan.com/index/hub/case/1083"
type: "case"
chars: 1294
sections: 6
figures: 1
chapter: "07-我要处理文档"
---

# 从一张Figma模板到能跑的电商App：把设计稿直接变成代码并推上Gitee
## 设计稿到代码之间，本来就隔着一道墙
做 App 最费时的往往不是写代码，而是把设计稿翻译成界面。Figma 里画好的页面，要变成能跑的代码，中间要手动还原布局、配色、交互，一遍遍对齐。

这次的做法是：找一套现成的 Figma mobile 模板，改一改，然后让 WorkBuddy 直接把设计稿落成可运行的页面。整个过程从模板到代码上线，一条流水线走完。

## 第一步：找模板、改名、改文案
在社区找到 Figma mobile 模板，里面已备好 Activities、Chat、Sign In、Checkout、Booking、Ecommerce、Social feed 等多套页面。先把它改名为自己的项目名，比如 feisu-mobile。

第二步修改模板：把第一屏 Ecommerce 的 title 改成中文名称，其余页面不用动。然后用左上角 File → save local copy 命令把模板保存到本地，会自动下载一个 .fig 文件。

![Figma mobile 模板的页面列表与电商首页预览](https://workbuddy.jiangyufan.com/uploads/attach/2026/11/20261122/eeaf941b5825dc037e8bc4c9f855312e.jpg)

*Figma mobile 模板的页面列表与电商首页预览*

## 第二步：把 .fig 文件交给 WorkBuddy
在 WorkBuddy 里用「日常办公—设计」的第 3 个指令，用鼠标把刚才下载的 .fig 文件拖进去。模型可以从默认的 auto 改成 GLM-5.1，让它自动读取 Figma 文件。

给它一句话任务：「把这个 Figma 组件落成一个可运行页面（React），要求用 mock 数据填充。」WorkBuddy 会先生成一份任务列表，再按顺序逐项执行——不是一次性吐出一堆代码，而是可跟踪的 8 个任务：商品详情页、路由整合、首页商品网格、社区信息流、聊天消息界面、个人中心设置页等。

## 第三步：看技术栈和成品
生成的页面用的是 Vite + React 19 + Tailwind CSS v4 + React Router 7，图表用 Recharts，图标用 Lucide React，还做了移动端适配（安全区域、viewport 适配）和无障碍访问（aria-label、tabindex）。

共生成 6 个完整页面：首页有搜索栏和 5 个分类标签切换，商品详情页含价格和图表，聊天页有客服/用户双样式和模拟自动回复，个人中心有用户卡片、订单、积分优惠券资产概览。数据全是 mock——8 个商品、5 条动态、6 条聊天记录、完整用户资料。

## 第四步：本地测试与上传仓库
代码生成后直接在本地测试：打开 localhost:5174 预览。注意默认端口 5173 如果被占用，工具会自动改用 5174，别以为没启动成功。

确认页面能跑之后，把代码推到 Gitee：cd 到项目目录，git init、git add .、git commit -m "first"，再 git remote add origin 指向自己的仓库，git push -u origin master。到这里，一套从 Figma 模板到线上仓库的电商 App 原型就完成了。

## 这件事的关键：先有一个能跑的东西
这套流程的价值不在于一次生成就能上线，而在于把「设计稿 → 可运行页面」这一步从半天压缩到几分钟。你能很快看到一个能点、能翻、能预览的成品，再决定要不要继续打磨。

跑起来，比一开始就追求完美更重要。
