# html 第一天 

## web标准

结构 HTML 表现 CSS 行为 JavaScript

## 标签关系

包含关系 并列关系

## 基本结构标签

HTML根标签

​	head头部标签

​		title 标题标签

​	body 主体内容

## 常用标签 

文本格式化

strong em del ins

div division 分割、分区 span 跨度、跨距

图像标签 <img src="图像URL" />

修改宽度或高度达到缩放效果

超链接

a anchor 锚

href 目标url地址

target 指定打开方式 _self  _blank

锚点链接 页面内快速跳转指定位置 href="#id" 

注释 <!--hehe-->

ctrl+/快速注释

特殊字符

```
&nbsp; 空格符
&lt; <小于号
&gt; >大于号
```

#  HTML 第二天

## 表格标签

 表格 展示数据

tr 行标签 td 单元格标签

th 表头单元格 居中加粗显示

align 对齐方式

thead tbody

rowspan 跨行合并 

colspan 跨列合并

cellpadding 边框与文字距离

cellspacing 单元格之间的空白

##  列表

布局页面

无序列表 有序列表 自定义列表

ul 无序列表 

li列表项目

ol 有序列表

自定义列表 

dl 定义描述列表

dt 定义项目名字

dd 描述每一个项目或名字

## 表单标签

收集用户信息

由表单域、表单控件（表单元素）、提示信息构成

表单域

form 用户信息的收集和传递给服务器

action url地址

method get/post 设置表单的提交方式

name 指定表单的名称

1、input输入表单元素

type属性 text、password、radio 单选按钮、checkbox 复选框、submit 将表单数据发送到服务器、reset 清除表单数据、submit 将表单数据发送到服务器、reset 清除表单数据button 可点击按钮、file 上传文件、label 标注标签 绑定表单元素，点击文本自动聚焦表单元素

```
<label for="sex">男</label>
<input type="radio" name="sex" id="sex" />
```

value提示元素的值即默认提示信息，主要供后台管理使用

checked设置默认属性

maxlength 输入字段最大长度

2、select 下拉表单元

```
<form>
<select>
	<option selected="selected">河南</option>
	<option>湖北</option>
</select>
</form>
```

3、textarea 文本域元素

多行文本内容输入 

# CSS 第一天

美化网页 布局页面

 CSS Cascading Style Sheets 层叠样式表 级联样式表 标记语言

HTML结构CSS样式

语法规范 选择器 声明样式

```
<head>
    <style>
        /* 选择器 */
        /* 给谁改样式{改什么样式} */
        p{
            color: red;
            font-size: 12px;
        }
    </style>
</head>
```

## 选择器

基础选择器、复合选择器

基础选择器：标签（p、div）、类（.class)、id（只能被调用一次）、通配符

字体属性

font-size

font-family

font-weight 400 700

font-style normal italic

字体复合属性

font: font-style font-weight font-size/line-height font-family;

必须保留size和family

文本属性

文本颜色 color

text-align left right center

装饰文本 text-decoraction none(删除链接下划线) underline(下划线)、overline(上划线)、line-through(删除线)

text-indent 文本缩进

```
text-indent: 20px
text-indent: 2em
```

em 当前元素相对单位

line-height 行高（上间距 字高 下间距）

##  CSS引入方式

1、行内样式表 行内式

放在标签内部

```
<p style="color: pink; font-size: 20px;"给我一个粉红的回忆</p>
```

2、内部样式表 嵌入式

放在style标签中

3、外部样式表 链接式

将CSS文件引入HTML页面中

```
link rel="stylesheet" href="style.css"
```

图片对齐需要设置父标签

# CSS 第二天

emmet语法

标签

```
div
div*3
ul>li
div+p
.demo
p.demo
p#demo
.demo$*5
div{ddd}
div{$}*5
```

样式

```
tac
ti
w100
h200
ti2
lh26
tdn
```

 快速格式化代码

shift+alt+F

复合选择器

基础选择器的组合

后代选择器（包含选择器）

选择父元素的后代元素

```
ol li {

}
```

子选择器

必须选择子元素

```
ol>li {

}
```

并集选择器

同时选择多组标签

```
div, 
p
```

语法规范 选择器竖写

伪类选择器

向某些选择器添加特殊效果，如链接等

```
:hover
```

链接伪类选择器

```
a:link 选择所有未访问连接
a:visited 选择所有已被访问的链接
a.hover 选择鼠标指针位于其上的链接
a.active 选择活动链接*（点击未松开）
```

LVHA love hate

focus伪类选择器

选取获得光标的表单元素

```
input:focus {
}
```

## 颜色显示模式

布局网页 显示方式

块元素 行内元素

块元素

div、h1-h6、p、ul、ol、li

独占一行

宽高内外边距可控

 文字类元素内不能使用块级元素

行内元素 内联元素

span、a、strong、b、em、i、del、s、ins、u等

一行显示多个

无法直接设置宽高

行内元素只能容纳文本元素或其他行内元素

链接内不能放链接 可以放块级元素

行内块元素

img、input、td

 元素显示模式转换

比如增加链接a触发范围

*转换为块元素：display:block;

转换为行内元素：display:inline;

*转换为行内块 display:inline-block;

单行文字垂直居中

文字行高等于盒子高度

## CSS背景

背景颜色

```
background-color: transparent; 透明的
```

背景图片

```
background-image: none|url(link);
```

背景平铺

```
background-repeat： repeat|no repeat|repeat-x|repeat-y;
```

背景图片的位置

```
background-position： x y;
```

length 百分数、由浮点数字和单位标识符组成的长度值

position top、center、bottom、left、right 方位名词

背景图像固定（背景附着）

scrol 背景图像随对象内容滚动

fixed 背景图像固定

```
background-attachment :scrol|fixed
```

背景复合写法

```
background: 背景颜色 背景图片地址 北京平铺 背景图像滚动 背景图片位置
```

背景色半透明

```
background: rgba(0, 0, 0, 0.5);
```

alpha透明度,取值在0~1之间，1为不透明，缩写为.5

# CSS第三天

## CSS三大特性

层叠性、继承性、优先级

层叠性 

样式冲突 就近原则

继承性

子标签会继承父标签的某些样式，文本颜色和字号等

行高的继承性

```
font: 12px/1.5 当前元素文字大小的1.5倍
```

优先级

选择器相同，就近原则

选择器不同，按权重执行

继承<元素选择器<类选择器、伪类选择器>ID选择器>行内样式>！important

## 盒子模型

边框，内外边距，内容

边框 

border-weight粗细 

style样式 solid实线边框 dashed 虚线边框 dotted点线边框

color颜色

边框简写

```
border: 1px soild red; 没有顺序
```

边框分开写法

```
border-top: 5px soild red; bottom left right 
```

表格的细线边框

```
border-collapse: collapse 合并相邻边框
```

盒子本身指定宽度高度后，边框会影响盒子的实际大小

内边距padding

外边距margin

盒子水平居中 左右外边距设置为auto

```
margin: 0 auto;
```

相邻块元素垂直外边距合并

嵌套块元素垂直外边距的塌陷

为父元素添加

```
overflow:hidden；
```

清除内外边距

```
* {
padding: 0; 清除内边距
margin: 0; 清除外边距
}

```

行内元素尽量只设置左右内外边距，不要设置上下

# CSS第四天

### 圆角边框

设置元素的外边框圆角

```
border-radius:length;
```

参数值可以为数值或百分比

### 盒子阴影

```
box-shadow: h-shadow v-shadow blur spread color inset;
```

水平阴影、垂直阴影

或模糊距离、阴影尺寸、阴影颜色、外部阴影outset改为内部阴影

文字阴影

```
text-shadow: h-shadow v-shadow blur color;
```

## CSS浮动

### 浮动

传统网页布局的三种方式：标准流、浮动、定位

标准流

标签按照规定的默认方式排列

网页布局第一准则：多个块级元素纵向排列找标准流，多个块级元素横向排列找浮动

```
选择器 {
	float: 属性值;
	}
```

none, 默认值元素不浮动；left，元素向左浮动；right，元素向右浮动

浮动特性

网页布局第二准则：先设置盒子大小，再设置盒子位置

常见网页布局

top

banner

main | 浮动 left right

footer

 浮动布局注意点

浮动和标准流的父盒子搭配

一个元素浮动了，理论上其余兄弟元素也要浮动

浮动元素只会影响后边的标准流

清除浮动的本质就是清除浮动元素造成的影响

```
选择器 {
clear: 属性值;
}
```

left、right、both不允许左、右、两侧有浮动

clear: both最常用

清除浮动的策略是闭合浮动

清除浮动的方法

1、额外标签法、隔墙法

```
<div style="clear:both"></div>
```

2、父级元素添加overflow属性

```
overflow: hidden;
```

hidden、auto、scroll 溢出隐藏

3、父级元素添加after伪元素

```
.clearfix:after {  
   content: ""; 
   display: block; 
   height: 0; 
   clear: both; 
   visibility: hidden;  
 } 
 .clearfix {  /* IE6、7 专有 */ 
   *zoom: 1;
 } 
```

4、父级添加双伪元素

```
 .clearfix:before,.clearfix:after {
   content:"";
   display:table; 
 }
 .clearfix:after {
   clear:both;
 }
 .clearfix {
    *zoom:1;
 }  
```



# CSS第五天

PS切图 

cutterman

学成在线案例

CSS属性书写顺序

1、布局定位属性

display、position、float、clear、visibility、overflow（建议display第一个写）

2、自身属性

width、height、margin、padding、border、background

3、文本属性

color、font、text-decoration、text-align、vertical-align、white-space、break-word

4、其他属性（CSS3）

content、cursor、border-radius、box-shadow、background:linear-gradient

 页面布局整体思路

1、确定页面的版心，即可视区域

2、分析页面中的行模块和每个行模块中的列模块。第一准则

3、一行中的列模块经常浮动布局，先确定每个列的大小，之后确定列的位置。 第二准则

4、制作HTML结构。先有结构，后有样式。

实际开发中，我们不会直接用链接a而是用li包含(li+a)的做法。

浮动的盒子不会有外边距合并的问题

# CSS第六天

## 定位

### 定位组成

定位模式 定位方式 

static 静态定位 relative 相对定位 

absolute  绝对定位 fixed 固定定位

边迁移 元素的最终位置

top bottom left right

1、静态定位 static

默认定位方式 无定位

```

选择器 { position static； }
```

按照标准流摆放位置，没有边偏移，很少用到

2、相对定位 relative

相对原来位置 

```
选择器 { position：relative；}
```

原来在标准流的位置继续占有，后续盒子仍然以标准流对待他。

3、绝对定位 absolute

相对于祖先元素来说

```
选择器 { position：absolute；}
```

如果没有祖先元素或祖先元素没有定位，则是以浏览器为准定位

如果祖先元素有定位，则以最近一级有定位祖先元素为参考点移动位置

绝对定位脱离标准流，不再占据原先的位置

子绝父相

父亲需要保留位置，子盒子不需要

4、固定定位 fixed

固定于浏览器的可视位置，页面滚动元素不会改变

以浏览器的可视窗口为参照点移动元素

固定定位不占有原先的位置

固定在版心右侧：left 50% margin left版心的一半

粘性定位 sticky

相对定位和固定定位的混合

以浏览器的可视窗口为参照点移动元素

占有原来位置

兼容性差，不支持IE

### 定位叠放次序 z-index

控制盒子的z轴

属性值相同按书写顺序后来居上

只有定位的盒子有这个属性

### 定位的拓展

绝对定位的盒子居中

定位的特殊性

1、行内元素添加绝对或者固定定位，可以直接设置宽度和高度

2、块级元素添加绝对或者固定定位，可以不给宽度或者高度，默认大小是内容的大小。

3、脱标的盒子不会触发外边距塌陷

浮动元素、绝对定位、固定定位元素都不会触发外边距合并问题

4、绝对定位、固定定位会完全压住盒子

浮动元素不同，会压住标准流的盒子，但是不会压住里面的图片或文字（最初的目的是为了文字环绕） 

绝对定位和固定定位会压住盒子和里面的内容。

### 淘宝焦点图布局

如果一个和盒子既有right和left属性、top和bottom属性，会执行left和top属性

1、标准流 

可以让盒子上下排列或者左右排列，垂直的块级盒子显示就用标准流布局。

2、浮动

可以让多个块级元素一行显示或者左右对齐盒子，多个块级盒子显示就用浮动布局。

3、定位

定位最大的特点是有层叠的概念，就是让多个盒子前后叠加来显示。如果元素自由在某个盒子内移动就用定位布局。

## 元素的显示和隐藏

在页面中隐藏元素

1、display 显示隐藏

```
dislay: none;隐藏对象并且不占有原来的位置
display: block;除了转换为块级元素之外，同时还有显示元素的意思
```

2、visibility 可见性

```
visibility: visible; 元素可视
visibility: hidden; 元素隐藏，继续占有原先位置
```

3、overflow 溢出

指定内容溢出元素框的显示方式

```
visible 不剪切内容也不添加滚动条
hidden 不显示超过对象尺寸的内容，超出的部分隐藏掉
scroll 不管超出内容否，总是显示滚动条
auto 根据内容智能显示滚动条
```

有定位的盒子慎用hidden

# CSS第七天

## css高级技巧

### css三角

```
div {
	width: 0;
	height: 0;
	line-height: 0;
	font-size: 0;
	border: 50px solid transparent;
	boder-left-color: pink;
}
```

### css用户界面样式

1、鼠标样式 cursor

```
li {cursor: pointer; }
```

设置或检索在对象上移动的鼠标指针采用何种系统预定义的光标形状

default 小白 默认

pointer 小手

move 移动

text 文本

not-allowed 禁止

2、轮廓线 outline

```
input {
	outline：none；/或0
	}
```

3、防止拖拽文本域 resize

```
textarea {
	resize； none；
}
```

3、vertical-align 属性应用

对齐方式 设置图片或者表单（行内块元素）和文字垂直对齐

```
baseline 默认 元素放置在父元素的基线上
top 元素的顶端与行中最高元素的顶端对齐
middle 元素放置在父元素的中部
bottom 将元素顶端与行中最低元素的的顶端对齐
```

解决图片底部留白问题

更改基线对齐方式

更改为块级元素

4、溢出的文字省略号显示

单行文本

```
1、先强制一行内显示文本
white-space：nowrap；（默认normal自动换行）
2、超出的部分隐藏
overflow：hidden；
3、文字用省略号代替超出的部分
text-overflow：ellipsis；
```

多行文本

兼容问题 适用于webkit浏览器

```
over-flow： hidden；
text-overflow：ellipsis；
弹性伸缩盒子模型显示
display：-webkit-box；
限制在一个块元素显示的文本的行数
-webkit-line-clamp：2；
设置或检索伸缩盒对象的子元素的排列方式
-webkit-box-orient：vertical；
```

更推荐让后台人员来做这个效果，后台人员可以设置显示字数

## 常见的布局技巧

1、margin负值的运用

解决外边距合并

```
ul li {
	float: left;
	list-style: none;
	width: 150px;
	height: 200px;
	border: 1px solid red;
	margin-left: -1px;
}
```

鼠标经过边框变色

```
1、如果盒子没有定位，则鼠标经过添加相对定位即可
ul li hover {
	position: relative;
	border: 1px soild blue;
}
2、如果li都有定位，则利用z-index提高层级
ul li:hover {
	z-index: 1;
	border: 1px soild blue;
}
```

2、文字围绕浮动元素

浮动元素不会压住文字

3、行内块元素巧妙运用

底部网页跳转导航栏

4、CSS三角强化

```
width: 0;
height: 0;
border-color: transparent red transparent transparent;
border-style: soild;
border-width: 22px 8px 0 0;
```

## CSS初始化

重设浏览器样式

# CSS第八天

H5C3

