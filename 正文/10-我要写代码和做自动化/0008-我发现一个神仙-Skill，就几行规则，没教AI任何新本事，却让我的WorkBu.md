---
title: "我发现一个神仙 Skill，就几行规则，没教AI任何新本事，却让我的WorkBu"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/370"
type: "skill"
chars: 3423
sections: 5
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 我发现一个神仙 Skill，就几行规则，没教AI任何新本事，却让我的WorkBu
哈喽大家好，我是阿胖~。朋友们，我最近又又又发现一个神仙 Skill。事情是这样的，最近我一直在琢磨能不能搞一个 AI 自动剪视频的工作流。

![Canary u004和Canary u005开始工作｜已使用浏览器运行了命令](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLrZ8AkOQyQruB0L2uY9W7iaK7jfAlWyJs1WuIfDyquUkUxunxBtXjud859mNgFurr6ZqokpOzypPUk2y1vjQx3mNHFYKibEJIEHo/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*Canary u004和Canary u005开始工作｜已使用浏览器运行了命令*

我扔进去一段 20 分钟口播，它自己找高光、删废话、加字幕、插 B-roll，最后给我吐出来 3 条短视频。

想法听着挺爽，但真开始琢磨，我很快就晕了。转写、高光提取、删废话、字幕、B-roll、配乐、渲染……这几个东西到底谁先谁后。我就把问题扔给 WorkBuddy，然后它开始给我上课了，给我整了一堆专业内容……每个字我都看得懂，组合在一起我就看不懂了，所以到底咋跑的。

![今天帮你做些什么？@引用对话文件，/调用技能与指令｜+ ①允许完全访问√](https://mmbiz.qpic.cn/sz_mmbiz_png/XXRDicaNweLpkK2Terhn00SnbYicKibK7dgzgiamTWgialiczM1Ky1km6lkGfwc9y3hicOekMkQSZ19ScI1Vo6HlEM81B3Cdfz3WsGDRCWx1FiaFbhY/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*今天帮你做些什么？@引用对话文件，/调用技能与指令｜+ ①允许完全访问√*

现在的AI越来越牛逼了，这背后也可能会出现一个问题，他想的很多，给的也很多。我只是想知道这玩意从哪儿进、经过哪儿、最后去哪儿。它恨不得给我写一份技术白皮书，哈哈。

最近我刷内容的时候就刚好刷到了一个叫 show-me 的 Skill，我一看，诶，这个skill有点东西啊，好像专门就是来解决“AI 明明讲了一大堆，但我看完还是没搞懂它到底在说什么”这个问题的。

我就把它装到了我的workbuddy里，调用show-me后问了workbuddy同样的一个问题。他没教我的AI任何新本事，但workbuddy却像换了个脑子似的。

## 看看workbuddy画的一部分图。

![](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLpF2StGmCy0R9rG7Dsytc5kDsW93NXKb7p2g1eF84KYWayldIMoz88OAibvlQYBfFlfucWuKWoyYia0iaIPz1x1KhsWoruLn88Y3I/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

不是哥们。早这么跟我说话不就完了吗。这多通俗易懂啊，还整前面那出。

这玩意是 HumanLayer 开源的，我看了一眼它的 SKILL.md，文件本身并不大，就几行规则。

干的事情也非常简单，就是：别一上来给用户写小作文，能画出来，就尽量画出来。

![](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLpwPfSt8DtfoIh4lKQcSPRg0Doia6Z6vH0URpp1Im8rG3CDXLibrZaTTtK8wZlmuPXgl1nxH2e8nTBQoOIpfYlVwttIlomdjgOy8/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

就这么个东西。我第一眼甚至有点不理解，这也算 Skill。因为你仔细想想，workbuddy 本来不会画 Mermaid 吗。会。不会写 HTML 吗。也会。这 Skill 压根没教 AI 什么新能力，但特别骚的地方就在这里。它没让 AI 变聪明，但是它却让 AI 换了一种跟你说话的方式。

我们理解很多复杂东西，本来就是靠结构的。你去看地铁线路图。没人会写一篇八千字文章告诉你，从人民广场到虹桥火车站，列车如何依次经过每一个站点。画条线就完了。你去看公司的组织架构，也不会给你发五千字告诉你，张三隶属于谁，李四汇报给谁。一张组织架构图就搞定了。

但不知道为什么，到了 AI 这里，我们突然开始容忍它一天给我们写几十篇小作文。所以HumanLayer 自己发布 show-me时，吐槽的其实也是这件事。

他们觉得现在的 coding agent 在纸面上越来越聪明，但在「能不能让人快速读懂」这件事上，体验反而变差了。

于是他们干了这件事，不继续想办法让模型多说一点，而是让模型少说一点，用视觉结构说。

![让 AI 少说，用视觉结构说｜不是更聪明，而是更好读懂](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLpicp0M75ByRjrvGrXf2mnmYh3HOjEcJ8ygm490FeTurL1Wm78rViaWJGOmyjbXJ6Du5o7aVMUqyC0MyofUpbiauImXHHqSZPuFu8/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*让 AI 少说，用视觉结构说｜不是更聪明，而是更好读懂*

这么一看，他们的设计理论和逻辑确实非常牛逼，但一次有效并不代表什么，于是我又做了几次实测，结果又发现了一些隐藏惊喜。

刚好我又想到一个让我纠结的问题。刚才这个 AI 剪视频工作流真要做起来，其实有两条路。一种是先让 AI 把整个 20 分钟视频看懂，挑完高光、删完废话，再统一开始剪。另一种是先把视频切成很多段，每一段分别处理，最后再拼起来。听起来都挺合理。但字幕怎么办。B-roll 怎么办。哪个方案上下文更完整。

于是我要求它不调用skill，又去问了这个相关问题，你看他的回复，熟悉的一幕......。

![尽量详细一点，把你考虑到的问题都讲清楚。不调用其他skill](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLpD8LJF12WvSAPE1FcsuzMDIyNWwicnK2jHqTdvJ8a6gwvvYm0oILQ41NeHbldKaavoCW0gTpl4JUTSSoKWSACfhSDSV1N1LnJU/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*尽量详细一点，把你考虑到的问题都讲清楚。不调用其他skill*

它非常认真地给我分析了半天，方案 A 有啥优点，方案 B 有啥问题，上下文怎么保留等等。

![二、各自的优缺点｜今天帮你做些什么？@引用对话文件，/调用技能与指令](https://mmbiz.qpic.cn/sz_mmbiz_png/XXRDicaNweLoZM7YC0iceeFlnRVoySXKWP4tvGl2MZKLDftoCZkehvV7aibsw2TANicl4S9zKz4FEmIeLls3Oym3bsmSLAxc9AvN4Uu52cyz6HI/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*二、各自的优缺点｜今天帮你做些什么？@引用对话文件，/调用技能与指令*

写得确实挺专业。然后我发现我看完，又得在自己脑子里画一遍图，那我还看个啥哈哈哈哈。

## 所以我直接调用/show-me。

![①两条流程各自怎么跑｜红色角标 = 该环节最容易出问题的地方](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLrlDQvhccqibIjiaWPk7H9NiaeU36PBWS2otW13mvoOaytIGdjRyhqIXy8NchVSnufb0L3asRWaRDkBYCTqYwCT3ib3dlpOdJ5qe90/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*①两条流程各自怎么跑｜红色角标 = 该环节最容易出问题的地方*

看看，这感觉，一下就舒服太多了。这轮测试让我又发现了一个隐藏优点，show-me 不只是把“流程”画出来。它连复杂方案之间的取舍，都能帮你把脑子里的结构搭出来。有时候 AI 给你列 10 条优缺点，其实信息一个没少，但咱真正缺的是：所以这两个东西到底差在哪。

到这里我本来已经觉得挺牛逼了。但我翻 show-me 的规则时，又发现了一个比较骚的东西。如果普通的图还讲不清楚，它甚至可以直接给你做 HTML。我看到这儿第一反应是。等等。HTML。意思是一张图不够，你还能直接给我做个网页讲。那我肯定得试啊哈哈哈。

我干脆把前面整个 AI 自动剪视频的工作流全扔给了 WorkBuddy。还是刚才那个需求，然后它真的开始给我做网页了。

![把我们前面讨论的「AI 自动剪口播视频」整个系统，做成一个完整的 HTML 可视化讲解页面。｜用户上传一段 20 分钟左右的口播视频，](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLpbWAHU427vH9T3FEkcXKWlW6xUDkOZ7wiasElnyiclAibmg7spKDbao1cQ3dyAicMP9tlb06cU3JHvJShiaoNN19JzegqUc8sBwWIA/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*把我们前面讨论的「AI 自动剪口播视频」整个系统，做成一个完整的 HTML 可视化讲解页面。｜用户上传一段 20 分钟左右的口播视频，*

不是哥们。我只是让你把这事儿给我讲明白。你怎么给我整了个课件出来。哈哈哈哈哈。

![页面已打开，共四个区块，30秒能看完主线：｜今天帮你做些什么? @引用对话文件，/调用技能与指令](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLpKa8OxalNMM2yDicqyNuZEmhWQ39gakgm6p28s91zYiaVxTESR3UeXNPdicewamdrjf2ZatESbQHyUJPkjlib7s5Z7mlrp5YN9sNI/640?wx_fmt=png&amp;from=appmsg#imgIndex=9)

*页面已打开，共四个区块，30秒能看完主线：｜今天帮你做些什么? @引用对话文件，/调用技能与指令*

而且我一开始还以为，它最多就是把刚才那张流程图放大一点。结果我往下滑了两下。发现不对，这玩意是真的在给我讲。最上面它先把整个系统压成了特别简单的一条线。

然后再往下，它直接给整个过程拆成了五步，听、懂、剪、配、出，先转写，再让大模型通读全文、挑高光。接着根据保留下来的内容重建新的 60 秒时间轴，最后字幕、B-roll、配乐全部挂到这个新时间轴上，再统一渲染。

![AI 自动剪口播视频｜一段完整口播 → 全自动理解、剪辑、包装 → 三条可直接发布的短视频](https://mmbiz.qpic.cn/sz_mmbiz_png/XXRDicaNweLqeObwiaW4nWyibXFD6kXuHticJyzv4Kzuyh3AzkjHKsRrFjTvicAGT1qhoJau1kgacrYfZRBLfVfAvWbyyWsu6f1p1ZhKvj1icib3Ns/640?wx_fmt=png&amp;from=appmsg#imgIndex=10)

*AI 自动剪口播视频｜一段完整口播 → 全自动理解、剪辑、包装 → 三条可直接发布的短视频*

我看到这里其实已经懂得七七八八了。但真正让我觉得这玩意有点东西的，是它后面居然把我最开始没搞明白的那个问题，专门拎出来画了一遍。

## 字幕时间戳到底咋办。

![输入 用户上传 20min MP4｜输出 视频文件（暂不处理画面）](https://mmbiz.qpic.cn/sz_mmbiz_png/XXRDicaNweLpzyeCyYdibY9YQ9VJcOYzbTCApRk4L4660s0Gg2O3kelzGMC2fCZGzNPfzFd8u07aAKsHLMDkfM5iaBoboSMDg9XMCu3fDic2dE4/640?wx_fmt=png&amp;from=appmsg#imgIndex=11)

*输入 用户上传 20min MP4｜输出 视频文件（暂不处理画面）*

## 你还记得文章最前面我为什么会被这套 AI 剪视频流程整懵吗。
就是因为我一直没想明白，假设原视频里一句话出现在 9 分 12 秒。

但是前面的废话被 AI 剪掉了 5 分多钟，那最后成片可能才 60 秒啊，你总不能还让字幕在第 9 分 12 秒出现吧，它就在网页里直接给我画出来了。

![](https://mmbiz.qpic.cn/mmbiz_png/XXRDicaNweLqJ8ctxZWBhcuMjibrjqQiaEZAticWhYMXXF3aNsK0O979iaHPuBF97P5XDyWoA2b0x4oAhLysGS8GhZQn1FWqgXDrM9Ayqy1VpRJ4/640?wx_fmt=png&amp;from=appmsg#imgIndex=12)

现在 WorkBuddy 这些 Agent 越来越能干以后，新的烦恼反而变成了，它知道得太多，但是我们的脑子也没有因为 ai 又升级了，就突然多长出八个前额叶。

一个管「别急着干」。一个管「别急着写」。

当然哈，任何skill也都不要无脑瞎装，这个skill这从它的设计加我的一些实测来看，我认为它比较适合的基本都是那种「信息一多，光靠文字脑子里很难搭出结构」的任务。

![这种 Skill, 适合什么时候用?｜信息一多，光靠文字就难搭结构](https://mmbiz.qpic.cn/sz_mmbiz_png/XXRDicaNweLqnQ085E3KsxONUbnoiba9gQdByKhBwAB9wkmzn3oG1I2u7Zwib8ZibQJPNySVybiahibibMjT4OlE5YvpFlmhRS3ytLsyc4eDZbVOHc/640?wx_fmt=png&amp;from=appmsg#imgIndex=13)

*这种 Skill, 适合什么时候用?｜信息一多，光靠文字就难搭结构*

比如接手一个陌生项目，接触一个陌生复杂的领域，又或者是AI 刚给你改完一大堆东西，你想知道它到底动了哪的时候。

或者最简单的，你的ai给你甩三屏文字，你盯着看了十秒，发现一个字都不想读，这时不用重新想半天 Prompt，直接调用show-me 就挺好。

但是哈，改个标题、写个小函数、问个命令这种事，真没必要啥都画一遍。那就有点。像是为了吃碗泡面，先画一张泡面系统架构图了，哈哈。简单来说，就是 Agent 干的活越复杂，这个skill的作用体现越明显。安装也挺简单。HumanLayer 官方仓库目前给的命令就是下面这行。

```
npx skills add humanlayer/skills --skill show-me。装好之后可以直接调用/show-me。也可以直接跟 Agent 说，让它使用show-meSkill。如果内容特别复杂，可以试试。/show-me as an html explainer。
```

另外还有一种极简的方法，直接让咱的 Work Buddy 去找“show me”这个 skill，然后让它装下来。

或者想要效率更高，可以打开 Work Buddy 加上 GitHub 的连接器，之前的内容也教过大家如何安装这个连接器，直接让workbuddy通过GitHub 连接器去搜。

![致敬好老师，送你 Buddy 好搭档，认证老师尊享积分好礼｜选择工作空间√](https://mmbiz.qpic.cn/sz_mmbiz_png/XXRDicaNweLpiapEmTnWZxezJP4Oltj239N47ZQwj9ldncVZBBXbib2JCN5iah76tlPX7Fn75WOuMn1saX9LyamXGM7XZVptacVeznToNYVSmfs/640?wx_fmt=png&amp;from=appmsg#imgIndex=14)

*致敬好老师，送你 Buddy 好搭档，认证老师尊享积分好礼｜选择工作空间√*

反正这个 Skill，我现在是准备留在 WorkBuddy 里了。以后再碰到那种 AI 讲了三屏，我看完还得自己在脑子里重新画一遍的东西，我估计也懒得继续让它解释了。

## 直接一句：/show me。
能画明白的，就别写那么多了哈哈。
