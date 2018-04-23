# baiduOpenLibrary
====================

处理了百度开源库的BUG，并做了更新

-------------------
## 来源
http://lbsyun.baidu.com/index.php?title=jspopular/openlibrary


#### 区域限制

百度地图浏览区域限制类，对外开放。 允许开发者输入限定浏览的地图区域的Bounds值， 则地图浏览者只能在限定区域内浏览地图。

修复BUG：
1. 去掉setTimeout死循环

[AreaRestriction.js](https://smartdata.b0.upaiyun.com/map/AreaRestriction.js)

[AreaRestriction.min.js](https://smartdata.b0.upaiyun.com/map/AreaRestriction.min.js)


#### 鼠标绘制工具条库
提供鼠标绘制点、线、面、多边形（矩形、圆）的编辑工具条的开源代码库。且用户可使用JavaScript API对应覆盖物（点、线、面等）类接口对其进行属性（如颜色、线宽等）设置、编辑（如开启线顶点编辑等）等功能。

新增功能点：
1. 增加多边形面积提示
2. overlaycomplete去掉面积提示

[DrawingManager.js](https://smartdata.b0.upaiyun.com/map/DrawingManager.js)

[DrawingManager.min.js](https://smartdata.b0.upaiyun.com/map/DrawingManager.min.js)