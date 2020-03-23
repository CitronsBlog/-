# 仿百度首页

只有多敲才能多学

这是一个练习布局思路的小项目

## 仿站截图

![截图](https://s1.ax1x.com/2020/03/24/8bSryq.png)

主要踩了背景图的坑

怎么让图片铺满全屏且不让他随窗口的变化而变化？
我用的是background-image
我的解决办法：
给父元素也就是html和body设置宽高都为100%
然后给body的样式如下：
```
   position:absolute;
    background: url('/img/885.jpg') no-repeat 0 0/100%;
    top:0;
    left: 0;
    background-position: center 0;
    background-repeat: no-repeat;
    background-attachment:fixed;
    background-size: cover;
    -webkit-background-size: cover;/* 兼容Webkit内核浏览器如Chrome和Safari */
    -o-background-size: cover;/* 兼容Opera */
   zoom: 1;   

```
仅供参考