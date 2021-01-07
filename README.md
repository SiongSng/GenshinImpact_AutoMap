# GenshinImpact_AutoMap
原神自动地图，基于原神小地图的自动标记资源地图

目前做成了原神的PC端悬浮窗地图工具……

## 运行画面

![运行画面](https://github.com/GengGode/GenshinImpact_AutoMap/blob/master/GenshinImpact_Map_Test_1/Img/Snipaste_2021-01-07_15-09-00.png)

## 目前实现

地图显示（平移、缩放）

检测游戏状态（游戏全屏下会失效）

可以添加标记（代码里）

## 计划实现

通过游戏内小地图，自动识别角色所在位置，根据数据库显示周围资源分布

在某些情况下自动隐藏悬浮窗，如传送时，打开大地图时，释放大招时……

优化UI

## 更远的计划

利用MFC或者Qt重写一个窗口，不再使用OpenCV提供的窗口，以便实现不规则窗口和边缘半透明效果

根据另一个做的小地图自动识别来看，还优化自动识别的速度

## 一些已知的问题

游戏全屏时，因为悬浮窗处于置顶状态，悬浮窗和原神会争抢顶层窗口的位置，以至于游戏来回全屏和最小化。

推测可能是原神的问题，在双屏幕时全屏原神，在另一个屏幕上鼠标点击，原神就会最小化，然而B服原神不会。