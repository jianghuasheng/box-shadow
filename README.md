# 常用的css3案例
-----------------------------------
##1、box-shadow
**外阴影**：box-shadow: X轴  Y轴  Rpx  color;

**属性说明**（顺序依次对应）：阴影的X轴(可以使用负值) 阴影的Y轴(可以使用负值)  阴影模糊值（大小）阴影的颜色

**内阴影**：box-shadow: X轴  Y轴  Rpx  color  inset;

*默认是外阴影   内阴影：inset 可以设置成内部阴影*

注（PS）：此属性使用于盒模型 如(div,p,h1,h2,h3,h4,h5,h6等) 不是用来设置文字阴影   如果设置文字阴影请参考知识点:text-shadow（同理）

因为是新属性，为了兼容各主流浏览器并支持这些主浏览器的较低版本，基于主流浏览器上使用box-shadow属性时，我们需要将属性的名称写成-webkit-box-shadow的形式。Firefox浏览器则需要写成-moz-box-shadow的形式

    -moz-box-shadow:投影方式 X轴偏移量 Y轴偏移量阴影模糊半径 阴影扩展半径 阴影颜色;
    -webkit-box-shadow:投影方式 X轴偏移量 Y轴偏移量阴影模糊半径 阴影扩展半径 阴影颜色;   
    -box-shadow:  投影方式 X轴偏移量 Y轴偏移量 阴影模糊半径 阴影扩展半径 阴影颜色; 

----------------------
[点击查看相关例子](http://www.cnblogs.com/wuchuanlong/p/5980766.html)

 

