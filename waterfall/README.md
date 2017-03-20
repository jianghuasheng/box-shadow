# 用css样式实现瀑布流效果

> 主要是CSS3 中的多列columns属性的运用


## W3C中的columns 

- **浏览器支持**

> Internet Explorer 10 和 Opera 支持 column 属性。
> Firefox 支持替代的 -moz-column 属性。
> Safari 和 Chrome 支持替代的 -webkit-column 属性。

**注释：**Internet Explorer 9 以及更早版本的浏览器不支持 column 属性。

- **CSS3 创建多列**

column-count 属性规定元素应该被分隔的列数：

    div{
	//创建三列
    column-count:3;
    -moz-column-count:3; 	/* Firefox */
    -webkit-column-count:3; /* Safari 和 Chrome */
    }

- **CSS3 规定列之间的间隔**

column-gap 属性规定列之间的间隔：

    div{
	//规定列之间 40 像素的间隔：
    -moz-column-gap:40px;		/* Firefox */
    -webkit-column-gap:40px;	/* Safari 和 Chrome */
    column-gap:40px;
    }

- **CSS3 列规则**

column-rule 属性设置列之间的宽度、样式和颜色规则。

    div{
	//规定列之间的宽度、样式和颜色规则：
    -moz-column-rule:3px outset #ff0000;	/* Firefox */
    -webkit-column-rule:3px outset #ff0000;	/* Safari and Chrome */
    column-rule:3px outset #ff0000;
    }
- **新的多列属性**

<table style="border-collapse: collapse;border: 1px solid #aaa;">
<tbody><tr>
<th style="width:25%;">属性</th>
<th>描述</th>
<th style="width:5%;">CSS</th>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-count.asp" title="CSS3 column-count 属性">column-count</a></td>
<td>规定元素应该被分隔的列数。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-fill.asp" title="CSS3 column-fill 属性">column-fill</a></td>
<td>规定如何填充列。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-gap.asp" title="CSS3 column-gap 属性">column-gap</a></td>
<td>规定列之间的间隔。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-rule.asp" title="CSS3 column-rule 属性">column-rule</a></td>
<td>设置所有 column-rule-* 属性的简写属性。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-rule-color.asp" title="CSS3 column-rule-color 属性">column-rule-color</a></td>
<td>规定列之间规则的颜色。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-rule-style.asp" title="CSS3 column-rule-style 属性">column-rule-style</a></td>
<td>规定列之间规则的样式。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-rule-width.asp" title="CSS3 column-rule-width 属性">column-rule-width</a></td>
<td>规定列之间规则的宽度。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-span.asp" title="CSS3 column-span 属性">column-span</a></td>
<td>规定元素应该横跨的列数。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_column-width.asp" title="CSS3 column-width 属性">column-width</a></td>
<td>规定列的宽度。</td>
<td>3</td>
</tr>

<tr>
<td><a href="http://www.w3school.com.cn//cssref/pr_columns.asp" title="CSS3 columns 属性">columns</a></td>
<td>规定设置 column-width 和 column-count 的简写属性。</td>
<td>3</td>
</tr>
</tbody></table>

[点击查看在线案例](https://www.jianghuasheng.cn/example/waterfall.html)