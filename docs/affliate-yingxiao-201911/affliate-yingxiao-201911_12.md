# 很多人知道我曾经也

富布斯 : 很多人知道我曾经也是某上市公司搞技术的码农，我 一直觉得技术做的好的人，收入怎么着都可以碾压很多职场 人的，毕竟互联网上有太多的赚钱生意需要技术驱动运营。

所以今天我邀请一位同样从知名上市 M 公司辞职出来创业的 技术大牛 「梁雨」作客《Affiliate 营销圈》分享一些他所触及 Affiliate Markerting 一些有价值的干货！他此前是负责 M 公司的 联盟系统、AFF Tracker 的研发。

说梁雨是技术偏执狂毫不夸张，明明凭借一身好技术就可以 赚到让人艳羡的收入，却选择全职独立开发一款为 Affiliate 而 生的追踪器：Just a Tracker！面对 Voluum 这样的头部追踪器， 大有当年国内第一程序员求伯君的 WPS 大战 MS Office 的异曲 同工之处，除此之外，梁雨还研究过 DSP 平台、劫持、Cloak 系统，对于 Affiliates 来说这些技能既神秘又是进阶分水岭。

Media buyer！最常规的工作就是 SPY，购买各种 SPY Tools（竞争情报工具），比如 AdPlexity、 家的 Idvert、 Adsxposed 等等），大多数人都是 SPY 大牛盈利的 LP、 Creatives、Angles，Offers……从中实现快速套利。 反过来 想，当你的 Offer 也已经实现获利并要放大规模时，你是否担 心被竞争对手和广告主 SPY，谁会动你的奶酪？

今天我邀请梁雨跟我们聊聊一个 Affiliates 关心却鲜被人提及的 话题「如何有效防止被人 SPY？」，Enjoy！

———————————————

感谢富布斯邀请我在这里分享一些个人在防 SPY 上的心得经 验，我知道「Affiliate 营销圈」有不少低调的 Aff 大佬，在这里 分享的是个人对这块的理解，欢迎有更好方案和想法的大佬 来指正和交流！

一，LP（Money Page）防 Spy 原理 图 1

我们先来看一下，整个转跳的过程。用户首先访问的是追踪 的地址(Campaign Link)，之后转跳到 Landing Page，用户点击 Landing Page 之后，跳去联盟/广告主页面。我们需要保护的是 LP，国外喜欢叫做 Money Page.

二，什么是防 spy? 如何防 spy?

防 spy 是指: 防止竞争对手，广告主抄袭你的 lp、创意。只让正 常的用户访问你的 Money Page.

关于如何防 spy 的问题，我们先明确一点，正常的用户，必定 是先经过你的追踪,再跳到 Money Page 的。直接访问 money page 的都是 SPYer。非正常用户。

三，如何验证用户是从追踪跳到 LP 的，而不是直接访问 LP? 图 2 通过”数字签名”：追踪为进来的每个点击，生成一个签名。

并通过参数传到 LP。LP 放一段 ”校验代码”检查签名是否合法

即可。

我们可以把签名理解成一把要钥匙。”校验代码”就像一把

锁。钥匙对了，才能开锁(访问 Money Page)

下面为大家提供两个测试地址。

测试地址(点击，可以正常打开 lp,10 秒后刷新，发现已经失 效。打不开了)

测试 LP(打不开，没办法直接访问) 四，如果 adp、SPYer 是通过爬虫技术，从开发者的网站上抓

取 Campaign link，这种情况如何应对?

1、过滤非目标国家的流量(你投的单子是台湾的，非台湾流 量禁止访问)

2、过滤机房 IP(aws,谷歌云，啊里云, linode 等等) 3、过滤 v 屁 n IP

如上三个功能，通过 ip2location 的 ip 库和匿名库就可以实现。 实现了这三个功能之后，只有真实用户的 ip 才可以正常访问 LP。对于大多数个人 spyer 想要打开你的 LP 已经非常困难。

4、收集 Spy 工具的 ip.

一般 spy 工具，像 adp 等, 机房 IP 和代理 IP 至少占 80%以上。那 剩下的 20%真实 ip，就需要平时的不断收集了。 如何准确快 速地收集 spy 工具的 ip? 想要打败敌人就得深入敌人内部。多去

spy 工具，查自己的 lp 域名，看看能不能找到自己的 lp。发现自 己的 lp 后，可以通过 lp 地址里的”签名” 反查服务器 log，找到点 击的信息，把 ip 入库。 当然你还可以为每一个用户种一个永 久性的 Cookie, 当 spy 工具，只换了 ip，而没有清 cookie 的时 候，就很容易把他们关联起来，一网打尽！

五，如果公司、团队并没有开发自己的 Tracker，而是用 saas 类 型的追踪，并没有 lp 签名这个功能，该如何实现?

图 3 其实方法也很简单。在追踪与 LP 服务器之间，加一个”网

关”，实现上述的 cloak 逻辑、lp 签名。然后转跳到 lp。同样可

以实现防 spy。不过缺点也显而易见。多了一层转跳。必定增

加部分点损。

关于梁雨提到的 LP 签名和 LP 签名校验代码，已发布到

「Affiliate 营销圈」社区，需要的下载：

感谢！梁雨的分享真的很真诚，很干货，其实他的 JustATracker 追踪器本身就已经内置 LP 防 SPY 功能了，诸如全 球部署、域名预警、自动优化都是 JustATracker 的基本功能， 其它的大家有兴趣自己体验吧。借此契机，我也跟梁雨跟圈 里的朋友要了个小福利，通过这个链接注册的朋友，可以免 费试用两周！

对于一款优秀的追踪系统，一个防 SPY 的技术细节要求就已 极为苛刻，更何况在整个追踪系统的生态需要如此强壮完

美，同为技术人，梁雨对于技术的追求和狂热是老富我所无 法企及的。写的一手好代码，做出一款好产品，关键是还忍 的了寂寞…..我..连最后一点臣妾都做不到，嘿嘿 ~

相关阅读：

[`demo.justatracker.com/lp_protection/signat...`](https://demo.justatracker.com/lp_protection/signature.php) [](https://bbs.fuyuzhe.com/affiliate/305.html) [`demo.justatracker.com/lp_protection/test_l...`](https://bbs.fuyuzhe.com/affiliate/305.html) [「如何有效防](https://bbs.fuyuzhe.com/affiliate/305.html) [](https://bbs.fuyuzhe.com/affiliate/305.html) [止](https://bbs.fuyuzhe.com/affiliate/305.html)[LP](https://bbs.fuyuzhe.com/affiliate/305.html)[被](https://bbs.fuyuzhe.com/affiliate/305.html)[SPY](https://bbs.fuyuzhe.com/affiliate/305.html)[？」代码分享：](https://bbs.fuyuzhe.com/affiliate/305.html)[LP](https://bbs.fuyuzhe.com/affiliate/305.html)[签名和](https://bbs.fuyuzhe.com/affiliate/305.html)[LP](https://bbs.fuyuzhe.com/affiliate/305.html)[签名校验代码](https://bbs.fuyuzhe.com/affiliate/305.html)[+-](https://bbs.fuyuzhe.com/affiliate/305.html)

[+Affiliate](https://bbs.fuyuzhe.com/affiliate/305.html)[营销圈](https://bbs.fuyuzhe.com/affiliate/305.html)[+-...](https://bbs.fuyuzhe.com/affiliate/305.html) [Just+A+Tracker](https://dash.justatracker.com/%23/184/Signup) [Affiliate](https://mp.weixin.qq.com/s/KtkKX0KkMlJ2ALBtjiHg1w)[欺骗的艺术（一）](https://mp.weixin.qq.com/s/KtkKX0KkMlJ2ALBtjiHg1w) [](https://bbs.fuyuzhe.com/affiliate/305.html) [Affiliate](https://bbs.fuyuzhe.com/affiliate/305.html)[欺骗的艺术](https://bbs.fuyuzhe.com/affiliate/305.html)[(](https://bbs.fuyuzhe.com/affiliate/305.html)[二](https://bbs.fuyuzhe.com/affiliate/305.html)[)+Cloaking](https://bbs.fuyuzhe.com/affiliate/305.html) [「如何有效防止](https://bbs.fuyuzhe.com/affiliate/305.html)[LP](https://bbs.fuyuzhe.com/affiliate/305.html)[被](https://bbs.fuyuzhe.com/affiliate/305.html) [](https://bbs.fuyuzhe.com/affiliate/305.html) [SPY](https://bbs.fuyuzhe.com/affiliate/305.html)[？」代码分享：](https://bbs.fuyuzhe.com/affiliate/305.html)[LP](https://bbs.fuyuzhe.com/affiliate/305.html)[签名和](https://bbs.fuyuzhe.com/affiliate/305.html)[LP](https://bbs.fuyuzhe.com/affiliate/305.html)[签名校验代码](https://bbs.fuyuzhe.com/affiliate/305.html)[+-+Affiliate](https://bbs.fuyuzhe.com/affiliate/305.html)[营](https://bbs.fuyuzhe.com/affiliate/305.html) [](https://bbs.fuyuzhe.com/affiliate/280.html) [销圈](https://bbs.fuyuzhe.com/affiliate/280.html)[+-... Voluum](https://bbs.fuyuzhe.com/affiliate/280.html)[中文使用手册](https://bbs.fuyuzhe.com/affiliate/280.html)[+-+Affiliate](https://bbs.fuyuzhe.com/affiliate/280.html)[营销圈](https://bbs.fuyuzhe.com/affiliate/280.html)[+-](https://bbs.fuyuzhe.com/affiliate/280.html)

[+Powered+by+HYBBS Adplexity+](https://bbs.fuyuzhe.com/affiliate/306.html)[官方使用教程（中文](https://bbs.fuyuzhe.com/affiliate/306.html) [](https://bbs.fuyuzhe.com/affiliate/306.html) [版）](https://bbs.fuyuzhe.com/affiliate/306.html)[PDF](https://bbs.fuyuzhe.com/affiliate/306.html)[下载](https://bbs.fuyuzhe.com/affiliate/306.html)[+-+Affiliate](https://bbs.fuyuzhe.com/affiliate/306.html)[营销圈](https://bbs.fuyuzhe.com/affiliate/306.html)[+-+Powere...](https://bbs.fuyuzhe.com/affiliate/306.html) [](https://bbs.fuyuzhe.com/affiliate/91.html) [Affiliate+Marketing](https://bbs.fuyuzhe.com/affiliate/91.html)[中文教程系列七：提升](https://bbs.fuyuzhe.com/affiliate/91.html)[LP](https://bbs.fuyuzhe.com/affiliate/91.html)[加载速度的建议](https://bbs.fuyuzhe.com/affiliate/91.html)

[+-+Affiliate...](https://bbs.fuyuzhe.com/affiliate/91.html)

2019-05-08(29 赞)

评论区：

富布斯 : 为鼓励国内的追踪系统崛起提供动力.[微笑]

兴国 : 支持国产！

杨永歌 : 加油

刘国兴 : 雨哥厉害

ins 老王 : 牛 B 啊

![image](img/Image_038.png)

小蛤蟆喝甜汤 : 码农厉害

余恒威 : 支持国产 码农厉害

![image](img/Image_039.png)

关注公众号"懒人找资源"，星球资源一站式服务