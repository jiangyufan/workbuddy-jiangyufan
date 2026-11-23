---
title: "我基于 WorkBuddy做错题整理：识别只是入口，后面五件事才关键"
source: "https://workbuddy.jiangyufan.com/index/hub/case/455"
type: "case"
chars: 1879
sections: 7
figures: 0
chapter: "02-我是老师"
---

# 我基于 WorkBuddy做错题整理：识别只是入口，后面五件事才关键
![](https://mmbiz.qpic.cn/sz_mmbiz_gif/I8KTaDpq0FhaHlM1Z2qblUBdwAvZ2UIA2YMbKQnibx0oAGhdHaTt2JTA8Hr0eFn7UeqaOtrRPkNPiakeiauAAiajx1WbkKXIgD24UUshwooia4Kg/640?wx_fmt=gif&amp;from=appmsg#imgIndex=0)

这一步当然要有。但如果只做到这一步，得到的还是一本「抄得更快的错题本」：题目省了手抄，可学生错在哪、什么时候再练、练什么，都没变。

我自己基于 WorkBuddy 搭了一套错题整理流程，给我带的初中生和四年级班上用。这篇不讲按钮怎么点，只讲背后的逻辑：

识别只是入口，真正决定错题本有没有用的， 是识别之后的五件事。

## 一、整体流程只有三步。
把试卷和答题卡拆开。文字转成 Markdown，公式用 LaTeX 写，最麻烦的是图——试卷上的图不直接截，而是用 TikZ 照原图重绘。

汇总错题。把学生的作答对到每一小问，挑出失分的部分。重新排版。用我现有的排版系统，按预设格式把错题排成一本能直接打印、能直接写的错题本。三步本身不稀奇，谁都能想到。下面五件事，才是我花时间最多的地方。

## 二、题目只存一份，产物可以有很多种。
我录入的每道题都会变成一张「题卡」：题干、小问、答案、图，还有这道题的属性。错题本是从题卡排出来的，试卷、课时作业也是从同一批题卡排出来的。

题卡一份、规则一份、产物多种。这样做有两个好处：同一道题改一次，所有用到它的地方都跟着对。「这张图是作图题、原卷印多宽、不能压」这类事实只记一次，记在题卡上，而不是记在某一份产物里。

这也是我坚持把图重绘、而不是截图修干净的原因。截图修得再干净，也只是一张图片；重绘出来的图是代码，能换数、能改条件、能按原卷宽度排，后面做变式题时它才用得上。

![录入第一步:图不截，重绘｜截图只是一张图片，重绘出来的是代码](https://mmbiz.qpic.cn/mmbiz_png/I8KTaDpq0FjPSJZVc6ULKbEibREp895Veda3Rktpib6yer5hyCE3c7orpJQ13tN8HbgsJSyIg8Dq7P6wtPI5HicVGNufzibcBIqqb6FJXRMbgpA/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=1)

*录入第一步:图不截，重绘｜截图只是一张图片，重绘出来的是代码*

左边是原卷截图，右边是 TikZ 重绘。

小学和初高中也不分两套：一个排版引擎，两套学段参数。差别只是作答区留多高、反思写几问，规则本身是同一套。

## 三、只收失分的那几小问，作答区不压缩。
一道大题有三问，学生只错了第二问，错题本里就只印第二问（题干照印，不然没法读）。整题照搬，学生会把已经会的再做一遍，时间花在不需要的地方。

版式上我用的是「折叠版」：左边是题，右边留出写的地方。作答区够写才算数，宁可多一页也不把格子压小。末尾留一页反思：初高中生四问，四年级简化成两问。

![](https://mmbiz.qpic.cn/mmbiz_png/I8KTaDpq0FiaVL96JFYicqzL8xW6mrQBRDgn4qYhyzeUEptTQ4qiaza2gzEz8ic41QIOPmINJBYXCBeX7qdLJP9qWFX9DiadvVvFAkjibC7pLz8V8/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=2)

四年级的一页折叠版：沿中线向后折，左边看题，右边自己写正解、思路、题型和错因。

## 四、先分错型，再决定怎么练。
不是每道错题都值得做变式题。我先把错误分成三类，处置完全不同：错型。典型表现。怎么练。执行失误。算错、抄错、填反。重做原题就够。概念没抓住。换个样子就不认识了。用反例和「非概念变式」，把本质逼出来。条件没用。漏看一个条件、少走一步。一次只改一个条件，看他能不能跟着变。

后两类用的是变式教学的思路（顾泠沅、鲍建生）：本质不动，只变非本质的地方，而且一次只变一个维度。

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/I8KTaDpq0FjDGx1icvIicFKOBmVoVU1nKpIaAew8364EibOBqUY98wibvjGtCWKUvX2FIsgCgPI3IJ7MpmClIDobia8wwic8KTW7qpT3Ck3lYWytE/640?wx_fmt=gif&amp;from=appmsg#imgIndex=3)

错型由老师判，不交给 AI 猜。算错和概念没懂，卷面上常常长得一模一样，要靠我对这个孩子的了解、有时还要当面问一句，才分得清。这一步分错了，后面练得再多也是白练。

## 五、不在当周做完，隔开、少量、多次出现。
很多错题本的问题是：当周订正，当周再做三道同类题，全对，看起来掌握了。但这多半是趁热记住，隔两周再考又错。

我的节奏是一道错题出现三次，每次换一道新变式：

![](https://mmbiz.qpic.cn/mmbiz_png/I8KTaDpq0FiaRgubfj13PJIb4TaxP2fCQS8oE97CMtvkWxzBTiayHA3XgribsUkyzoDNVFyrdOFaomp3Rq9a2YUSVvtUTEGHiaZKUYS2Tiatpu6c/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=4)

第一次。约 3 天后，兼做诊断——订正没改到位的，这时就暴露了。第二次。约 10 天后，混在新题里出。第三次。3～4 周后，反过来问或换个情境。

连续两次做对就退出，做错就回流，重新进入这个节奏。这背后是认知心理学里的间隔效应：同类题别一次刷完，隔开再提取，记得更牢。

## 六、AI 管「送到面前」，想明白留给学生。
很多 AI 错题工具主打「AI 帮你分析为什么错、怎么改」。我刻意没这么做。

学习真正发生的地方，是学生自己对着题想、自己动笔做的那一刻。AI 替他把「为什么错」讲明白了，他读懂了，不等于他会了。所以在我这套流程里，系统只管两头：

输入端。挑哪道题、什么时候、以什么样子送到他面前。反馈端。他做完还错不错，据此调整下一次推什么。中间那段，留给孩子自己。

## 七、为什么基于 WorkBuddy：方法写成文件，壳和模型都能换。
这套东西我没有写成一个「产品」，而是拆成几层文件，放在本地：

![](https://mmbiz.qpic.cn/sz_mmbiz_png/I8KTaDpq0Fh6nFYYZsstITZx80icJic1GfNwQUma17GsKNkicC28iaWtJdic2iaByuTdVxL8WicC9te4Z7B2m7sKPibrUhKuzE9xr2SFBC3KQzxdM14/640?wx_fmt=png&amp;from=appmsg&amp;watermark=1#imgIndex=6)

最后一层值得多说一句。只写在说明里的规则，模型偶尔会忘；写进脚本，脚本每次都会检查。所以要紧的护栏我两头都放。

这样分层的好处是：方法是我的，写在文件里；壳和模型都可以换。今天用这个模型，明天换一个更好的，错题本的逻辑不用重来。

如果你只想先做一件事，我建议从第四节开始：下次改卷，在每道错题旁边标一下，它是算错、概念没懂，还是条件没用。

这一步不需要任何工具，但做完之后你会发现，错题本该怎么做，答案已经出来了一大半。

![](https://mmbiz.qpic.cn/mmbiz_gif/I8KTaDpq0FgELddN0XMibj2oI2UPwGxTv4EriaBZkXMm7gibADqoN9nQbMYeIDHsVycDj8cKwrZe3xTs7ODPiapx1ia68pwbLHxzZ3mNI3bKrD7o/640?wx_fmt=gif&amp;from=appmsg#imgIndex=7)

![](https://mmbiz.qpic.cn/sz_mmbiz_gif/I8KTaDpq0Fg3icEF4wkBnbMDJpxcOTp2bJudy4wTqFUz96IY4LyME8qiacvxDRTR6HunD9MVCwKEWml9ibB7EfUoqEGwoKGvIYEu6s4sJEuPz4/640?wx_fmt=gif&amp;from=appmsg#imgIndex=8)
