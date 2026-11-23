---
title: "用豆包工作做了个 skill， 自动剪辑旅行 vlog"
source: "https://workbuddy.jiangyufan.com/index/hub/skill/413"
type: "skill"
chars: 1442
sections: 0
figures: 0
chapter: "10-我要写代码和做自动化"
---

# 用豆包工作做了个 skill， 自动剪辑旅行 vlog
![用豆包工作｜做了个自动剪辑](https://mmbiz.qpic.cn/sz_mmbiz_png/CFe2b8yvCoxElTViadLdhtfg9Qb2MazPGLxGiazGpUSSzdTsgUq28JJDx8URQU7M01jkibLWfu21o1Kgrq9kCsMZIAVR226aUepnZaxKuVHxU4/640?wx_fmt=png&amp;from=appmsg#imgIndex=0)

*用豆包工作｜做了个自动剪辑*

前两天做的地图动效 skill，放到豆包工作里，也可以输出很完美的动效。于是我在豆包工作里，对这个动效 skill 做了一些优化。

现在它可以输出 3D 形式的地图动效，根据照片找到拍摄机位，还能直接拿一系列照片来制作旅行 vlog。效果如下：

![](https://mmbiz.qpic.cn/mmbiz_jpg/CFe2b8yvCoxNFfjJssyJdgFDxicBFBkicBibL4sJyZZsk3KSBnExhkNHeJ872EtXglI929AA0viagxuqiaRI9TMZAOdbgbPUHWeyTnIDaQQrHXWo/640?wx_fmt=jpeg#imgIndex=1)

最好用的是下面这条，我用云南自驾的照片做的 vlog 成片：从地球俯冲定位到虎跳峡开始，Q 版小人沿着真实路线一颠一颠走，每到一站停下来拍张照，照片一张张弹出，片尾照片墙收尾。

下面就展开讲讲，怎么使用这个 skill，我全程都是在豆包工作里使用的。

第一步，安装 skill。发送给豆包工作：安装这个 skill：SpaceZephyr/travel-vlog。

![h/SpaceZephyr/travel-vlog 安装这个 skill，告诉我｜安装完成，一切就绪。下面是安装结果和使用说明。](https://mmbiz.qpic.cn/sz_mmbiz_png/CFe2b8yvCozbZicTdyYtzQuzUzaibVa1LbWZkwQfkq9o07tUiaBRdsy00Z3ePX27qqsUjkZvhfPQgu5ic7eeVE8lLHd6cTvdgeI1457MlzwBuQU/640?wx_fmt=png&amp;from=appmsg#imgIndex=2)

*h/SpaceZephyr/travel-vlog 安装这个 skill，告诉我｜安装完成，一切就绪。下面是安装结果和使用说明。*

Map-motion 里有多个子命令：plan（机位规划）、avatar（形象生成）、check（成片质检）、make（渲染成片）、status（查看状态）。

第二步，给照片。如果你要制作旅行 vlog，需要提供你旅行拍摄的一些照片。

最简单的方式，是直接提供你发在网络社媒上的链接，如下图用的即刻的帖子链接。链接里包含你发的图，它会自动下载，一张不落。

![(1)消耗0.04% 昨天17:53｜下载这个链接里的图片，根据这几张图片，制作我的旅行 vlog](https://mmbiz.qpic.cn/sz_mmbiz_png/CFe2b8yvCowLEk64xPnNdQ1d3UxxfohIWicEb70WbopXmLGMSut3p3RmUMpX7ssjib10T2qKtvJof9ibHZtINia1uJM3Icht4M06sWicAmYM26EQ/640?wx_fmt=png&amp;from=appmsg#imgIndex=3)

*(1)消耗0.04% 昨天17:53｜下载这个链接里的图片，根据这几张图片，制作我的旅行 vlog*

然后就可以等待豆包工作来制作成品了。模型会根据图片里你个人的照片，设计几个动漫 IP，用作视频里的小人。

![](https://mmbiz.qpic.cn/mmbiz_png/CFe2b8yvCoxh8y9WrkPN8HXJexbqr039edvftrnpXcTvOMRFswnzNrBVt710xK5LV1D1FKiccqDibvbcHzXomtsbBaeZPDgmswHxMNpbeNJY8/640?wx_fmt=png&amp;from=appmsg#imgIndex=4)

这里必须得夸夸豆包工作自带的多模态生成能力。

只需要上传一张你的旅行自拍，它就能无缝输出 Q 版贴纸：走路姿势、拍照姿势，两个姿势都能生成，还会自动把背景抠成透明的，直接做成视频里的小人素材。

Q 版小人形象（走路/拍照双姿势）。

![](https://mmbiz.qpic.cn/sz_mmbiz_png/CFe2b8yvCoxHBw3u4U9fMu5Tf2e8gWcuS5LqU4iaY9KojWKSgibmRNP9HwVUODfJb3lZ6vpzOx1bPyg5icibqg48icrO9L2cibM3WGZYxfZ6vJhbI/640?wx_fmt=png&amp;from=appmsg#imgIndex=5)

有了照片之后，豆包工作会根据图片中的特征，挑选出这些照片的拍摄位置，然后在地图上标注出来。照片里没有 GPS 也没关系，它会根据画面内容推断机位，再匹配地图上的真实地点。

![](https://mmbiz.qpic.cn/mmbiz_png/CFe2b8yvCozxzHSibe8usa1c3icTpzKkCovU7iaM9Kv4KQRHIGLh3nRz6bR42GRKJbDQgNuCNhjt6AgwjKib1kmGm8629B3icV7wcZHFcmOM3fks/640?wx_fmt=png&amp;from=appmsg#imgIndex=6)

我这次的照片就是从社媒链接下载的，定位信息早被转码剥掉了，它照样把三个机位，虎跳峡、梅里雪山、雨崩。在地图上标得明明白白，连站点之间的驾驶里程都算好了。

懒得发照片的话，你也可以试试把小红书的链接发给它。如果你想要更精确的路线，也可以对话，提供更详细的旅行路线。它就开始制作视频、配乐，交付 mp4 格式的视频和 gif 格式的动图。

至此，我们通过一个链接，就获得了一个一分钟左右的炫酷旅行记录视频。一张网图都没要，一张照片都没修，全自动。

还没。如果你觉得这个视频做的不够完善，或者你手里有大量的视频素材，需要自己来剪辑。这个时候，你可以调用剪辑 skill，来把生成的动效视频，作为你创作的 vlog 里的一个片段。

先安装这个大佬制作的开源 skill：luoluoluo22/jianying-editor-skill。

![/luoluoluo22/jianying-editor-skill 安装这个 skill｜安装完成。](https://mmbiz.qpic.cn/mmbiz_png/CFe2b8yvCoybjdibduTqov0SUmfxGPvO3TQnzib6oAPnMb3DLygLKMA7qdDEsXViaaw2yv6qaAiaHRoETxRKOibWgicYL5f8yqtJUwDDY0wUxHTew/640?wx_fmt=png&amp;from=appmsg#imgIndex=7)

*/luoluoluo22/jianying-editor-skill 安装这个 skill｜安装完成。*

然后让它根据视频素材制作剪映的工程文件。有了像下面这样的轨道可以可以剪辑字幕、音效、添加自己拍摄的视频。

![第1站·出发·202｜第2站·已走2894](https://mmbiz.qpic.cn/sz_mmbiz_png/CFe2b8yvCowPSvrOIjzeA4QL8e6dsgp5U3gdLickfZxbHicT97leT0ZadtKMibNHeoVWrhRxw9djPiaOrYyT8WF6jmiatQOZouSCUzCEug6st5Ro/640?wx_fmt=png&amp;from=appmsg#imgIndex=8)

*第1站·出发·202｜第2站·已走2894*

我经常是有大量的视频素材，懒得剪辑。就可以让豆包工作调用剪辑 skill 来粗剪一版，这就解决了我旅行 vlog 的制作大难题了。

豆包工作大家想要用的话，可以在网页搜索豆包工作下载电脑端，还可以领取最高60天会员权益。
