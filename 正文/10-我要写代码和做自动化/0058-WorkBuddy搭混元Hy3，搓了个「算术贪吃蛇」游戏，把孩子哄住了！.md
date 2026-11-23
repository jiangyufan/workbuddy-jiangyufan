---
title: "WorkBuddy搭混元Hy3，搓了个「算术贪吃蛇」游戏，把孩子哄住了！"
source: "https://workbuddy.jiangyufan.com/index/hub/case/649"
type: "case"
chars: 918
sections: 0
figures: 0
chapter: "10-我要写代码和做自动化"
---

# WorkBuddy搭混元Hy3，搓了个「算术贪吃蛇」游戏，把孩子哄住了！
上回趁着混元Hy3免费，我复刻了小时候那款经典坦克大战。虽说没做到像素级还原，但也够用了，毕竟给家里小孩玩上了。他玩得特开心，还问我说：爸爸你是做腾讯云 AI 的，是不是以后能给我弄好多小游戏。

当然，我不是什么 vibe coding 高手，在不少人眼里这就是个前端网页，没什么技术含量。可看着孩子玩得不亦乐乎，对我来说就够了。

眼看混元Hy3 免费进入倒计时，也不知道会不会续期。趁还免费，又有个新点子：「把算术做进贪吃蛇游戏」。游戏不能只图个爽、刺激一下多巴胺，还是得跟教学揉在一起，既能玩，又能顺带帮孩子练算术。

这次的设计，想用一下专家看看效果，就召唤UI设计师像素君。

![像素君 专家 产品设计｜精通设计系统和组件库，追求像素级完美，打造无障碍用户界面](https://mmbiz.qpic.cn/sz_mmbiz_jpg/ABXvT52NoZyGWVTQUDqHGHHHJdl16ibDKr5ibebrC6hkwSq3a6ftNe81AucbhJVicUP5hErlVNCW9ToeJzvqX2fpXLzSMXjicY143Rc68FrWbXw/640?wx_fmt=jpeg#imgIndex=0)

*像素君 专家 产品设计｜精通设计系统和组件库，追求像素级完美，打造无障碍用户界面*

第一轮的提示词：

![G金融服务｜C 数据分析及可视化](https://mmbiz.qpic.cn/mmbiz_png/ABXvT52NoZxpMCp8R1ZaH49bf3br8sKCSCFX3cAIPazm9IOLImPjSc7NtgQqJGefaGHib3ViawicsPGnZaREiaIlJjrr0aVyTvSBLrEDdywACmA/640?wx_fmt=png&amp;from=appmsg#imgIndex=1)

*G金融服务｜C 数据分析及可视化*

在提示词里界面设计这块，如果没有给到定制化的细节要求，做出来的界面风格不会有什么太大的惊喜，一眼html模版风格。这是第一版生成的「数字贪吃蛇」页面，不是很满意。

![吃下正确答案，越算越聪明！｜加减法·1-20 3-6岁](https://mmbiz.qpic.cn/sz_mmbiz_png/ABXvT52NoZwfR61cGxZxFeia3Ec5mvQNJj8iblwGIv1r55FSMZGicweiaHYmojKguFMiaQ1AtA8D8FGh7Dw9zsUHxzOfmAVxgvuqY54SvJJickzZ4/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*吃下正确答案，越算越聪明！｜加减法·1-20 3-6岁*

插个题外话，感觉召唤这个像素君专家有点大材小用了。我不怎样用专家和专家团，最近趁着hy3免费，试着用了几次，交付的产物感觉也没比正常模式下来的质量好啊，而且感觉处理任务还更慢。

回归正题。之后就开始经过多轮的提示词调整，重新设计游戏首页、设置弹窗、游戏区、结束弹窗等模块。这里就不一放修改的过程了。有了上一次经典坦克大战的产出，自己也希望一次能比一次有进步。

以下多次交互调整后，开始首页、难度/时长选择、游戏区页面、游戏结束弹窗的样式：

![算术贪吃蛇｜吃下正确答案，越算越聪明](https://mmbiz.qpic.cn/mmbiz_png/ABXvT52NoZxFNqqorzHH3zZbsyQiauEEXPIT35gvkd6k62XObM6MV9ecF7aPkoa9kcEziaWHVtbXjau3Vvxea1d9TwDw1sUicuJzzk7EbFYTVU/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*算术贪吃蛇｜吃下正确答案，越算越聪明*

![①选择难度｜②选择时长](https://mmbiz.qpic.cn/sz_mmbiz_png/ABXvT52NoZyCj0yPsagbIIgibnEicgE1KbMmM8t8BFicZTZmibTps3Aqcb6uSOeooEbEf0xz0opGn7R3PQiaQaBpf21vwrgCET0Mq97m3cczxhmE/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

*①选择难度｜②选择时长*

![方向键/ WASD 控制方向｜空格/ P 暂停/ 继续](https://mmbiz.qpic.cn/sz_mmbiz_png/ABXvT52NoZzn52DBHn6VwWTMN2seVxTjRUjz2FF7rX27iaC1V6iahlSQ0Dv2cHDPeFCpdlBfJo2Pq4ygRe8ylZUs1DIfaEdAIpuuIeMU3gKmM/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

*方向键/ WASD 控制方向｜空格/ P 暂停/ 继续*

![小玩家的战绩｜历史最高分:129](https://mmbiz.qpic.cn/mmbiz_png/ABXvT52NoZyxjjkojUMNc1uVy9iaWnv23As6VkEFpiae6BiaTpe8bt5TJcEfeE9dCdLCW7r0z0kzvv5lpL821qckcOjEY51DQuaCxtib49jKHs0/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

*小玩家的战绩｜历史最高分:129*

由于考虑小孩子玩，就没设置撞墙失败的玩法，而是可以穿墙到另外一头继续。依旧保持蛇变长后，撞到自己的身体，游戏就失败的设定。

现在有了智能体之后，真的可以创造很多东西给低龄一点的孩子玩，当然现在大点的孩子用AI可比我们很多大人还厉害，脑子也更灵光，可以用AI创造的东西更多。
