---
title: Css3实现背景毛玻璃效果
date: 2018-03-06 14:57:46
tags:
- 小程序
- css3
categories:
- CSS3
banner: https://app.yinxiang.com/shard/s72/res/3f70954e-30e0-4b67-b182-dd2acd6d5fc9
---



##### 先上代码
```html

<div class="father">
	<img src="your bacImage address"/>
	<div class="mask"></div>
</div>


```
<!-- more -->



```css
.father{
	width:100%;
	height: 270px;
	display:flex;


}
.father img{
	width:100%;
	height:100%;
    -webkit-filter: blur(2px) ;  //css3 滤镜属性  
}


//给图片加黑色背景蒙层
.mask{
  width:100%;
  position: absolute;
  background-color: red;
  height: 270px;
  z-index: 10;
  background: #132445;
  opacity: 0.6;
}
```

##### 效果图

![效果图](https://app.yinxiang.com/shard/s72/res/3f70954e-30e0-4b67-b182-dd2acd6d5fc9)



#### 主要实现  ：

使用到了 css ` filter`(滤镜) 属性

#### 具体请看 [CSS filter属性  文档](https://developer.mozilla.org/zh-CN/docs/Web/CSS/filter)
