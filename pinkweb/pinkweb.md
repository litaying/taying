# HTML 第一天 

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

## HTML5

新的标签、表单和表单属性，需要IE9+

1、新增的语义化标签

```
header 头部标签
nav 导航标签
article 内容标签
section 定义文档某个区域
aside 侧边栏标签
footer 尾部标签
```

2、多媒体标签

音频audio、视频video

```
<video src="文件地址" controls="controls"></video>
```

```
autoplay autoplay 视频自动播放（谷歌浏览器需要添加muted解决）
controls controls 向用户显示播放控件
width pixels（像素） 设置播放器宽度
height pixels（像素） 设置播放器高度
loop loop 是否循环播放
preload auto/none 是否预加载视频，设置autoplay后忽略该属性
src url 视频url地址
poster imgurl 等待加载的画面图片
muted muted 静音播放
```

```
<audio src="文件地址" controls="controls"></audio>
```

```
autoplay
controls
loop
src
```

3、新增input表单类型

```
type="email" 限制用户输入必须为Email类型
url 
date
time
month
week
number
tel
search
color
```

 number tel search

4、新增的表单属性

```
required required 内容不能为空
placeholder 提示文本 表单的提示信息
autofocus autofocus 自动聚焦属性
autocomplete off/on 默认打开 显示历史成功输入记录
multiple multiple 可以多选文件提交
```

placeholder、multiple

## CSS3

1、新增选择器

属性选择器、结构伪类选择器、 伪元素选择器

属性选择器

```
1、属性选择器可以不借助类或者ID选择器
input[value] {
	选中带有value值的input表单
}
*2、选择属性=值的某些元素
input[type="text"] {
	选中type值为text的input表单
}
3、选择属性值开头的某些元素
div[class^="icon"] {
	div具有class属性，属性值为icon开头的元素
}
4、选择属性值结尾的某些元素
section[class$="data"] {
	section具有class属性，属性值为data结尾的元素
}
5、选择属性值中含有val的元素
section[class*="val"] {
	section具有class属性，包含属性值为val的元素
}
```

类选择器、属性选择器、伪类选择器，权重为10

结构伪类选择器

根据文档结构选择，常用于根据父级选择器选择里边的子元素

```
E:first-child 匹配父元素中的第一个子元素E
E:last-child 匹配父元素中最后一个E元素
E:nth-child(n) 匹配父元素中的第n个子元素E
n可以是
数字（从1开始）、
关键字（even偶数、odd奇数）、
公式（n从零开始，2n即偶数孩子、2n+1即奇数、5n、n+5即第5和以后所有元素、-n+5即前5个）
E:first-of-type 指定类型E的第一个
E:last-of-type 指定类型E的最后一个
E:nth-of-type(n) 指定类型E的第n个
```

```
1、子元素 先排序再判断元素类型
ul li:first-child {
	选择ul的第一个孩子li
}
ul li:first-child(n) {
	选择ul的n个孩子li
}
2、指定类型元素 先判断类型排序
ul li:first-of-type {
	选择ul的第一个li类型
}
ul li:first-of-type(n) {
	选择ul的n个孩子li
}
权重
```

​	*伪元素选择器

利用CSS创建新标签，简化HTML结构

```
::before 在元素内部的前面插入内容
::after 在元素内部的后面插入内容
```

element::before/after

必须具有content属性 

行内元素

伪元素选择器和标签选择器一样，权重为1

伪元素使用场景1伪元素字体图标

```
p::before {
	position: absolute;
	right: 20px;
	top: 10px
	content: '\e91e';
	font-size: 20px
}
```

伪元素使用场景2伪土豆效果

```
.tudou:hover::before {
}
```

伪元素使用场景3伪元素清除浮动

```
.clearfix:before,.clearfix:after {
	content:'';
	display:table;
}
.clearfix:after {
	clear:both;
}
```

## CSS3盒子模型

border-sizing: content-box 盒子大小为width+padding+border（默认属性）

box-sizing: border-box 盒子大小为width  //padding和border不超过width就不会撑大盒子

```
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
```

## CSS3其它特性

1、图片变模糊

CSS3滤镜filter：

filter CSS属性将模糊或颜色偏移等图形效果应用于元素

```
filter: 函数(); 例如：filter:blur(5px) blur模糊处理 数字化越大越模糊
```

2、计算盒子宽度width：calc函数

calculate

```
width: calc(100%-80px);
```

括号里可以使用+-*/来进行计算

## *CSS3过渡

过渡动画，从一个状态渐渐的过渡到另一个状态

```
transition：要过渡的属性 花费时间 运动曲线 何时开始；
1、属性：想要变化的css属性，宽度高度 背景颜色 内外边距 想要所有的属性都变化过渡用all
2、花费时间：单位是秒（必须写单位）比如0.5s
3、运动曲线：默认是ease（可以省略）
4、何时开始：单位是秒（必须写单位）可以设置延迟触发时间 默认是0s（可以省略）
```

多个属性利用逗号进行分割

### 进度条案例

进度条如何布局

进度条过渡

## 狭义的HTML5 CSS3

HTML5 结构标签本身

CSS3 相关样式

## 广义的H5

HTML5 CSS3 javascript

# PC端品优购项目

favicon.ico 缩略的网站标志 显示在浏览器的地址栏或者标签上

## 网站TDK三大标签SEO优化

Search Engine Optimization 搜索引擎优化

title description keyword 

LOGO优化

1、h1标签提权

2、放一个可以返回首页的链接

3、链接里面放网站名称，但是文字不要显示

- 方法1：text-indent移到盒子外面（text-indent: -9999px), 然后overflow:hidden，淘宝的做法
- 方法2：直接给font-size: 0; 就看不见文字了，京东的做法

4、给链接一个title属性，鼠标放到logo上可以看到提示文字

# H5C3再提升

## 4、2D转换

转换可以实现元素的位移、旋转和缩放

transform 变形

- 移动 translate
- 旋转 rotate
- 缩放 scale

### transform 移动

```
transform: translate(100px,100px);
transform: translate(100px,0);
transform: translateX(100px);
transform: translateY(100px);
```

不会影响其他盒子的位置

translate中的百分比单位是相对于自身元素的 translate:(50%,50%);

对行内标签没有效果

### rotate 旋转

```
transform: rotate(度数)

	/* Rotate div */
	transform:rotate(90deg);
	-ms-transform:rotate(90deg); /* IE 9 */
	-webkit-transform:rotate(90deg); /* Safari and Chrome */

```

rotate里面跟度数， 单位是 deg 比如 rotate(45deg)

角度为正时，顺时针，负时，为逆时针

默认旋转的中心点是元素的中心点

### 2D转换中心点 transform-orgin

```
transform-origin: x y;
```

- 注意后面的参数用空格隔开
- 默认值是元素的中心点(50% 50%)
- 可以给x y设置像素或者方位名词 top bottom left right center

### scale 缩放

```
transform:scale(x,y);
```

x  y为宽 高 倍数

sacle缩放最大的优势：可以设置转换中心点缩放，默认以中心点缩放的，而且不影响其他盒子

### 2D转换综合写法

transform: tranlate() rotate() scale()

顺序会影响效果

### 转换总结

转换transform 我们简单理解就是变形 有2D 和 3D 之分
 我们暂且学了三个 分别是 位移 旋转 和 缩放
2D 移动 translate(x, y) 最大的优势是不影响其他盒子， 里面参数用%，是相对于自身宽度和高度来计算的
可以分开写比如 translateX(x) 和 translateY(y)
2D 旋转 rotate(度数) 可以实现旋转元素 度数的单位是deg
2D 缩放 sacle(x,y) 里面参数是数字 不跟单位 可以是小数 最大的优势 不影响其他盒子
设置转换中心点 transform-origin : x y; 参数可以百分比、像素或者是方位名词
当我们进行综合写法，同时有位移和其他属性的时候，记得要将位移放到最前

## 5、CSS3动画

```
@keyframes move {
            from {
                transform:translate(0,0);
            }
            to {
                transform: translate(1000px,0);
            }
        }
        /* 动画序列 */
        
        div {
            width: 100px;
            height: 100px;
            background-color: pink;
            animation-name: move;
            animation-duration: 2s;
        }
        0%
        100% 
        时间划分
```

常用属性

下面的表格列出了 @keyframes 规则和所有动画属性：

| 属性                                                         | 描述                                                         | CSS  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :--- |
| [@keyframes](https://www.runoob.com/cssref/css3-pr-animation-keyframes.html) | 规定动画。                                                   | 3    |
| [animation](https://www.runoob.com/cssref/css3-pr-animation.html) | 所有动画属性的简写属性。                                     | 3    |
| [animation-name](https://www.runoob.com/cssref/css3-pr-animation-name.html) | 规定 @keyframes 动画的名称。                                 | 3    |
| [animation-duration](https://www.runoob.com/cssref/css3-pr-animation-duration.html) | 规定动画完成一个周期所花费的秒或毫秒。默认是 0。             | 3    |
| [animation-timing-function](https://www.runoob.com/cssref/css3-pr-animation-timing-function.html) | 规定动画的速度曲线。默认是 "ease"。                          | 3    |
| [animation-fill-mode](https://www.runoob.com/cssref/css3-pr-animation-fill-mode.html) | 规定当动画不播放时（当动画完成时，或当动画有一个延迟未开始播放时），要应用到元素的样式,forwards,backwards。 | 3    |
| [animation-delay](https://www.runoob.com/cssref/css3-pr-animation-delay.html) | 规定动画何时开始。默认是 0。                                 | 3    |
| [animation-iteration-count](https://www.runoob.com/cssref/css3-pr-animation-iteration-count.html) | 规定动画被播放的次数。默认是 1。infinite 无限。              | 3    |
| [animation-direction](https://www.runoob.com/cssref/css3-pr-animation-direction.html) | 规定动画是否在下一周期逆向地播放。默认是 "normal"。alternate。 | 3    |
| [animation-play-state](https://www.runoob.com/cssref/css3-pr-animation-play-state.html) | 规定动画是否正在运行或暂停。默认是 "running"。pause。        | 3    |

动画简写属性

```
animation：动画名称 持续时间 运动曲线 何时开始 播放次数 是否反方向 动画起始或结束状态；
```

运动曲线：steps（）步长，突变 打字机效果

元素可以添加多个动画，用，分割

## 6、3D转换

三维坐标系 

x右正左负，y下正上负，z外正里负

```
transform:translateX(100px)
transform:translateY(100px)
transform:translateZ(100px) 一般以px为单位
transform:translate3d(x,y,z)
```

### perspective透视

近大远小

写在被观察元素的父盒子上

```
perspective：500px 
```

### rotate3d 3D旋转

元素在三维平面沿着xyz轴进行旋转

```
transform:rotateX(45deg) 沿着X轴正方向旋转45度
transform:rotateY(45deg) 沿着y轴正方向旋转45度
transform:rotateZ(45deg) 沿着z轴正方向旋转45度
transform:rotate3d(x,y,z,45deg) 沿着自定义轴正方向旋转45度
```

左手准则 大拇指朝向轴正方向 手指弯曲的方向就是旋转的方向

### transform-style 3D呈现

控制子元素是否开启三维立体环境

```
transform:flat 子元素不开启3d立体空间 默认
transform-style:preserve-3d; 子元素开启3D空间
```

代码写给父级，但是影响的是子盒子

 两面翻转

旋转木马案例

## 7、浏览器私有前缀

兼容老版本的写法

- -moz-：代表Firefox浏览器私有实行
- -ms-：代表IE浏览器私有属性
- -webkit-：代表Safari、Chrome私有属性
- -o-：代表Opera私有属性

提倡的写法：

```
-moz-border-radius：10px；
-webkit-border-radius：10px；
-o-border-radius：10px；
border-radius：10px；
```

CSS3新增属性

1. 新的选择器

   1. 属性选择器

      [title] [class="demo"]

   2. 结构伪类选择器

      nth-child(n) 数字、关键词、公式

      nth-of-type(n) 根据类型选择

   3. 伪类选择器

      ::before

      ::after

2. 转换transform

   1.  2D 

      translate(x,y)

      rotate(45deg)

      scale(x,y)

   2. 3D

      translate3d(x,y,z)

      rotateX(x)

      rotateY(y)

      rotateZ(z)

3. 动画animation

   1. 重点记住动画简写属性
   2. 动画的暂停，状态等

4. 浏览器私有前缀

