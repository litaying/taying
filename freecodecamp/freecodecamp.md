# 一、 响应式网页设计

在响应式网页设计认证中，你将学习开发者用来编写网页的语言：HTML（超文本标记语言）用于创建内容，CSS（级联样式表）用于样式设计。

首先，你将通过编写一个展示猫咪图片的应用，学习 HTML 和 CSS 的基本知识。 然后，通过画企鹅来学习像 CSS 变量这样的现代技术，以及通过构建网页表单来学习无障碍的最佳实践。

最后，你将学习使用 flexbox（弹性盒子）构建一个 Twitter 卡片，以及使用 CSS 网格构建复杂的博客布局，以此学习制作适应不同屏幕大小的网页。

## 1 基础HTML和HTML5

HTML 是一种标记语言，使用特殊的语法或标记来向浏览器描述网页的结构。HTML 元素由开始和结束标签构成，标签之间是文本内容。 不同的标签可以让文本内容以标题、段落、列表等形式展现。

在这个课程中，你将通过编写一个展示猫咪图片的应用，学习最常见的 HTML 元素——它们可以用来构成任何网页。

h1 标题 h2 副标题 p 段落 <!-- 注释 --> 

### 1.1 **HTML5 元素介绍**

HTML5 引入了很多更具描述性的 HTML 元素， 包括 `main`、`header`、`footer`、`nav`、`video`、`article`、`section` 等等。

这些元素让 HTML 更易读，同时有助于搜索引擎优化和无障碍访问。 `main` 元素让搜索引擎和开发者能很快地找到网页的主要内容。

### 1.2 图片

```
<img src="" alt="">
```

### 1.3 链接

```
<a href="" target="_blank"></a>
```

```
<a href="#"></a>
id=""
```

### 1.4 无序列表

```
<ul>
	<li>
	<li>
</ul>
```

### 1.5 有序列表

```
<ol>
	<li>
	<li>
</ol>
```

### 1.6  web表单

```
<form action="url" >
//单选
<label for="A">A
      <input id="A"  value="a" type="radio" name="ABC" checked>
</label> //name=value checked
<label for="B">B
      <input id="B" value="b" type="radio" name="ABC"
</label>
//复选
<label for="A">A
      <input id="A" value="a" type="checkbox" name="ABC"
    </label>
    <label for="B">B
      <input id="B" value="b" type="checkbox" name="ABC"
</label>
 //输入框
<input type="text" placeholder="" required>
//提交按钮
<button type="submit">Submit</submit> 
</form>
```

### **1.7 元素嵌套**

`div` 元素也叫内容划分元素，是一个包裹其他元素的通用容器。

它也是 HTML 中出现频率最高的元素。

```
<!DOTYPE html>
<html>
	<head>
		<link></link>
		<meta></meta>
		<title></title>
		<style></style>
	</head>
	<body>
		<header></header>
		<footer></footer>
	</body>
</html>
```

## 2 基础CSS

CSS（级联样式表）告诉浏览器如何显示你在 HTML 中写入的文本和其他内容。你可以使用 CSS 控制 HTML 元素的颜色、字体、大小、间距等许多属性。

### 2.1 更改文本颜色

```
<h2 style="color: blue;">H2</h2>
```

### 2.2 使用元素选择器来设置元素的样式

```
<style>
	h2,
	p {
		//更改字体颜色
		color: blue;
		//更改字体大小
		font-size: 30px;
		font-weight: 200px;
		//更改字体族名
		font-family: sans-serif,monospace;
	}
</style>
```

### 2.3  在元素周围添加边框

CSS 边框具有 style、color、width 属性。

```
.box1 {
	border-color: red;
	border-width: 5px;
	border-style: solid;
	//用 border-radius 添加圆角边框
	border-radius: 6px
    //给 box1添加背景色
    background-color: pink;
}

class="box box1"
```

除了 class 属性，每一个 HTML 元素都有一个 id 属性。#id

### 2.4 调整元素的边距

HTML 元素都是以矩形为基础。

每个 HTML 元素所占有的矩形空间由这三个重要的属性来控制：内边距 `padding`、外边距 `margin` 、边框 `border`。

`padding` 用来控制着元素内容与 `border` 之间的空隙大小。

```
padding: 20px;
```

外边距 `margin` 用来控制元素的边框与其他元素之间的 `border` 距离。

```
margin: 20px;
```

给元素添加负外边距
元素的 margin（外边距） 用来控制元素 border（边框） 与其周围元素之间的距离大小。

如果你把元素的 margin 设置为负值，元素会变得占用更多空间。

```
margin: -20px;
```

给元素的每一侧添加不同的边距

padding-top、padding-right、padding-bottom、padding-left 

margin-top、margin-right、margin-bottom、margin-left 

### 2.5 使用属性选择器来设置元素的样式

```
[type='radio'] {
  margin: 20px 0px 20px 0px;
}
```

### 2.6 理解绝对单位与相对单位

单位长度的类型可以分成 2 种：相对和绝对。 绝对单位与长度的物理单位相关。 例如，in 和 mm 分别代表着英寸和毫米。 绝对长度单位会接近屏幕上的实际测量值，不过不同屏幕的分辨率会存在差异，这就可能会造成误差。

相对单位长度，比如 em 和 rem，它们的实际值会依赖其他长度的值而决定。 比如 em 的大小基于元素字体的字体大小。 如果使用它来设置 font-size 值，它的值会跟随父元素的 font-size 值来改变。

### 2.7 选择器优先级

Class 选择器的优先级高于继承样式; 

ID 选择器优先级高于 Class 选择器; 

内联样式的优先级高于 ID 选择器;

Important 的优先级最高

### 2.8 颜色

十六进制 #000000

rgb rgb(0, 0, 0)

### 2.9 使用 CSS 变量一次更改多个元素

```
.penguin {
    --penguin-skin: black;
    --penguin-belly: gray;
    --penguin-beak: yellow;
  }
  .penguin-top {
    background: var(--penguin-skin, gray);
  }
```

### 2.10 继承 CSS 变量

:root 是一个伪类选择器，它是一个能够匹配文档根元素的选择器，通常指的是 html 元素。 我们在 :root 里创建变量在全局都可用，即在任何选择器里都生效。

特定区域或者媒体查询实现

## 3  应用视觉设计

视觉设计结合了排版、色彩理论、图形、动画、页面布局等，以表达独特的信息。

### 3.1 文本排版

使用 text-align 属性创建视觉平衡-文本对齐方式

```
text-align: justify; 将文本隔开，使每行的宽度相等。
text-align: center; 可以让文本居中对齐。
text-align: right; 可以让文本右对齐。
text-align: left; 是默认值，它可以让文本左对齐。
```

```
p {
	text-align: center;
}

img {
  width: 220px;
  height: 100px;
}
```

使用 strong 标签加粗文本

使用 u 标签给文本添加下划线

使用 em 标签强调文本

使用 s 标签给文本添加删除线

使用 hr 标签创建水平线

### 3.2 调整文本的背景色-RGBA

---RGB 值可以取在 0 到 255 之间。 alpha 值可取在 0 到 1 之间，其中 0 代表完全透明，1 代表完全不透明。

调整标题元素与段落元素的大小

---font-size

### 3.3 给卡片元素添加 box-shadow

---box-shadow 属性用来给元素添加阴影，该属性值是由逗号分隔的一个或多个阴影列表。

box-shadow 属性的阴影依次由下面这些值描述：

offset-x 阴影的水平偏移量；
offset-y 阴影的垂直偏移量；
blur-radius 模糊半径；
spread-radius 阴影扩展半径；
color
其中 blur-radius 和 spread-radius 是可选的。

```
box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
```

### 3.4 降低元素的透明度

---CSS 里的 opacity 属性用来设置元素的透明度。

属性值为 1 代表完全不透明。
属性值为 0.5 代表半透明。
属性值为 0 代表完全透明。
透明度会应用到元素内的所有内容，不论是图片，还是文本，或是背景色。

### 3.5 使用 text-transform 属性给文本添加大写效果

```
lowercase   "transform me"
uppercase   "TRANSFORM ME"
capitalize  "Transform Me"
initial     使用默认值
inherit     使用父元素text-transform值
none        Default:不改变文字
```

### 3.6 设置段落的 line-height

### 3.7 调整锚点的悬停状态

伪类是可以添加到选择器上的关键字，用来选择特定状态的元素。可以使用 :hover 伪类选择器来选取超链接的悬停状态。 下面的代码可以在鼠标悬停在超链接上时将其 color 变成红色：

```
a:hover {
  color: red;
}
```

### 3.8 更改元素的相对位置

元素默认按照这种方式布局称为文档的普通流，同时 CSS 提供了 position 属性来覆盖它。当元素的定位设置为 `relative` 时，它允许你通过 CSS 指定该元素在当前文档流页面下的*相对*偏移量。 CSS 里控制各个方向偏移量的属性是 `left`、`right`、`top` 和 `bottom`。 它们代表从原来位置向远离该方向*偏移*指定的像素、百分比或者 em。 下面的例子展示了段落向上偏移 10px：

```
p {
  position: relative;
  bottom: 10px;
}
```

把元素的位置设置成相对，并不会改变该元素在布局中所占的位置，也不会对其它元素的位置产生影响

### 3.9 绝对定位的参照物是元素的父元素

CSS position 属性的取值选项 absolute，它的含义是相对于其包含块定位。 和 relative 定位不一样，绝对定位会将元素从当前的文档流里面移除，周围的元素会忽略它。 这样我们就可以用 CSS 的 top、bottom、left、right 属性来调整元素的位置。

绝对定位比较特殊的一点是元素的定位参照于最近的 positioned 祖先元素。 如果它的父元素没有添加定位规则（默认是 position: relative;），浏览器会继续寻找直到默认的 body 标签。

### 3.10 固定定位的参照物是浏览器的窗口

`fixed` 定位，它是一种特殊的绝对（absolute）定位，将元素相对于浏览器窗口定位。 类似于绝对位置，它与 CSS 偏移属性一起使用，并且也会将元素从当前的文档流里面移除。 其它元素会忽略它的存在，这样也许需要调整其他位置的布局。

但 `fixed` 和 `absolute` 的最明显的区别在于，前者定位的元素不会随着屏幕滚动而移动。

### 3.11 使用 float 属性将元素左浮动或右浮动

浮动元素不在文档流中，它向 `left` 或 `right` 浮动，直到它的外边缘碰到包含框或另一个浮动框的边框为止。 通常需要用 `width` 属性来指定浮动元素占据的水平空间。

```
#left {
      float: left;
      width: 50%;
    }
#right {
      float: right;
      width: 40%;
    }
```

### 3.12 使用 z-index 属性更改重叠元素的位置

 z-index 的取值是整数，数值大的元素会叠放到数值小的元素上面。

### 3.13 用 margin 属性将元素水平居中

在应用设计中经常需要把一个块级元素水平居中显示。 一种常见的实现方式是把块级元素的 `margin` 值设置为 auto。

同样的，这个方法也对图片奏效。 图片默认是内联元素，但是可以通过设置其 `display` 属性为 `block`来把它变成块级元素。

### 3.14 互补色

色环是我们认识颜色关系的好工具。它是一个近色相邻、异色相离的圆环。 当两个颜色恰好在色环的两端时，这两个颜色就互为补色。

### 3.15 三次色

三次色是由原色和二次色相加产生的颜色， 例如，在 RGB 颜色模型中，红色（原色）和黄色（二次色）相加产生橙色（三次色）。 将这六种颜色中相邻的颜色相加，便产生了十二色色环。

设计里面有很多种颜色搭配方法。 涉及到三次色的一种配色方法是分裂补色搭配法。 选定主色之后，在色环上选择与它的补色相邻的两种颜色与之搭配。 此种搭配既有对比，又不失和谐。

### 3.16 色相

颜色具有多种特性，包括色相、饱和度和亮度。 CSS3 引入了 hsl() 做为颜色的描述方式。

色相 是色彩的基本属性，就是平常所说的颜色名称，如红色、黄色等。 以颜色光谱为例，光谱左边从红色开始，移动到中间的绿色，一直到右边的蓝色，色相值就是沿着这条线的取值。 在 hsl() 里面，色相用色环来代替光谱，色相值就是色环里面的颜色对应的从 0 到 360 度的角度值。

饱和度 是指色彩的纯度，也就是颜色里灰色的占比。 饱和度越高则灰色占比越少，色彩也就越纯；反之则完全是灰色。 饱和度的取值范围是表示灰色所占百分比的 0 至 100。

亮度 决定颜色的明暗程度，也就是颜色里白色或者黑色的占比。 其中，100% 的亮度表示纯白色， 0% 的亮度则表示纯黑色；而 50% 的亮度就表示在色相中选取的颜色。

```
红	hsl(0, 100%, 50%)
黄	hsl(60, 100%, 50%)
绿	hsl(120, 100%, 50%)
蓝绿	hsl(180, 100%, 50%)
蓝	hsl(240, 100%, 50%)
品红	hsl(300, 100%, 50%)
```

### 3.17 创建一个 CSS 线性渐变

```
background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);
background: linear-gradient(90deg, red, yellow, rgb(204, 204, 255));
```

### 3.18 使用 CSS 线性渐变创建条纹元素

```
background: repeating-linear-gradient(
      90deg,
      yellow 0px,
      blue 40px,
      green 40px,
      red 80px
    );
```

### 3.19 使用 CSS Transform scale 属性可以更改元素的大小

把页面的段落元素放大到了原来的 2 倍：

```
p {
  transform: scale(2);
}
```

### 3.10 使用 CSS Transform skex 属性沿X、Y轴倾斜元素

`transform` 属性是 `skewX()`：它使选择的元素沿着 X 轴（横向）倾斜指定的角度。

`skewY` 属性使指定元素沿 Y 轴（垂直方向）翻转指定角度

```
transform: skewX(24deg);
```

### 3.11 伪元素

伪元素 `::before` 和 `::after`。 `::before` 创建一个伪元素，它是所选元素的第一个子元素； `::after` 创建一个伪元素，它是所选元素的最后一个子元素。`::before` 和 `::after` 必须配合 `content` 来使用。 这个属性通常用来给元素添加内容诸如图片或者文字。 尽管有时 `::before` 和 `::after` 是用来实现形状而非文字，但 `content` 属性仍然是必需的，此时它的值可以是空字符串。

```
.heart::before {
  content: "";
}
```

### 3.12 CSS 的关键帧和动画是如何工作的

@keyframes

`animation-name` 用来设置动画的名称，也就是我们稍后要在 `@keyframes` 里用到的名称。

`animation-duration` 设置动画所花费的时间。

  `animation-timing-function` 默认值是 `ease`，动画以低速开始，然后加快，在结束前变慢。 其它常用的值包括 `ease-out`：动画以高速开始，以低速结束；`ease-in`，动画以低速开始，以高速结束；`linear`：动画从头到尾的速度是相同的。

```
#anim {
  animation-name: colorful;
  animation-duration: 3s;
  animation-fill-mode: forwards; //保持结束状态
  animation-iteration-count: infinite；//重复动画
  animation-timing-function: ease; //速度曲线
}

@keyframes colorful {
  0% {
    background-color: blue;
  }
  100% {
    background-color: yellow;
  }
}
```

### 3.13 贝塞尔曲线

用 cubic-bezier 来定义贝塞尔曲线。 曲线的形状代表了动画的速度。 曲线在 1 * 1 的坐标系统内， 其中 X 轴代表动画的时间间隔（类似于时间比例尺），Y 轴代表动画的改变。

cubic-bezier 函数包含了 1 * 1 网格里的4个点：p0、p1、p2、p3。 其中 p0 和 p3 是固定值，代表曲线的起始点和结束点，坐标值依次为 (0, 0) 和 (1, 1)。 你只需设置另外两点的 x 值和 y 值，设置的这两点确定了曲线的形状从而确定了动画的速度曲线。 在 CSS 里面通过 (x1, y1, x2, y2) 来确定 p1 和 p2。 以下就是 CSS 贝塞尔曲线的例子：

```
animation-timing-function: cubic-bezier(0.25, 0.25, 0.75, 0.75);
```

## 4  应用无障碍

在网页开发中，可访问性是指网页内容和用户界面可以被用户理解、浏览并与之交互。这里的用户包括有视觉障碍、听觉障碍或认知障碍的用户。

图片添加alt注释

合理利用H1-H6

 HTML5 引入了诸如 main、header、footer、nav、article、section 等大量新标签。默认情况下，浏览器呈现这些元素的方式类似于普通的 div。 但是，在适当的地方使用它们会让标记文本具有更多的含义。 仅标签名称就可以表示它所包含的信息类型，这给内容增加了语义含义。 辅助技术可以获取这种信息，为用户提供更好的页面摘要或导航选项。

`article` 用于独立且完整的内容

`section` 用于对与主题相关的内容进行分组

div 当内容组之间没有联系

nav 导航信息

audio 标签用于呈现音频内容或音频流，它也具有语义化特性。 音频内容也需要备用文本，供聋哑人或听力困难的人使用。 这可以通过页面上的文本或与字幕链接来实现。

```
<audio id="meowClip" controls>
  <source src="audio/meow.mp3" type="audio/mpeg">
  <source src="audio/meow.ogg" type="audio/ogg">
</audio>
```

figure HTML5 引入了 figure 标签以及与之相关的 figcaption 标签。 它们一起用于展示可视化信息（如：图片、图表）及其标题。 这样通过语义化对内容进行分组并配以用于解释 figure 的文字，可以极大地提升内容的可访问性。

```
<figure>
  <img src="roundhouseDestruction.jpeg" alt="Photo of Camper Cat executing a roundhouse kick">
  <br>
  <figcaption>
    Master Camper Cat demonstrates proper form of a roundhouse kick.
  </figcaption>
</figure>
```

label 标签的文本内容通常会是表单组件的名称或标签。 这些文本表明了组件的意义，也提升了表单的可访问性。 label 标签的 for 属性将标签与表单组件绑定；同时，屏幕阅读器也会读取 for 属性的属性值。

```
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
</form>
```

fieldset 标签包裹整组单选按钮，实现这个功能。 它经常使用 legend 标签来提供分组的描述，以便屏幕阅读器用户会阅读 fieldset 元素中的每个选项。

```
<form>
  <fieldset>
    <legend>Choose one of these three items:</legend>
    <input id="one" type="radio" name="items" value="one">
    <label for="one">Choice One</label><br>
    <input id="two" type="radio" name="items" value="two">
    <label for="two">Choice Two</label><br>
    <input id="three" type="radio" name="items" value="three">
    <label for="three">Choice Three</label>
  </fieldset>
</form>
```

type="date"、"time"

如果我们想在页面中添加一些只对屏幕阅读器可见的内容，可以用 CSS 来实现。 当信息为视觉格式（例如图表）时，但屏幕阅读器用户需要备用文稿（例如表格）来访问数据，在这种情况下， 使用 CSS 将屏幕的只读元素放到浏览器窗口可视区域之外。

```
.sr-only {
  position: absolute;
  left: -10000px;
  overflow: hidden;
}
```

高对比度、颜色

accesskey  HTML 提供 accesskey 属性，用于指定激活元素或者使元素获得焦点的快捷键。 添加 accesskey 属性可以让使用键盘的用户更高效率地导航。

```
<button accesskey="b">Important Button</button>
```

tabindex 属性可以指定元素的 tab 键焦点顺序， 将它的值设置为大于等于 1 的整数，就可以实现这个功能。给元素设置 tabindex="1"，键盘将首先把焦点放在这个元素上。 然后它按照指定的 tabindex 值（2、3 等等）顺序循环，再移动到默认值和 tabindex="0" 项目。

```
<div tabindex="1">I get keyboard focus, and I get it first!</div>
<div tabindex="2">I get keyboard focus, and I get it second!</div>
```

## 5  响应式网页设计原则

人们可能通过形状和大小不同的设备来访问网页。通过响应式网页设计，你可以设计出能灵活适应不同屏幕大小、方向和分辨率的网页。

### 5.1 媒体查询

媒体查询是 CSS3 中引入的一项新技术，它可以根据不同的视口大小调整内容的布局。 视口是指浏览器中，用户可见的网页内容。 视口会随访问网站的设备不同而改变。

```
//当设备宽度小于或等于 100px 时返回内容：
@media (max-width: 100px) { /* CSS Rules */ }
//当设备高度大于或等于 350px 时返回内容：
@media (min-height: 350px) { /* CSS Rules */ }
```

### 5.2 图片自适应

```
img {
  max-width: 100%;
  height: auto;
}
```

### 5.3 针对高分辨率屏幕应使用视网膜图片

 像素密度就是区分不同显示设备的一个指标，它一般会以 PPI（Pixel Per Inch，即每英寸像素）或 DPI（每英寸点数）为计量单位。由于“视网膜显示屏”和“非视网膜显示屏”显示器之间像素密度的不同，某些未考虑高分辨率显示器的图像在高分辨率显示器上渲染时，可能因出现“像素化”而不够清晰。

让图像正确出现在高分辨率显示器上的最简单方式， 是定义它们的 `width` 和 `height` 值为原始值的一半。 

```
<style>
  img { 
  height: 250px; 
  width: 250px; 
  }
</style>
<img src="coolPic500x500" alt="A most excellent picture">
```

### 5.4 使排版根据设备尺寸自如响应

除了使用 `em` 或 `px` 设置文本大小，你还可以用视窗单位来做响应式排版。 视窗单位和百分比都是相对单位，但它们是基于不同的参照物。 视窗单位是相对于设备的视窗尺寸（宽度或高度），百分比是相对于父级元素的大小。

四个不同的视窗单位分别是：

- `vw`：如 `10vw` 的意思是视窗宽度的 10%。
- `vh：` 如 `3vh` 的意思是视窗高度的 3%。
- `vmin：` 如 `70vmin` 的意思是视窗的高度和宽度中较小一个的 70%。
- `vmax：` 如 `100vmax` 的意思是视窗的高度和宽度中较大一个的 100%。

下面这个例子是设置 `body` 标签的宽度为视窗宽度的 30%。

```
body { width: 30vw; }
```

## 6 CSS弹性盒子

Flexbox（弹性盒子）是最新版本的 CSS（即 CSS3）中引入的一种强大且兼容性好的布局方法。使用 flexbox，我们可以很容易地处理好页面上的元素布局，并创建可以自动缩小和放大的动态用户界面。

### 6.1 使用 display: flex 定位两个盒子

```
<style>
  #box-container {
    height: 500px;
    display: flex;
  }

  #box-1 {
    background-color: dodgerblue;
    width: 50%;
    height: 50%;
  }

  #box-2 {
    background-color: orangered;
    width: 50%;
    height: 50%;
  }
</style>
<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>
```

### 6.2 使用 flex-direction 属性创建一个行

属性值为 row 或 column，即可横向排列或纵向排列它的所有子元素。 创建一行将使子项水平对齐，创建一列将使子项垂直对齐。flex-direction 的其他可选值还有 row-reverse 和 column-reverse。

```
#box-container {
    display: flex;
    height: 500px;
    flex-direction: column;
  }
```

### 6.3 使用 justify-content 属性对齐元素

以什么方式排列 flex 子元素，以及调整它们的间距

- `flex-start`：从 flex 容器的起始位置开始排列项目。 对行来说是把项目移至左边， 对于列是把项目移至顶部。 如未设置 `justify-content` 的值，那么这就是默认值。
- `flex-end`：从 flex 容器的终止位置开始排列项目。 对行来说是把项目移至右边， 对于列是把项目移至底部。
- `space-between`：项目间保留一定间距地沿主轴居中排列。 第一个和最后一个项目被放置在容器边沿。 例如，在行中第一个项目会紧贴着容器左边，最后一个项目会紧贴着容器右边，然后其他项目均匀排布。
- `space-around`：与`space-between`相似，但头尾两个项目不会紧贴容器边缘，所有项目之间的空间均匀排布。
- `space-evenly`：头尾两个项目不会紧贴容器边缘，所有项目之间的空间均匀排布。

### 6.4 使用 align-items 属性对齐元素

 `align-items` 属性用来定义 flex 子元素沿交叉轴的对齐方式。

- `flex-start`：从 flex 容器的起始位置开始对齐项目。 对行来说，把项目移至容器顶部； 对列来说，是把项目移至容器左边。
- `flex-end`：从 flex 容器的终止位置开始对齐项目。 对行来说，把项目移至容器底部； 对列来说，把项目移至容器右边。
- `center`：把项目居中放置。 对行来说，垂直居中（项目距离顶部和底部的距离相等）； 对列来说，水平居中（项目距离左边和右边的距离相等）。
- `stretch`：拉伸项目，填满 flex 容器。 例如，排成行的项目从容器顶部拉伸到底部。 如未设置`align-items`的值，那么这就是默认值。
- `baseline`：沿基线对齐。 基线是文本相关的概念，可以认为它是字母排列的下端基准线。

### 6.5 使用 flex-wrap 属性包裹一行或一列

- `nowrap`：默认值，不换行。
- `wrap`：如果排列以行为基准，就将行从上往下排列；如果排列以列为基准，就将列从左往右排列。
- `wrap-reverse`：如果排列以行为基准，就将行从下往上排列；如果排列以列为基准，就将列从右往左排列。

#### 6.6 使用 flex-shrink 属性定义 flex 子元素的收缩规则

上边的属性都是应用于 flex 容器（flex 子元素的父元素）的。 除此之外，flex 子元素也有很多实用属性。

flex-shrink 属性。 使用之后，如果 flex 容器太小，则子元素会自动缩小。 当容器的宽度小于里面所有子元素的宽度之和时，所有子元素都会自动压缩。数值越大，则该元素与其他元素相比会被压缩得更厉害。

```
#box-1 {
    background-color: dodgerblue;
    width: 100%;
    height: 200px;
    flex-shrink: 1;
  }

  #box-2 {
    background-color: orangered;
    width: 100%;
    height: 200px;
    flex-shrink: 2;
  }
```

### 6.7 使用 flex-grow 属性定义 flex 子元素的增长系数

flex-grow 会在容器太大时对子元素作出调整。

```
	flex-grow: 1;
	flex-grow: 2;
```

### 6.8 使用 flex-basis 属性设置元素的初始大小

flex-basis 属性定义了在使用 CSS 的 flex-shrink 或 flex-grow 属性对元素进行调整前，元素的初始大小。

```
	flex-basis: 10em;
	flex-basis: 20em;
```

### 6.9 使用 flex 短方法属性

```
flex: 1 0 10px; 会把项目属性设为 flex-grow: 1;、flex-shrink: 0; 以及 flex-basis: 10px;。
```

### 6.10 使用 order 属性重新排列子元素

order 属性告诉 CSS flex 容器里子元素的顺序。 默认情况下，项目排列顺序与源 HTML 文件中顺序相同。 这个属性接受数字作为参数，可以使用负数。

### 6.11 使用 align-self 属性

调整单个子元素自己的对齐方式，而不会影响到全部子元素。align-self 可设置的值与 align-items 的一样，并且它会覆盖 align-items 所设置的值。

center，flex-end...

## 7、CSS网格

CSS 网格是一个较新的标准，用于构建复杂的响应布局。它通过把 HTML 元素转换为具有行和列的网格容器，以便将子元素放置在所需要的位置。

通过将属性 `display` 的值设为 `grid`，HTML 元素就可以变为网格容器。

### 7.1 使用 grid-template-columns 添加多列

```
.container {
  display: grid;
  grid-template-columns: 50px 50px;
}
```

### 7.2 使用 grid-template-rows 添加多行

```
grid-template-rows: 50px 50px;
```

### 7.3 使用 CSS 网格单位来更改列和行的大小

在 CSS 网格中，可以使用绝对单位（如 `px`）或相对单位（如 `em`）来定义行或列的大小。 下面的单位也可以使用：

`fr`：设置列或行占剩余空间的比例，

`auto`：设置列宽或行高自动等于它的内容的宽度或高度，

`%`：将列或行调整为它的容器宽度或高度的百分比

```
grid-template-columns: auto 50px 10% 2fr 1fr;
```

### 7.4 使用 grid-column-gap 创建多列或多列之间的间距

在你所创建的网格中，每列都相互紧挨着。 有时候你想要列之间有一个间距。 如果需要在列与列之间添加一些间距，我们可以使用 grid-column-gap：

```
grid-column-gap: 10px;
```

```
grid-row-gap: 10px;
```

### 7.5 使用 grid-gap 为网格添加间距

grid-gap 属性是前两个挑战中出现的 grid-row-gap 和 grid-column-gap 的简写属性，它更方便使用。 如果 grid-gap 只有一个值，那么这个值表示行与行之间、列与列之间的间距均为这个值。 如果有两个值，那么第一个值表示行间距，第二个值表示列间距。

```
grid-gap: 10px 20px;
```

### 7.6 使用 grid-column /grid-row来控制空间大小

`grid-column` `grid-row`属性是用于网格项本身的属性。

```
grid-column: 1 / 3;
grid-row: 2 / 5;
```

### 7.7 使用 justify-self 水平对齐项目

 justify-self 属性，设置其内容的位置在单元格内沿水平轴的对齐方式。 默认情况下，这个属性的值是 stretch，这将使内容占满整个单元格的宽度。

`start`：使内容在单元格左侧对齐，

`center`：使内容在单元格居中对齐，

`end`：使内容在单元格右侧对齐，

```
justify-self: center;
```

### 7.8 使用 align-self 垂直对齐项目

网格项沿竖直方向的对齐方式

```
align-self: center;
```

### 7.9 使用 justify-items 水平对齐所有项目

对网格容器使用 justify-items 使它们一次性沿水平轴对齐。

```
justify-items: center;
```

### 7.10 使用 align-items 垂直对齐所有项目

对网格容器使用 align-items 属性可以让网格中所有的网格项沿竖直方向对齐。

```
align-items: center;
```

### 7.11 将网格划分为区域模板

你可以将网格中的一些单元格组合成一个区域（area），并为该区域指定一个自定义名称。 可以通过给容器加上 grid-template-areas 来实现：

```
grid-template-areas:
  "header header header"
  "advert content content"
  "advert footer footer";
```

### 7.12 使用 grid-area 属性将项目放置在网格区域中

在为网格添加区域模板后，可以通过引用你所定义的区域的名称，将元素放入相应的区域。 为此，你需要对网格项使用 grid-area：

```
.item1 {
  grid-area: header;
}
```

### 7.13 使用 grid-area 创建区域模板

如果网格中没有定义区域模板，你也可以像这样为它添加一个模板：—  | —  |  y1,x1,y2,x2

```
grid-area: horizontal line to start at / vertical line to start at / horizontal line to end at / vertical line to end at;
item1 { grid-area: 1/1/2/4; }
```

### 7.14 使用 repeat 函数减少重复

使用 grid-template-columns 或 grid-template-rows 定义网格结构时，你需要为添加的每一行或每一列都输入一个值。

如果一个网格共有 100 行且每行高度相同， 那我们就需要输入 100 个值，这显然不太实际。 为此，更好的方式是使用 repeat 方法指定行或列的重复次数，后面加上逗号以及需要重复的值。

```
grid-template-rows: repeat(100, 50px);
grid-template-columns: repeat(2, 1fr 50px) 20px;
grid-template-columns: 1fr 50px 1fr 50px 20px;
```

### 7.15 使用 minmax 函数限制项目大小

置函数 minmax 也可用于设置 grid-template-columns 和 grid-template-rows 的值。 它的作用是在网格容器改变大小时限制网格项的大小。 为此，你需要指定网格项允许的尺寸范围。 例如：

```
grid-template-columns: 100px minmax(50px, 200px);
```

### 7.16 使用 auto-fill 创建弹性布局

repeat 方法带有一个名为自动填充（auto-fill）的功能。 它的功能是根据容器的大小，尽可能多地放入指定大小的行或列。 你可以通过结合 auto-fill 和 minmax 来更灵活地布局。

```
repeat(auto-fill, minmax(60px, 1fr));
```

### 7.18 使用 auto-fit 创建弹性布局

auto-fit 效果几乎和 auto-fill 一样。 不同点仅在于，当容器的大小大于各网格项之和时，auto-fill 会持续地在一端放入空行或空列，这样就会使所有网格项挤到另一边；而 auto-fit 则不会在一端放入空行或空列，而是会将所有网格项拉伸至合适的大小。

```
grid-template-columns: repeat(autofit, minmax(60px, 1fr));
```

### 7.19 使用媒体查询创建响应式布局

将 CSS 网格与使用媒体查询结合使用，如使用媒体查询重新排列网格区域、更改网格尺寸以及重新排列网格项位置，我们可以让制作出的网站更具响应性.

```
@media (min-width: 400px){
    .container{
      grid-template-areas:
        "advert header"
        "advert content"
        "advert footer";
    }
  }
```

### 7.20 在网格中创建网格

将元素转换为网格只会影响其子元素（即直接后代元素，英文为 direct descendants。意思是一个元素的所有后代元素中，父级元素为该元素的所有元素）。 因此，如果我们把某个子元素设置为网格，就会得到一个嵌套的网格。

```
.item3 {
    background: PaleTurquoise;
    grid-area: content;
    display: grid;
    grid-template-columns: auto 1fr;
  }
```

# 二、 Emmet 语法 速查表

![img](https://upload-images.jianshu.io/upload_images/2836722-2f241e2455b5dc46.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/550/format/webp)

**Emmet是一款文本编辑器/IDE的插件，用来快速生成复杂的HTML代码，只要掌握一些常用的语法（类似于CSS选择器），就可以减少重复编码的工作。**

------

#### 1.调用方法

> ##### Emmet使用Tab作为自动生成HTML代码的触发器。

###### 输入完生成HTML的缩写语句后，按下Tab，即可生成对应的HTML代码

#### 2.相关语法

> ##### 后代：>

------

##### Child: >

**缩写**：`div>ul>li`



```xml
    <div>
        <ul>
            <li></li>
        </ul>
    </div>
```

> ##### 兄弟：+

------

##### Sibling: +

**缩写**：`div+p+bq`



```xml
    <div></div>
    <p></p>
    <blockquote></blockquote>
```

> ##### 上级元素：^

------

##### Climb-up: ^

**缩写**：`div+div>p>span+em^bq`



```xml
    <div></div>
    <div>
        <p><span></span><em></em></p>
        <blockquote></blockquote>
    </div>
```

**缩写**：`div+div>p>span+em^^bq`



```xml
    <div></div>
    <div>
        <p><span></span><em></em></p>
    </div>
    <blockquote></blockquote>
```

> ##### 分组：（）

------

##### Grouping: ( )

**缩写**：`div>(header>ul>li*2>a)+footer>p`



```xml
    <div>
        <header>
            <ul>
                <li><a href=""></a></li>
                <li><a href=""></a></li>
            </ul>
        </header>
        <footer>
            <p></p>
        </footer>
    </div>
```

**缩写**：`(div>dl>(dt+dd)*3)+footer>p`



```xml
    <div>
        <dl>
            <dt></dt>
            <dd></dd>
            <dt></dt>
            <dd></dd>
            <dt></dt>
            <dd></dd>
        </dl>
    </div>
    <footer>
        <p></p>
    </footer>
```

> ##### 重复多份：*

------

##### Multiplication: *

**缩写**：`ul>li*5`



```xml
    <ul>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
    </ul>
```

> ##### 编号：$

------

##### Item numbering: $

**缩写**：`ul>li.item$*5`



```xml
    <ul>
        <li class="item1"></li>
        <li class="item2"></li>
        <li class="item3"></li>
        <li class="item4"></li>
        <li class="item5"></li>
    </ul>
```

**缩写**：`h$[title=item$]{Header $}*3`



```xml
    <h1 title="item1">Header 1</h1>
    <h2 title="item2">Header 2</h2>
    <h3 title="item3">Header 3</h3>
```

**缩写**：`ul>li.item$$$*5`



```xml
    <ul>
        <li class="item001"></li>
        <li class="item002"></li>
        <li class="item003"></li>
        <li class="item004"></li>
        <li class="item005"></li>
    </ul>
```

**缩写**：`ul>li.item$@-*5`



```xml
    <ul>
        <li class="item5"></li>
        <li class="item4"></li>
        <li class="item3"></li>
        <li class="item2"></li>
        <li class="item1"></li>
    </ul>
```

**缩写**：`ul>li.item$@3*5`



```xml
    <ul>
        <li class="item3"></li>
        <li class="item4"></li>
        <li class="item5"></li>
        <li class="item6"></li>
        <li class="item7"></li>
    </ul>
```

> ##### ID和类属性

------

##### ID and CLASS attributes

**缩写**：`#header`



```xml
    <div id="header"></div>
```

**缩写**：`.title`



```jsx
    <div class="title"></div>
```

**缩写**：`form#search.wide`



```jsx
    <form action="" id="search" class="wide"></form>
```

**缩写**：`p.class1.class2.class3`



```jsx
    <p class="class1 class2 class3"></p>
```

> ##### 自定义属性

------

##### Custom attributes

**缩写**：`p[title="Hello world"]`



```xml
    <p title="Hello world"></p>
```

**缩写**：`td[rowspan=2 colspan=3 title]`



```xml
    <td rowspan="2" colspan="3" title=""></td>
```

**缩写**：`[a='value1' b="value2"]`



```xml
    <div a="value1" b="value2"></div>
```

> ##### 文本：{ }

------

##### Text: { }

**缩写**：`a{Click me}`



```xml
     <a href="">Click me</a>
```

**缩写**：`p>{Click }+a{here}+{ to continue}`



```xml
    <p>Click <a href="">here</a> to continue</p>
```

> ##### 隐式标签

------

##### Implicit tag names

**缩写**：`.class`



```ruby
    <div class></div>
```

**缩写**：`em>.class`



```xml
    <em><span class="class"></span></em>
```

**缩写**：`ul>.class`



```xml
    <ul> <li class="class"></li></ul>
```

**缩写**：`table>.row>.col`



```xml
    <table>
        <tr class="row">
            <td class="col"></td>
        </tr>
    </table>
```

##### 3.HTML

> *所有未知的缩写都会转换成标签，例如，foo → <foo></foo>*
> **缩写**：`!`



```xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

------

> 本文所列仅为最常用的一些语法和缩写，有关其他较为少用的可参考[Emmet官方文档](https://link.jianshu.com/?t=http%3A%2F%2Fdocs.emmet.io%2Fcheat-sheet%2F)

**特别声明：**文中演示代码来自于官网API：[http://docs.emmet.io/cheat-sheet/](https://link.jianshu.com/?t=http%3A%2F%2Fdocs.emmet.io%2Fcheat-sheet%2F)

