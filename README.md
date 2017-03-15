# 常用的css3案例
-----------------------------------
基础说明：
    外阴影：box-shadow: X轴  Y轴  Rpx  color;

    属性说明（顺序依次对应）： 阴影的X轴(可以使用负值)    阴影的Y轴(可以使用负值)    阴影模糊值（大小）    阴影的颜色

    内阴影：box-shadow: X轴  Y轴  Rpx  color  inset;

       默认是外阴影   内阴影：inset 可以设置成内部阴影

    注（PS）：此属性使用于盒模型 如(div,p,h1,h2,h3,h4,h5,h6等) 不是用来设置文字阴影   如果设置文字阴影请参考知识点:text-shadow（同理）

     因为是新属性，为了兼容各主流浏览器并支持这些主浏览器的较低版本，基于主流浏览器上使用box-shadow属性时，我们需要将属性的名称写成-webkit-box-shadow的形式。Firefox浏览器则需要写成-moz-box-shadow的形式

                        欧朋浏览器  -o-box-shadow   IE>9  -ms-box-shadow    

基础练习：
为了更好的了解box-shadow的特征，做几个小测试：(为了方便直接在标签内嵌套样式)

 测试1： <div style="box-shadow: 0 0 10px #f00; border:1px solid green"></div>  box-shadow: 0 0 10px #f00  （因没有使其X轴与Y轴移动 设置值 所在会在本身发生作用   半径范围，颜色）

 



 测试2： <div style="box-shadow:4px 4px 10px #f00; border:1px solid green"></div> box-shadow:4px 4px 10px #f00;与测试1不同 X轴与Y轴改变了正值（正值 向右 向下） 所以变成了这样‍

 

   

测试3：<div style="box-shadow:-4px -4px 10px #f00; border:1px solid green"></div> box-shadow:-4px -4px 10px #f00;与测试2不同 之处是 X轴与Y轴改变成了负值（负值 向左 向上） 所以变成了这样‍

     

同理：你可以测试下一正值，一负值的效果，这里就不做测试了。。。。。。。。

测试4：<div  style="box-shadow:-10px 0px 10px red,   /*左边阴影*/ 
                                                   0px -10px 10px #000,  /*上边阴影*/ 
                                                   10px 0px 10px green,  /*右边阴影*/ 
                                                   0px 10px 10px blue;" /*下边阴影*/ ></div>

你看到这样的代码会感觉很乱 但是看到效果图片之后你就能明白这是怎么做的了无非改一下X轴与Y轴位置与颜色值 还有阴影值大小，（用逗号隔开）多练习几次就好



 

测试5：--内阴影  <div style="box-shadow: 0px 0px 10px red inset; border:1px solid green"></div> box-shadow: 0px 0px 10px red inset;    与上面写法相同 唯一不同的是添加了一个inset 其它属性与外阴影相同

   