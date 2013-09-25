# 韩国电商网站（偏移动版）浅析

韩国电商发达风格也符合亚洲人审美，业界电商都不忘参考下；会点韩语，虽然看韩剧和看韩站的感觉不一样，但看着基本无违和感，不懂的只靠google了，翻译得不地道反正将就着体会吧(有些请教了韩国设计师禹治大哥)；里面的说明侧重页面主要模块构成、交互和前端体验方面，另外真心赞韩国的网站视觉设计！那就开始吧，화이팅！在google中搜索 ‘쇼핑’，韩国主流购物网站都可以找到……

<table>
<tr><th>网站名称</th><th>浅析</th><th>网站简介</th><th>各终端</th></tr>
<tr><th>naver购物</th><td><a href="dist/naver.md">H5&PC</a></td><td>韩国第一大入口网站，在韩国搜索市场占据70%份额购物网站</td><td>pc版本支持宽窄屏的响应（990&1200），H5版本自适应,pc版本不支持触屏，移动端（含平板和手机）的推荐的h5版本,native版的主体内容直接嵌h5页面</td></tr>
<tr><th>daum购物</th><td><a href="dist/daum.md">H5&PC</a></td><td>韩国最大门户网站之一 life on daum 有基于搜索的购物频道</td><td>native版的主体内容直接嵌入h5页面，h5版响应得有特色</td></tr>
<tr><th>Gmarket</th><td><a href="dist/gmarket.md">H5&PC</a></td><td>韩国最大的综合购物网站，占网购份额的25%左右</td><td>native直接嵌h5页面,h5页面自适应宽度，pc版独立一个版本</td></tr>
<tr><th>basket 比价购物</th><td><a href="dist/basket.md">H5&PC</a></td><td>韩国专业比价购物网站</td><td>h5版自适应宽度，引入backbone view渲染view，router没用，非webapp，native版直接嵌h5版</td></tr>
<tr><th>emart mall</th><td><a href="dist/emartmall.md">H5&PC</a></td><td>专营食品和日用品，类似国内的1号店</td><td>h5版宽度自适应，类webapp但还是有差距，用cookie记录上一次的tab，汗！这个native也是嵌h5页面，设计得大气，能弥补点页面反应不流畅的问题:)</td></tr>
</table>

## 其他网站
<table>
<tr><th>名称</th><th>备注</th></tr>
<tr><th><a href="http://www.11st.co.kr/">11ST</a></th><td>C2C NO.3 (upgrade your life) 11号街(11st.co.kr)是韩国SK（韩国第三大跨国企业）电信开设的网上购物中心，提供种类丰富的产品，如服装、居家用品、电影音乐、数码手机、家电等等</td></tr>
<tr><td><a href="http://www.interpark.com/">interpark</a></td><td>B2C NO1</td></tr>
<tr><td><a href="http://www.gsshop.com/index.gs">GS SHOP</a></td><td>B2C NO3</td></tr>

<tr><th><a href="http://www.auction.co.kr/">auction옥션</a></th><td>Auction是韩国综合性购物网站,韩国历史上首家购物网站，已被Ebay收购</td></tr>
<tr><th><a href="http://www.cjmall.com/">CJ mall</a></th><td>B2C NO6 希杰集团（食品&饮食服务、家庭购物&物流、生物制药&基础设施、娱乐&媒体）旗下电商平台</td></tr>
<tr><th><a href="http://www.gsshop.com/index.gs">GS SHOP</a></th><td>PC首页支持宽窄屏响应</td></tr>
<tr><td><a href="http://www.nsmall.com/">NS홈쇼핑</a></td><td></td></tr>
<tr><td><a href="http://www.akmall.com/">AKmall</a></td><td></td></tr>
<tr><td><a href="http://mall.shinsegae.com/main/initMallMain.do">新世界商城</a></td><td>新世界百货 B2C NO.5 </td></tr>
<tr><td><a href="http://www.lotteimall.com/">乐天mall</a></td><td>乐天百货 B2C NO4</td></tr>
<tr><th><a href="http://www.coupang.com/">coupang</a></th><td>韩国团购网站(color your days!)</td></tr>
</table>

# 小评下 
韩国大部分的电商网站都是B2C，大多数不是韩国各大财阀的旗下的就是电视购物公司的，财阀的经营范围涉及到各个行业（食品、服饰、家居、家电、建筑、物流等）
甚至是娱乐界，如CJ集团旗下的CJ娱乐也会为电商网站服务，有专门的潮流明星导购频道；同时大部分线下都有百货公司（乐天百货、现代百货等），线上线下整合营销也是韩国财阀电商的一大特色。
如此多的电商网站，也造就了很多上游的比价导购网站，可见一淘还是有存在的必要性的。

在设计兴国的韩国，视觉上确实有自己的风格，个人感觉交互上整体一般，最多的就是switchable； 前端方面除了daum的shoping频道整站（从首页到srp）异步化有勇气；韩国电商网站除了naver用自己的类库，其他的网站用的都是jquery,在跨终端上面响应式和自适应都用得非常广泛，这块比国内要稍微前面一点；app方面全部是嵌h5页面，只维护一套，难道是成本原因而不care native的原生体验,明显没有我大阿里有资源:)，不过韩国网速快，也许能用就行吧。

所有网站的模块构成（今日特卖、best100、优惠券等固定模块）基本都差不多，也有本国的一些特有的交互（比如每个网站的左右2边全站都有fixe的内容区，放着购物车、收藏夹和浏览历史，naver后来把他演变成了固定的toolbar)，隐约感觉韩国电商会向日本借鉴（雷达图评价商品日本电商也有），也会向中国借鉴（detail页面交互太像了，也有可能是相互借鉴）；特别是在时尚美容时装的类目，活动页面都很华丽，营销氛围很浓厚。

# 可借鉴点
* <a href="dist/improve.md">可借鉴点</a>

# 各电商H5版首页一览
* <a href="dist/h5homepage.md">各电商H5版首页一览</a>

# 各电商H5版srp一览
* <a href="dist/h5srp.md">各电商H5版srp一览</a>

# 各电商H5版detail一览
* <a href="dist/h5detail.md">各电商H5版detail一览</a>

# 首页一览
* <a href="dist/homepage.md">首页一览</a>

# 各电商srp页一览
* <a href="dist/srp.md">各电商srp页一览</a>

# 各电商detail页一览
* <a href="dist/detail.md">各电商detail页一览</a>


# 一些好看的页面

* basket fashion soho 比较适合频道的模块
* http://fashion.basket.co.kr/html/soho/main/main.html
* http://fashion.basket.co.kr/html/soho/bestitem.html
* http://fashion.basket.co.kr/html/soho/main/submain03.html
* 图片墙主题集
* http://stylebook.basket.co.kr/sweb/main/mainKpopStylebook
* 最下面的模块
* http://www.fashionplus.co.kr/mall/default.asp
* style finder模块
* http://soho.auction.co.kr/sohoshop
* 图片不断闪，程序自动生成的不断变的jpg的图片？
* http://soho.auction.co.kr/sohoshop/SohoRanking.aspx
* 垂直家装频道，图片好看:)
* http://basket.dawonmall.com/
* http://basket.dawonmall.com/shop/?mtype=001002
* http://shopping.basket.co.kr/shoppingshop/socialShopping.do
* http://shopping.naver.com/plan/template.nhn?id=14215&nds=MjE0NzQ4MzY0NzE0MjE1


# 参考资料
* [韩国网上购物发展情况](http://blog.donews.com/veryls/archive/2009/07/08/1540643.aspx)
* 淘宝UED韩国行分享