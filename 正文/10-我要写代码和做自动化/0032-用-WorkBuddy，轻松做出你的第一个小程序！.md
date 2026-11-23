---
title: "用 WorkBuddy，轻松做出你的第一个小程序！"
source: "https://workbuddy.jiangyufan.com/index/hub/case/465"
type: "case"
chars: 2437
sections: 6
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 用 WorkBuddy，轻松做出你的第一个小程序！
![](https://mmbiz.qpic.cn/mmbiz_gif/u0lmmJTuFHgZaOfHW6VwNe0UDbXdibVVJ40XrYFe81kUQ8vghddibjRg9cVHQWjMmibQqpict4WjPI284e6cL9ibgwzQuaI8y488dV5uO0G4Zdc8/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

想做一个自己的小程序，却不会写代码。

无论是待办清单、日常记账，还是社团管理工具，现在都可以借助 WorkBuddy，从需求描述到开发上线，一步步把想法变成现实。

在10月22日的直播中，WorkBuddy 技术专家 Jiawei、腾讯设计 Ardot 产品体验官 Hongcen，带大家实操演示了如何用 WorkBuddy 搭建微信小程序，并结合 Ardot 完成 UI 设计与优化。

这篇文章就带大家一起从常见场景出发，从 0 到 1 搭建出自己的小程序。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHgGzaeJxkbnGP73ZEfBLLnTAhPHemAhqSYsat89SXhX7yJtd3qSYms3oOia4aOc3eicMg0r60RibrYukn30ZwUNCCTLjODDfWkNvg/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

## 01 基础版：用 WorkBuddy，快速搭建一个小程序。
如果你还没有接触过小程序开发，可以先从基础版开始。以「今日待办」小程序为例，只需要通过自然语言描述需求，就可以让 WorkBuddy 帮你完成开发。

## 第一步：说清楚需求，让 WorkBuddy 开始开发。
打开 WorkBuddy，如果有「开发」模式，可以直接进入开发模式进行对话；

![办公 开发 设计｜选择工作空间](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHgjNhqmdB4ibZRRiauTgKiavsBAe75lBLq5C8xn8uNNSh0oyBeMMRGUgAk6iatGlwNsiaWloVxyYF14uYyF2RNLBsYGZP8TJiagOviaAc/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*办公 开发 设计｜选择工作空间*

如果没有「开发」模式，也可以直接在对话框中明确提出「帮我开发一个微信小程序」，WorkBuddy 会根据意图触发任务。

![PM线稿原型｜企业智能办公专家团](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHhwkDLwmqh9QOnTWJLNUpy7ibM0Br9QqrwQZOXJTNlv4Pf9S4jb4jV9hNDwCShmzuwDlpe8fCUd5zYdvp0BOOtolozOCS99qokU/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*PM线稿原型｜企业智能办公专家团*

不同版本的 WorkBuddy 可能存在界面和入口差异，但不影响小程序开发功能的正常使用，按照上述任一方式操作即可。

开始前，建议从四个方面描述需求：

- 用途：这是什么类型的应用？主要解决什么问题？
- 使用对象：是自己使用、团队共用，还是提供给客户？
- 功能：需要哪些页面？每个页面分别实现什么功能？
- 视觉风格：希望采用什么配色、布局和设计风格？

例如，想搭建一个待办清单，可以这样描述：

要做一个微信小程序。做一个自己用的待办清单小程序，叫「今日待办」。首页是列表，能新增、勾选完成、删除；关掉再打开数据还在，数据上传到云服务；主色蓝色，适配手机。

先把核心功能说清楚即可。后续需要增加筛选、调整界面，都可以继续对话修改。

## 第二步：分步骤完善需求，生成小程序预览。
需求不必一次写得很长，建议先生成可用版本，再按「功能—存储—优化—检查」逐步迭代。下面这组指令可按开发进度分次发送：01 功能开发。02 云端存储。把待办数据改成存在云数据库里，换手机登录同一个账号也能看到自己的清单。03 功能优化。顶部加筛选：全部 / 未完成 / 已完成。列表项支持左滑删除，删除后能撤销。

04 自查检查。

帮我检查一遍：所有页面是否都已在配置里登记；有没有用到小程序不支持的写法；有没有写死的文字该改成配置；有没有需要用户授权的信息。

WorkBuddy 会根据要求生成代码，处理相应的工程配置与构建检查。完成后，打开产物卡片即可预览。预览时先看页面是否符合需求，再逐项测试新增、删除、筛选和跳转等交互。

![开发今日待办小程序｜失败，已暂存本机，下次打开或下拉刚刚新时自动补传，不静默失败。](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHgJsNicMuIQSGySAxL4LTMUmUFAdzgC7ec3PHX9lic0wHGkzoMqEu3p0f9vgRWiaJiaU703HF2Q75SYva9wia4YTFZM5YVaSGPlvm58/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*开发今日待办小程序｜失败，已暂存本机，下次打开或下拉刚刚新时自动补传，不静默失败。*

如果效果不理想，不必重新开始，可以针对问题继续修改，例如：

- 首页增加已完成任务的统计区域；
- 将列表行距调大一些；
- 增加任务分类和筛选功能；
- 修改按钮样式和页面布局。

遇到难以描述的视觉问题，直接附上截图或参考图，比笼统地说「更好看一点」更有效。

![开发今日待办微信小程序｜Clickboard_Screenshot.png 参考这个页面优化画面配色及排版](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHgcy5xn7TMrL65GCDTNrl1BB5QuZeBzsRwWLxq75PhXsbTG0WlJRdGAYOmSOoWQxNWocDUK2AVos2nqRd1CAFYsqn1AqRZlknE/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*开发今日待办微信小程序｜Clickboard_Screenshot.png 参考这个页面优化画面配色及排版*

小技巧：一次集中修改一个问题，说清楚「当前效果」和「期望效果」，方便检查修改结果。

## 第三步：接入云服务，让数据真正保存下来。
待办、记账、打卡等应用，需要在关闭页面后保留记录。只生成界面还不够，还需要数据存储。如果将记录存入云端，同一账号就能在不同设备读取数据；图片上传、用户登录等功能，也可以根据需要接入。

传统做法需要自行配置服务器和数据库。使用 WorkBuddy，可以在开发过程中开通配套云服务，并让应用调用相应能力。

![](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHh6jMqhqC8hFaCn5XyrbItPuw50udfr6ibPlqHgOQJiaLRic10Ywmd9TDTffhicTk95w0lNQsARIbkmGYnBVAvtZn12UicPU3QFELnA/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

![](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHiaHxPul6ibrm9eYFP6xraTfJfKKmpibJdoadovSeiapdFAib5QwAc7qgHhgwI62S6K8dibVewwdyFwic4VQYqQMnU7BoKAOWlOk7yBJU/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

入口一：预览页面左上角云服务。

![](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHgbg9icFAOHWoMfM7EBDiacnqQ0tY7njGriaic59ekXSeiajrSDFz8vRZq5Vq67UQgbWLMDtwkhaMxEoVoU1D0qPWzug2vA7HjtwYlY/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

入口二：设置-数据管理-应用。例如，「今日待办」可用云数据库保存任务，按需要配置登录，并通过数据管理页面查看应用的使用情况。注意：

使用 WorkBuddy 云服务时，需要关注「可开启云服务的应用数」和「单应用云服务资源点」两项额度。

不同会员版本对应不同的使用额度。其中，应用数决定最多有多少个应用可以开启云服务；资源点则用于计算单个应用使用数据库、文件存储、服务调用等云服务能力产生的消耗。

资源点按应用独立计算、按月刷新，用尽后对应应用的云服务将暂停。用户可在「云服务用量」页面查看使用情况，也可通过升级会员获取更多额度。

![套餐与积分｜记忆与进化](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHgfHXf5e4ojQvn1YIg04Ia9rEcBlUxibu7CryuVqJx1bJQeiaLLJDPrnWQFjmqibDAW3gAIicVhMbavLOOxt252tl8hib7ATvOgvcfQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

*套餐与积分｜记忆与进化*

详细说明可点击「资源点消耗规则」查看。

![试用小程序，请在2026/11/04前发布使用｜试用版已发布](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHgU0I3fzZb5GjvLVcx72kDLzxUAGlrpcOBRU0GMIB2UNe1P8HtnT8M78cGcjPwvWZrC5S9g5bqmGjXiaWTDdwm2v1IBtPLJeViaU/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*试用小程序，请在2026/11/04前发布使用｜试用版已发布*

![试用小程序，请在2026/11/04前发布使用｜试用版已发布](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHjU3icSj3giar2bFMFCWFvc4AcKjTqnKXZykWgPs16jTwYOaKERWVsv6oc1XibSyZLcz0lHia5gxwcBk0ic7LUrBdzicFERuFcjfGxpM/640?wx_fmt=png&amp;from=appmsg#imgIndex=11)

*试用小程序，请在2026/11/04前发布使用｜试用版已发布*

![试用小程序，请在2026/11/04前发布使用｜试用版已发布](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHiaZkZqSLSgK7aY7O3lTxHibMozNR9iay5ZXpNctcBedibhYrQgDB3GQEs07bKUNDRwXxsS3CDl4j0mDd4TsSt36aGzYtjOhnicKOvk/640?wx_fmt=png&amp;from=appmsg#imgIndex=12)

*试用小程序，请在2026/11/04前发布使用｜试用版已发布*

![试用小程序，请在2026/11/04前发布使用｜试用版已发布](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHhEhfKvpnT6K36mREeJ84EZOicuKseudNvGsmhNkEGgKQxAzU34oyfKwBeFkZZ5QZvMtQHKhDOama5e8wtuwpkoocRgV21PCRnY/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

*试用小程序，请在2026/11/04前发布使用｜试用版已发布*

![](https://mmbiz.qpic.cn/mmbiz_png/u0lmmJTuFHia9VxDpyyniaoXa7iaVzN1ibLljiaQMqKWpNskZxibzEaLT1t8S6UYj7tU3nyPsliaXKtSQ4wFkjpFicnpgUZBeAWLwo9Bic72yBkMD8D0/640?wx_fmt=png&amp;from=appmsg#imgIndex=14)

试用版、体验版与正式版区别。

注意：试用小程序有 14 天有效期，主要用于快速验证功能，不能直接发布成正式版。如果发现问题，回到 WorkBuddy 修改，再重新发布或更新对应版本。

至此，基础版小程序的搭建就完成了，若对界面有更高要求，可以继续进入进阶设计流程。

## 02 进阶版：结合腾讯设计 Ardot，让小程序更好看。
能用之后，下一步是让页面更清晰、风格更统一。这里可以借助腾讯设计 Ardot，把视觉方案变成可交付的 UI 稿。

以「咖啡账本」为例，我们可以通过 WorkBuddy 与 Ardot 的配合，打造一本专属于咖啡爱好者的记录手账。

## 第一步：确定产品方案，生成设计概念图。
在正式设计之前，先明确小程序的定位、核心功能和页面结构。例如，咖啡账本可以围绕四个核心页面展开：

![](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHj3PUibtibqUlrj6D56kU93EK1wiaNkqbCWeOODv67PmjZyqSy7TlrlU8libhPVFRM1UN9ePp9ZPibcTyq3Oo0s4icibA8Rw265oEof6U/640?wx_fmt=png&amp;from=appmsg#imgIndex=15)

确定页面结构后，就可以进一步探索配色、字体和视觉风格，为小程序确定整体设计方向。打开 WorkBuddy，如果有「设计」模式，可以直接进入设计模式进行对话；

![](https://mmbiz.qpic.cn/sz_mmbiz_png/u0lmmJTuFHjm2AtcjSrBjcURdn6ibc4XGl99NQ10mVNLia0WXjuJP9WYTNYDsJ3JIibe5vtJ42UGd9nCsXGyDscPxvib2WAV5SykYgppewVVnc8/640?wx_fmt=png&amp;from=appmsg#imgIndex=16)

如果没有「设计」模式，也可以通过「UI/UX」入口进入设计模式。进入后，可以通过对话描述设计需求，调用 Ardot 画布生成小程序的初步设计稿；
