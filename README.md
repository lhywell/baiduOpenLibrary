# baiduOpenLibrary

处理了百度开源库的BUG，并做了更新

-------------------
## 改进的百度地图功能

#### 库来源
http://lbsyun.baidu.com/index.php?title=jspopular/openlibrary


#### 区域限制

百度地图浏览区域限制类，对外开放。 允许开发者输入限定浏览的地图区域的Bounds值， 则地图浏览者只能在限定区域内浏览地图。

- 修复BUG：
1. 去掉setTimeout死循环

- 源文件:

[AreaRestriction.js](https://smartdata.b0.upaiyun.com/map/AreaRestriction.js)

[AreaRestriction.min.js](https://smartdata.b0.upaiyun.com/map/AreaRestriction.min.js)


#### 鼠标绘制工具条库
提供鼠标绘制点、线、面、多边形（矩形、圆）的编辑工具条的开源代码库。且用户可使用JavaScript API对应覆盖物（点、线、面等）类接口对其进行属性（如颜色、线宽等）设置、编辑（如开启线顶点编辑等）等功能。

- 新增功能点：
1. 增加多边形面积提示
2. overlaycomplete去掉面积提示

- 源文件:

[DrawingManager.js](https://smartdata.b0.upaiyun.com/map/DrawingManager.js)

[DrawingManager.min.js](https://smartdata.b0.upaiyun.com/map/DrawingManager.min.js)




## 案例
#### BaiduMap用canvas渲染万级POI点






## BaiduMap BUG

1. 地图坐标偏移

    浏览器类型、版本号：Microsoft Edge

    pc系统或手机型号：系统window10

    使用的接口／api:

    问题描述:鼠标点击地图出现位置偏差

- 复现链接：http://smartdata.b0.upaiyun.com/map/baiduMap.html

- 上报链接：http://bbs.lbsyun.baidu.com/forum.php?mod=viewthread&tid=137838

2. 引入限制区域开源库的问题

    浏览器类型、版本号：Chrome

    pc系统或手机型号：window10

    使用的接口／api:

    问题描述:引入限制区域开源库，AreaRestriction.js，拖动地图会出现这个问题，地图movestart，moveend事件不停的执行，不停的刷新header

- 复现链接：http://smartdata.b0.upaiyun.com/map/baiduMap-AreaRestriction.html

- 上报链接：http://bbs.lbsyun.baidu.com/forum.php?mod=viewthread&tid=138400&page=1#pid309255

![map](https://raw.githubusercontent.com/lhywell/baiduOpenLibrary/master/map.gif)