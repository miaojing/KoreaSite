# 一个触动我的写法 -- 语义化是无障碍的基础

继去年解决淘宝关键购买关键路径的无障碍问题后，最近淘宝无障碍前端兴趣小组重新出发，立足跟进解决用户反馈的无障碍问题和无障碍相关技术研究。众所周知，更好的语义化有利于搜索引擎、读屏软件等机器的分析识别，注意下语义化问题基本解决了常见web无障碍问题（input label/img/a等）的70%的问题，其实这些web开发者都知道，只是有时为了更简易实现而忽略了。语义化的改善不光对机器（搜索引擎、读屏软件等）更友好，有时正常的我们也可以从中受益，分享一段最近看源码被触动的小经历:)

2个月前，无线业务改版视觉风格和业务内容参考韩国电商，会点韩语看着无违和感，索性就翻译了[几大韩国电商网站](https://github.com/miaojing/KoreaSite/)。在翻http://m.daum.net/的排行榜模块时，大部分词汇看不懂，就随手复制到google翻译，翻译出来一句很顺畅的话，额，明明只复制了一个词，竟然能构成一句话，发现原来复制后粘贴板上多了几个词。
![](http://gtms01.alicdn.com/tps/i1/T1S6q4FdheXXXfXYUc-386-451.png)
![](http://gtms02.alicdn.com/tps/i2/T1k3y7FlJXXXaenoEl-846-154.png)

真相在源码里面：
![](http://gtms03.alicdn.com/tps/i3/T1nPC3Fe0gXXXaYiHl-703-260.png)
![](http://gtms04.alicdn.com/tps/i4/T1L.9MFodgXXXIBVn3-411-176.png)





