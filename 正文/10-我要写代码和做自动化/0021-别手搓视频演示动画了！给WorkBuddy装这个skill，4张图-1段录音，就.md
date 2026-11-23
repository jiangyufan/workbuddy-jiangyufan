---
title: "别手搓视频演示动画了！给WorkBuddy装这个skill，4张图+1段录音，就"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/366"
type: "skill"
chars: 2925
sections: 5
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 别手搓视频演示动画了！给WorkBuddy装这个skill，4张图+1段录音，就
我是可可，广东潮汕人，2个孩子的妈妈，新教育践行者，AI一人公司实战圈共创主理人，专注于研究AI+一人公司提效与变现。

![别手搓视频演示动画了！｜给WorkBuddy装这个skill就能自动生成完整演示视频](https://mmbiz.qpic.cn/mmbiz_png/ATa6yEDN5ayAfRXCZJKQeTa4moF7YsRQc0yYpLOFzcxvrKH9hOwAH8AnegD5W0DR1quXIuiaQ3myLTdIeNMwBIibyT4kR7kdBxcqNeSdKKbjM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=0)

*别手搓视频演示动画了！｜给WorkBuddy装这个skill就能自动生成完整演示视频*

以前做演示视频，最耗时间的并不是写稿，也不是录音，而是打开剪辑软件后，要一再重复这一套，听录音 → 找时间点 → 对画面 → 播放检查 → 发现画面提前了 → 再往后挪 → 重新导出。

我明明只是想把一个操作讲清楚，最后却被迫同时做导演、动画师和剪辑师。录音可能只有一分多钟，为了让这一分多钟的画面，却要在剪辑软件的时间轴上反复折腾几个小时。

更磨人的，是口播讲到了，手里却没有对应的画面，可能只有那么几张操作截图。为了不让画面一直空着，只能自己去找图、截界面，有时还得临时手搓一张图补进去。

一分多钟的视频，光是给每段口播找合适的画面，就能磨掉不少时间。这次我尝试完全交给WorkBuddy去完成。

我没有打开剪辑软件，只准备了1 段口播录音、3 张截图和1张封面，然后把它们交给 WorkBuddy。

最后，它给我做出了这样一条完整的演示视频。成片一共 1 分 40 秒，3:4 竖版。WorkBuddy 根据口播和截图，自动补了一些简单画面，把原本只有几张截图撑不住的地方接了起来。

刚开始走这个流程，有些地方还要调试，中间也出现过画面太静、转场空白、音画错位这些问题，但我知道这将是一个做演示视频的新方式了。

最让我轻松的地方就在这里，不需要回到时间轴上自己挪，而是直接告诉 WorkBuddy 哪里不对，让它继续改。

下面我来将整个操作过程告诉大家。

## 一、先给 WorkBuddy 装了一个做视频的 skill。
打开 WorkBuddy 的【技能】，搜索 remotion，找到了一个 Remotion 视频生成套件，点右边的“+”装上。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/ATa6yEDN5awAuTYBPsr8dpvwkrlgZlQZ3ia6o3FQZfkh6y4E5NicEDmN0u65pS7gPicE8gzibPq9AWscIKPOrMZ6PmO1U6tFXBvtBBp5jWev99g/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

Remotion 可以用代码来生成视频，这正好适合拿来做演示视频。它可以根据口播生成一些对应画面，把几张截图之间的空缺补起来，不用我再到处找图、做图。

装好以后，我把这次要用的素材放进同一个文件夹：3 张操作截图、1 张封面和 1 段 m4a 录音。

![▶新加卷(F:)▶ workbuddy工作文件夹▶演示动画▶8.13workbuddy演示｜FJE9，我帮你能设计](https://mmbiz.qpic.cn/mmbiz_png/ATa6yEDN5awibACWn6iav5aHgVSs3nY4ZBYl7KNic1oibzYfuOPZyhWNspAOy4a4xL4Vo6iacOsxlzGuPbeOjcqod8Cicibzc0kOOoWRa2D0THW2M8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

*▶新加卷(F:)▶ workbuddy工作文件夹▶演示动画▶8.13workbuddy演示｜FJE9，我帮你能设计*

不需要一张张上传图片，WorkBuddy 本来就能读取电脑里的本地文件，我只要把文件夹位置告诉它，它会自己进去找。

## 二、我把逐字稿和素材丢给它，看它会怎么做。
接着，我新建了一个日常办公任务，把逐字稿和视频要求一起发过去。

![日常办公 代码开发 设计创意｜文档处理 金融服务 数据分析及可视化 个人工作台 幻灯片](https://mmbiz.qpic.cn/sz_mmbiz_png/ATa6yEDN5axnaIw551OMSRfXlg9J8jWR2VKnVjfkM3udSDGAcDAP38cT1Q8urkAWadKw5TFhH7dTx6Cg2Ts7wIN49fS3DiaWHZ21uN4JzQZU/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=3)

*日常办公 代码开发 设计创意｜文档处理 金融服务 数据分析及可视化 个人工作台 幻灯片*

我当时最在意两件事。第一，先把需要的环境和依赖装好，不要做到一半才发现跑不起来。第二，别急着直接渲染，先把分镜脚本给我看。方向不对时，改分镜总比整条视频做完再推倒重来省事。如果你也想做类似的视频，可以直接照着下面这段提示词改。

用 Remotion 视频生成 skill 做一条口播演示视频。主题：《WorkBuddy从零到一，新手指南》 画面比例：竖版3:4 请读取我指定文件夹里的录音、截图和封面。先安装需要的依赖，再根据录音和逐字稿设计分镜。分镜脚本先发给我确认，我确认后再渲染MP4。画面要跟着口播内容走。截图不够的地方，请根据逐字稿生成简单画面补上，同时加好字幕和转场。如果加入背景音乐，不要盖住人声。以下是逐字稿： （粘贴自己的逐字稿）。

任务发出去后，WorkBuddy 先去找对应的 skill，又读取了素材文件夹。

它告诉我，里面有 3 张截图、1 张封面、1 段录音，还把需要用到的 Remotion 工作流一起读了。

![我先调用 emotion 视频生成器 skill，并同时查看你的素材文件夹。｜先建任务清单，并并行做几件事：检查运行环境、读取音炉、长、查看截图内容。](https://mmbiz.qpic.cn/mmbiz_png/ATa6yEDN5ayH3SibZNpN7t5fUpbFWfLa63NcDl2A9j8SWVCa461OEOujy8vicPcOxyZ3450sg6kSLMGuobCyYBZSvk8bzDVsxhe1qmogx9djM/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

*我先调用 emotion 视频生成器 skill，并同时查看你的素材文件夹。｜先建任务清单，并并行做几件事：检查运行环境、读取音炉、长、查看截图内容。*

以前这些准备工作都得我自己做，先听一遍录音，把每段话的时间记下来，再决定这一句配哪张截图、下一句用什么动画，现在我只看它给出的方案合不合适。

## 三、截图太少，我让它自己补画面。
第一轮做出来后，我马上发现了一个问题，我的素材实在太少了，只有 3 张截图，画面看起来也很像一份会自动翻页的 PPT。

于是我直接问WorkBuddy，。

截图素材会不会太少。如果画面总停顿在一个静止的画面上，观众就看不下去了。除了我的截图，你生成动画加上。

把找素材的活交给 WorkBuddy去做，它接到反馈后，开始按照口播内容补画面。

![制作WorkBuddy新手指南口播视频｜今天帮你做些什么？@引用对话文件，/调用技能与指令](https://mmbiz.qpic.cn/mmbiz_png/ATa6yEDN5azR93mc3vjtVc3XqhctQibqialp214c1icKwXMibql2qwpx9LBz9tY23vOwkicXgeZzyoX7414pzq1THCQ2YASjr9VicITdUf2IiayYKw/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=5)

*制作WorkBuddy新手指南口播视频｜今天帮你做些什么？@引用对话文件，/调用技能与指令*

它根据逐字稿，生成了几段简单的图文画面，接在我的截图之间。

它确实把原本缺画面的地方填上了，不是从头到尾只轮流播放那 3 张截图，虽然画面还不是很精细，但这些后面都是可以再调整的。

## 四、第一版有问题，我也没再碰时间轴。
画面动起来后，我以为已经差不多了，从头播放一遍，又发现画面和画面之间切换得太慢，中间空了一截。我把这个问题继续丢回原来的任务，让它重做。

![需要我调画面风格、时长分配，或导出 9:16 竖屏版（更适合手机全屏刷）吗？](https://mmbiz.qpic.cn/mmbiz_png/ATa6yEDN5az1DdibRPicl9AFYaIdsMO2tJXYgBbSibT8Jvq2bKW1OPicBCDeEpvNic3zRV9bFHribzBhsmRIzdEJWIbNw5CDGDycJhyadjBRQ0ekQ/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

*需要我调画面风格、时长分配，或导出 9:16 竖屏版（更适合手机全屏刷）吗？*

新版本出来，我又看了一遍，这次空白少了，但画面和配音还是没对上。口播还在讲第三步，画面已经跑到了第四步。另外，视频里也没有听到背景音乐。

这种问题，我以前太熟悉了，只能重新听录音、找时间点、把画面往后挪。前面一改，后面几十秒又可能全部跟着错位，改完还要重新导出，再从头检查。

但这次我只回了它一句：还是画面和配音对不上，画面出现早了。另外，没有听到背景音乐。

WorkBuddy 收到后，重新检测了整段录音里的停顿，又按照逐字稿，把每一段画面的真实起点重新锁了一遍。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/ATa6yEDN5ay5EFhtth8zbA5SUfXUZ8nbd3swdy29VdQV2etDH8vciaSia886picbJ9PTrcibZqiaib6fpnia3eOb8UjBMCicN5wnglrrMQGFt0ichBbg/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=7)

它甚至把问题说得很具体：上一版某一段画面在 61.6 秒就开始了，但我的口播到 64.67 秒才真正讲到这里，整整早了 3 秒。

就算是3 秒，放在以前手搓视频时，那是非常磨人的。现在它自己找到了，还把后面的时间轴一起重新对齐，再重新渲染。

至于背景音乐，它虽然说已经处理了，但我在最终成片里还是几乎没听到，应该是音量还没调好，这就是开头看到的成片。

## 五、我喜欢的不是“一次生成”，而是可以继续使唤它改。
这条视频并没有第一次就做对，截图太少，画面会闷；转场留白太长；配音和画面对不上；背景音乐也还没有处理好，可这些问题没有把我重新赶回剪辑软件。

我做的事情变成了看成片，然后用平常说话的方式告诉它：这里太慢了，那里早了，音乐没听到，再改。它负责回去找原因、改代码、重排时间轴，再交一版给我检查。

这个 skill 最适合的，并不是对每一帧都有严格要求的专业剪辑。它更适合我们平时常做的工具教程、产品演示、课程讲解和工作汇报。

尤其是手里只有一段录音和几张截图，又不想让视频像静态 PPT 的时候，它确实能接走很大一部分苦活。

当然，最后还是要自己从头看一遍，画面有没有跟上口播，转场有没有空白，背景音乐到底能不能听到、音量是否合适，这几件事 AI 还需要人来判断。但已经是很大化地解放了我的劳动力了。

我再也不用为了那一分多钟的视频，坐在时间轴前反复挪几个小时了。关于作者：我是可可，一人公司实践者，AI一人公司实战圈共创主理人，教你怎么用AI提效，搞定IP、流量和变现。
