---
title: "用豆包工作搭建求职看板，助你收获秋招Offer！"
source: "https://workbuddy.jiangyufan.com/index/hub/case/778"
type: "case"
chars: 2096
sections: 5
figures: 0
chapter: "12-我看别人怎么用"
---

# 用豆包工作搭建求职看板，助你收获秋招Offer！
![](https://mmbiz.qpic.cn/mmbiz_gif/kegUvHaA0d7wXO1yJ7zrcrokHf58p3fFR4lmy5o6RqJk3NWbzXk35TC1CJ0ePvRVppTZZDW4GFNibjROiasmwjb3XPIicIB5l9J6LDFNOefxyg/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

秋招期间，每天刷招聘网站，是不是总忘记投过哪些岗位、漏掉截止日期、搞混投递进度。

为了解决这个问题，博主@奥兰多话不多 用豆包工作做了一个「校招信息看板」：打开界面，就能一键查看所有校招新信息和投递进度。看板还能提醒你临近截止的岗位，列出今天需要准备的笔试和面试。

下面，我们就把搭建过程拆成具体步骤，附上可复制的提示词，带你从 0 到 1 做一个自己的校招看板。即使不懂代码，也能用豆包工作把它搭出来。

![](https://mmbiz.qpic.cn/mmbiz_png/kegUvHaA0d7LvsIXUiaRDx3uIvYwgdbKnYglLFnMcyJFCxAuZLSTfPru7RKyEicjmc7nnDRCSiaS1eGBuXOqgUTaQhESpdgZNadYeiag4iaiac1wc/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

## 第一步，先把使用场景和基础需求说清楚：
提示词。帮我做一个校招信息看板，用来管理求职进度。看板需要包含三个页面：今日看板：展示近期校招信息、今日待办、临近截止岗位和申请概览。

岗位跟踪：记录企业名称、岗位名称、岗位类型、城市、投递链接、投递状态、当前阶段、截止日期、下一步动作和备注；支持搜索、筛选、排序、编辑和删除。

添加岗位：支持手动填写岗位信息。添加后自动进入岗位跟踪，并根据截止日期判断是否临近截止。

投递状态至少包括待投递、已投递、笔试、面试、Offer、已拒和备选。数据需要保存在浏览器本地，刷新页面后不能丢失。

先做出一个可以直接打开试用的版本。如果部分功能暂时无法实现，请保留可用的替代方案，并告诉我如何测试。

![](https://mmbiz.qpic.cn/mmbiz_png/kegUvHaA0d6WiaOMFicqT0d9HJuMAForjjUuJnAiaHVAQopvJx2yDFMtsP2ZwbB1mvhFSmSDx07e0d4lZQAEEibKOvARdibtsuLD9O85vvbBYnGY/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

“今日看板”界面。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/kegUvHaA0d6IYDfzMBsbMkArm3wAHvPf08ZyRmgxfBPOKKOXWMrPdtZFL90EdT8dvgpqfPGcV6mEnrq8H0pnaz3Z4II15iaRGG1e6aY9ZfLc/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

“岗位跟踪”界面。

![秋招信息看板｜+ 添加岗位生成](https://mmbiz.qpic.cn/sz_mmbiz_png/kegUvHaA0d4wTmqEDCsYDvictsgAatGcqPuXsdfFlDT2aicNPh60T0l9ia2sficIHWUSYiaI8GgSVbrGxIgdz6HxMAc8pSNwicyEibdSo8bV7yOmug/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*秋招信息看板｜+ 添加岗位生成*

“添加岗位”界面。成后检查：

- 能否添加一个新岗位，并在岗位跟踪中找到它。
- 能否修改状态、截止日期和下一步动作。
- 搜索、筛选和排序是否生效。
- 刷新页面后，刚刚填写的数据是否还在。

Tip：第一步不需要写复杂 PRD，对第一次搭工具的人来说，先跑通流程，做出原型，比一次性塞满所有功能更重要。

![](https://mmbiz.qpic.cn/mmbiz_png/kegUvHaA0d7xSywNfO78W17EUlesPd8M01AoYvib22S1f2iaOHK60p5allWf3Ud6vjnpgk6ibFkz3PaZ2XblhxN1T2vib96BCIVRqbXRvZLeYzA/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

## 02边用边改，让看板更加顺手✦。
第一版出来后，按实际使用顺序测试一遍：添加岗位、修改状态、编辑待办、点击投递链接、刷新页面。发现问题后，直接进一步跟豆包工作说明需求，包括“在哪里、现在怎样、希望怎样”：请在当前版本上修改，不要改变我已经确认的整体布局：

1. 把“岗位 Tracking”改成“岗位跟踪”，界面名称尽量使用中文。
2. 岗位类型改成可自由输入，不要只提供固定选项。
3. 今日待办添加后可以继续编辑。
4. 已过截止日期的岗位整行变灰，并显示“已过期”标签。
5. 投递链接需要可以正常打开；如果只是预览环境限制，请说明正确的打开方式。

修改完成后，请逐项说明改了什么，并给我一个新的可试用版本。 Tips：

1. 一次只提一组同类修改。布局、字段、交互分开改，更容易定位问题。
2. 功能不稳定就先降级。@奥兰多Ruthburg 曾尝试自动解析招聘链接，但很多招聘网站无法稳定读取。比起卡住，她选择保留了手动录入，把时间用在进度管理上。

如果你也遇到类似功能迭代不理想的情况，可以直接告诉豆包工作：请移除当前不稳定的[你想改进的某功能]，保留[此前的形式]。不要影响其他已经可以使用的功能。

![](https://mmbiz.qpic.cn/mmbiz_png/kegUvHaA0d5wvXFHINoDHzlKObJSclibr6XjGT8Hia0Z7nKoy1x2JSJQJ85aa7ILnrOTolVAvuIrickCeTZxEdZmkNvLAHZraP2XprJVaWaoSM/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

## 03设定时任务，信息自动更新✦。
第一版里的“校招新信息”只是示例数据，为了让它每天自动更新，接下来，奥兰多单独创建了一个定时任务。请创建一个每天早上 8:30 执行的定时任务，更新校招看板里的“每日校招最新信息”，每次执行时：

1. 搜索最近 24 小时内新发布或有更新的校招信息。
2. 优先保留企业官方招聘页面或学校就业中心等可核验来源。
3. 每条信息写清企业、发布日期、城市、岗位方向、简要亮点和可点击链接。
4. 过滤重复信息；没有确认的信息不要写入。
5. 更新看板里的“最后更新时间”，并在任务结束后告诉我新增了哪些岗位。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/kegUvHaA0d4CUWgGDVlqCVTiayp3K8wUzsMlwRgVgFczqhVYuowOq6OQFXcVLg2HAwgq8Wm3OU1v9hkjcnxrFn06ofWdTf89s35vjn0kN0zM/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

- 定时任务是否已启用，下一次执行时间是否正确。
- 信息区的最后更新时间是否变化。
- 岗位链接能否打开，是否指向可核验来源。
- 连续执行时，是否会重复添加同一条信息。

Tip：“定时任务执行成功”和“固定网页已经更新”不是一回事。如果任务只生成一个新文件，你仍然需要每天下载和替换。要彻底自动化，还要完成下一步。

## 04固定网址，更新自动上线。
定时任务有了，但还差最后一步：能否让新信息自己出现在同一个网址里，彻底省去手动操作的环节呢。类似这样的问题，你都可以直接追问豆包工作。

请把校招看板发布成一个固定网址，并接上已有的每日更新任务。不要只把更新后的文件发给我：我要每天搜索、更新文件、提交仓库、发布网页都能自动衔接。

请先说明哪些步骤你能完成，哪些需要我登录或授权；不能自动完成的地方，请明确告诉我，不要当作已经实现。经过讨论，奥兰多在豆包工作给出的方案中选择了 GitHub Pages。除了技术方案，具体的操作与设置问题，也可以让豆包工作代劳。

![这是什么情况？｜让我看看这张截图。](https://mmbiz.qpic.cn/mmbiz_png/kegUvHaA0d6oIgGo4ahJBeURS3lQAHsds3tj51iaRibJ8j5Cau2BMoS53VsxicuXvsTjCJVkc4kcTjA7lqJ7Nib5H5qyhKt9fLPichhh4wjYycSE/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

*这是什么情况？｜让我看看这张截图。*

你甚至可以直接让它帮你获取 token，搭建 GitHub 仓库。

![生成步骤:](https://mmbiz.qpic.cn/sz_mmbiz_png/kegUvHaA0d7xLCppvSwZM31Fib06QA56VH2ofoX8iahic43AlYbBleqQSkuhvHR9icLoSFwUPAmhIO1JJq2BFnKCFbnGCt2QbUcic8UAUjZRncFQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*生成步骤:*

上线后检查看板能否正常使用，原先每天要手动完成的操作，就能自动跑起来了。

Tip：如果部署需要访问令牌，只授权必要的仓库和权限，并设置有效期。不要把令牌明文放进公开文档、截图或网页代码；优先使用平台提供的安全凭据配置方式。

还有一个容易忽略的点，这个校招看板把公共信息和个人记录分开保存。校招动态由网页统一更新，岗位跟踪和待办保存在每个人自己的浏览器中。因此，换电脑、换浏览器或清除网站数据后，个人记录可能不再保留。

![一欢迎关注一](https://mmbiz.qpic.cn/mmbiz_jpg/kegUvHaA0d5PDfmV3b1iawvAZcEKibibdFKhshicW9xWsdo66MTSAoFribsEHmD6boMoHRqO5PJOpumLUyYiabqug2rKtNUTWicMQagjcoUwT7kzlI/640?wx_fmt=jpeg&amp;from=appmsg#imgIndex=11)

*一欢迎关注一*
