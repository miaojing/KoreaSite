# 一些可借鉴点

1. native和h5之间的连接
	
![http://m.naver.com/](img/naverh5index3.png) 

	<a class="btn_sch btn_cod" data-tiara-area-code="code_lmode" href="http://search.daum.net/search?w=tot&q=%EB%8B%A4%EC%9D%8C%EC%95%B1" data-store-url="itms-apps://itunes.apple.com/us/app/da-eum-daum/id365494029"><span class="img_sg ico_cod">코드검색</span></a>

ios:
	<a class="btn_sch btn_cod" data-tiara-area-code="code_lmode" href="daumapps://codeSearch?" data-store-url="itms-apps://itunes.apple.com/us/app/da-eum-daum/id365494029"><span class="img_sg ico_cod">코드검색</span></a>

android:
	<a class="btn_sch btn_search" data-tiara-area-code="voice_lmode" href="intent://voiceSearch?type=total#Intent;scheme=daumapps;action=android.intent.action.VIEW;category=android.intent.category.BROWSABLE;package=net.daum.android.daum;end" data-store-url="itms-apps://itunes.apple.com/us/app/da-eum-daum/id365494029"><span class="img_sg ico_vic">음성검색</span></a>


2. h5和pc的连接

页面下方和各个终端的连接，并且除了客户端所有的链接都是随所在页面位置变化的
pc版/简易版/客户端/
如下： http://m.basket.co.kr/mobile/contents/shopping/prodDisp/?svcCd=01&coDataVenNo=1&coPrdMstNo=B20392707&keyword=%EC%8A%A4%EC%BB%A4%ED%8A%B8

3. 雷达图的方式分析商品的各个方面还不错
![http://m.naver.com/](img/basketpcdetail3.png) 

4. 首页焦点图轮播不是一帧一帧，而是一组一组，或者整个类目切换，增加广告收入？
![http://www.gmarket.co.kr/](img/gmarketpcindex1.png) 
![http://www.gmarket.co.kr/](img/gmarketpcindex3.png) 
[auction也是](http://www.auction.co.kr/?redirect=1)
[乐天首页的轮播图也不错](http://www.lotteimall.com/main/viewMain.lotte?dpml_no=1)

5. 是否应该iframe第三方网站，曾经etao也不想跳到第三方网站，期望可以搞个etao的标准头然后iframe嵌入各个网站
当时反对的原因：强制加上去太山寨，在iframe内部影响页面内部跳转和某些功能，第三方网站是可以防止被iframe的
可是[daum](http://shopping.daum.net/go.daum?pkey=8Pzo0TM1ytl8FlUoupJAmZj6egLH.s7U3DTr.9ERec_s5LC46KQ.DfyiOVCHL324UGeqnEPn8z-pst6zcLXaE1.RCqAgX5DGhaitjpcC25T5EUjSPc7YbpdhQV_9vdbdhZmWXfaifh6O8-8uLxXvUXg-jdg00&val=FKA00_zKVYha5tlhVCi9d1S6TsvdXxha-kJIP9GfsOk12jIP3C-KxP8e-OLLBQFnFN27WlaZkvCqD-V6OWvZ_ePQAC2k-Brgl.PYcFx5tQ69eKNPCH5jJQxPSuw00&search=OBL58v2oJJHglUrGnvXtXainQHkJt4dyt82Dwk-6KMHfwijQcUuScWJbOOTKtdtpLBLOo6TyggXZk9xTVqBHrKBM6BTw.alh339Q1t_.NC.TB-OTPVHdZe_D9ybs9-jpaB9Ct)加了：
[basket]也加了，daum是直接iframe第三方网站，而basket是和所有第三方网站合作，提供了一个basket的header通过cookie标记是否加basket头部，可以看得出来basket和第三方网站的合作都是深度合作。

6. [详情页太长，加个锚点分段定位](http://www.interpark.com/product/MallDisplay.do?_method=detail&sc.shopNo=0000100000&sc.dispNo=001206&evtNo=130084&sc.prdNo=1767882770)

7. [srp左右翻页](http://www.ellotte.com/search/search.total.ldpm?currentPage=1&rowSperpage=30&searchTermAll=%EC%BF%A0%EC%95%84%EC%B9%98%EB%A7%88&searchTermPre=&searchTermExc=&searchTermOri=%EC%BF%A0%EC%95%84%EC%B9%98%EB%A7%88&orderType=1&brandAll=&colorAll=&mCat=&lCat=S01A05&sprice=&eprice=&holdKwd=y&_cloc=&searchTerm=%EC%BF%A0%EC%95%84%EC%B9%98%EB%A7%88#price_color_tit)
