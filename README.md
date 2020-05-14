# 爬取

去哪儿网-
景点名称, 地址, 评论,评论的图片

```
一级页面, 每个页面有10条景点, 假设爬取50页
北京旅游景点列表 https://travel.qunar.com/p-cs299914-beijing-jingdian
------------------------------------------------------------------------------

 每次保存
//划掉QAQ 经纬度(不保存白不保存 万一有用呢) : <li class="item" data-lat="39.502139" data-lng="116.340954">
 景点名称: 如"故宫"; <span class="cn_tit">故宫<span class="en_tit">Forbidden City</span></span>
 景点简介: 世界....; <div class="desbox">世界五大宫之首，是中国明清两代的皇家宫殿。</div>
 评论链接 点击进入 <a data-beacon="poi" href="https://travel.qunar.com/p-oi710603-gugong"  alt="故宫"
------------------------------------------------------------------------------

 二级页面, 每个页面有10条评论, 每次要点击进入下一页, 如果没有 next, 则表示爬取完毕
 下一页 <a class="page next"  href="https://travel.qunar.com/p-oi710603-gugong-1-2?rank=0#lydp">下一页</a>
 用户ID <li class="e_comment_item clrfix" id="cmt_item_10158224437">
 用户评论 <p class="first">我和同学是10月1号去的，因为人太多，</p>
```
