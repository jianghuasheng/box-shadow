# box-shadow
css3 box-shadow 阴影案例
<!DOCTYPE html>  
<html>  
  
<head>  
<meta content="text/html; charset=utf-8" http-equiv="Content-Type">  
<title>CSS3属性：box-shadow测试</title>  
<style type="text/css">  
/* 
    -moz-box-shadow:投影方式 X轴偏移量 Y轴偏移量阴影模糊半径 阴影扩展半径 阴影颜色;  
    -webkit-box-shadow:投影方式 X轴偏移量 Y轴偏移量阴影模糊半径 阴影扩展半径 阴影颜色;   
    box-shadow:  投影方式 X轴偏移量 Y轴偏移量 阴影模糊半径 阴影扩展半径 阴影颜色;  

*/
.box-shadow-1{  
  -webkit-box-shadow: 3px 3px 3px;  
  -moz-box-shadow: 3px 3px 3px;  
  box-shadow: 3px 3px 3px;  
}  
.box-shadow-2{  
  -webkit-box-shadow:0 0 10px #0CC;  
  -moz-box-shadow:0 0 10px #0CC;  
  box-shadow:0 0 10px #0CC;  
}  
.box-shadow-3{  
  -webkit-box-shadow:0 0 10px rgba(0, 204, 204, .5);  
  -moz-box-shadow:0 0 10px rgba(0, 204, 204, .5);  
  box-shadow:0 0 10px rgba(0, 204, 204, .5);  
}  
.box-shadow-4{  
  -webkit-box-shadow:0 0 10px 15px #0CC;  
  -moz-box-shadow:0 0 10px 15px #0CC;  
  box-shadow:0 0 10px 15px #0CC;  
}  
.box-shadow-5{  
  -webkit-box-shadow:inset 0 0 10px #0CC;  
  -moz-box-shadow:inset 0 0 10px #0CC;  
  box-shadow:inset 0 0 10px #0CC;  
}  
.box-shadow-6{  
    box-shadow:-10px 0 10px red, /*左边阴影*/  
    10px 0 10px yellow, /*右边阴影*/  
    0 -10px 10px blue, /*顶部阴影*/  
    0 10px 10px green; /*底边阴影*/  
}  
.box-shadow-7{  
    box-shadow:0 0 10px 5px black,  
    0 0 10px 20px red;  
}  
.box-shadow-8{  
    box-shadow:0 0 10px 20px red,  
    0 0 10px 5px black;  
}  
.box-shadow-9{  
    box-shadow: 0 0 0 1px red;  
}  
  
  
  
.obj{  
    width:100px;  
    height:100px;  
    margin:50px auto;  
    background:#eee;      
}  
.outer{  
    width: 100px;  
    height: 100px;  
    border: 1px solid red;  
}  
.inner{  
    width: 60px;  
    height: 60px;  
    background-color: red;  
    -webkit-box-shadow: 50px 50px blue;  
    -moz-box-shadow: 50px 50px blue;  
    box-shadow: 50px 50px blue;  
  }  
</style>  
</head>  
  
<body>  
    <div class="obj box-shadow-1"></div>  
    <div class="outer">  
        <div class="inner"></div>  
    </div>  
    <div class="obj  box-shadow-2" ></div>  
    <div class="obj  box-shadow-3" ></div>  
    <div class="obj  box-shadow-4" ></div>  
    <div class="obj  box-shadow-5" ></div>  
    <div class="obj  box-shadow-6" ></div>  
    <div class="obj  box-shadow-7" ></div>  
    <div class="obj  box-shadow-8" ></div>  
    <div class="obj  box-shadow-9" ></div>  
    <script type="text/javascript">  
        $(document).ready(function(){  
        if($.browser.msie) {  
          $('.obj').boxShadow(-10,-10,5,"#0cc"); //obj元素使用了box-shadow  
        }  
      });  
    </script>  
  
</body>  
</html>  
