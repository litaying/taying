# **HTML菜鸟教程学习笔记**

# 1 HTML简介

HTML实例

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>菜鸟教程(runoob.com)</title>
    </head>
    <body>
        <h1>
            我的第一个标题
        </h1>
        <p>
            我的第一个段落
        </p>
    </body>
</html>
```

实例演示：

------



<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title> 菜鸟教程(runoob.com)</title>
    </head>
    <body>
        <h1>
            我的第一个标题
        </h1>
        <p>
            我的第一个段落
        </p>
    </body>
</html>


------

实例解析

![img](https://www.runoob.com/wp-content/uploads/2013/06/02A7DD95-22B4-4FB9-B994-DDB5393F7F03.jpg)

- !DOCTYPE声明为HTML5文档

- html是HTML页面的根元素

- head包含了文档的元数据（meta），如<meta charset="utf-8"定义网页编码格式为utf-8。
- titlle描述了文档的标题
- body元素包含了可见的界面
- h1元素定义一个大标题
- p元素定义一个段落

什么是HTML？

超文本标记语言 Hyper Text Markup Language

HTMl文档也叫web界面

HTML标签

开始标签 结束标签 开放标签 闭合标签

```
<标签>内容</标签>
```



HTML元素

元素包含两个标签

web浏览器

读取HTML文件，显示为网页。

HTML网页结构

<div style="width:99%;border:1px solid grey;padding:3px;margin:0;background-color:#ddd">&lt;html&gt;
<div style="width:90%;border:1px solid grey;padding:3px;margin:20px">&lt;head&gt;
<div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;title&gt;页面标题&lt;/title&gt;
</div>
&lt;/head&gt;
</div>
<div style="width:90%;border:1px solid grey;padding:3px;margin:20px;background-color:#fff">&lt;body&gt;
<div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;h1&gt;这是一个标题&lt;/h1&gt;</div>
<div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;p&gt;这是一个段落。&lt;/p&gt;</div>
<div style="width:90%;border:1px solid grey;padding:5px;margin:20px">&lt;p&gt;这是另外一个段落。&lt;/p&gt;</div>
&lt;/body&gt;
</div>
&lt;/html&gt;
</div>

只有白色部分会在浏览器中显示。

HTML版本

不同HTML版本有不同声明。

课后笔记：

1. doctype 声明是不区分大小写的，用来告知 Web 浏览器页面使用了哪种 HTML 版本。

在HTML 4.01 中，<!DOCTYPE> 声明需引用 DTD （文档类型声明），因为 HTML 4.01 是基于 SGML（Standard Generalized Markup Language 标准通用标记语言）。

HTML 4.01 规定了三种不同的 <!DOCTYPE> 声明，分别是：Strict、Transitional 和 Frameset。

HTML5 不是基于 SGML，因此不要求引用 DTD。

2. 对于中文网页需要使用 <meta charset="utf-8"> 声明编码，否则会出现乱码。有些浏览器(如 360 浏览器)会设置 GBK 为默认编码，则你需要设置为 <meta charset="gbk">。

目前在大部分浏览器中，直接输出中文会出现中文乱码的情况，这时候需要在头部将字符声明为 UTF-8。

# 2 HTML基础

HTML标题

通过<h1>到<h6>定义

```
<h1>这是h1标题</h1>
<h2>这是h2标题</h2>
<h3>这是h3标题</h3>
<h4>这是h4标题</h4>
<h5>这是h1标题</h5>
<h6>这是h1标题</h6>
```

实例演示：

<h1>这是h1标题</h1>

<h2>这是h2标题</h2>

<h3>这是h3标题</h3>

<h4>这是h4标题</h4>

<h5>这是h5标题</h5>

<h6>这是h6标题</h6>

HTML段落

通过<p>标签定义

```
<p>这是一个段落。</p>
<p>这是另一个段落。</p>
```

实例演示：

<p>这是一个段落。</p>

<p>这是另一个段落。</p>

HTML链接

通过<a>定义

```
<a href="http://www.runoob.com">这是一个链接</a>
```

实例演示：

<a href="http://www.runoob.com">这是一个链接</a>

HTML图像

通过&lt;img&gt;定义

```
<img loading="lazy" src="http://www.runoob.com/images/logo.png" width="258" height="39" />
```

实例演示：

<img loading="lazy" src="http://www.runoob.com/images/logo.png" width="258" height="39" />

# 3 HTML元素

HTML文档由相互嵌套的HTML元素构成。

没有美容的HTML元素被称空元素。

元素&lt;br&gt;通过<br/&gt;关闭

HTML标签对大小写不敏感，推荐小写。

# 4 HTML属性

属性是HTML元素提供的附加属性

一般描述于开始标签

以名称/值对的形式出现

name="value"

如：

```
<a href="http://www.runoob.com">这是一个链接</a>
```

<table class="reference">
<tbody><tr>
<th align="left" width="15%">属性</th>
<th align="left" width="85%">描述</th>
</tr>
<tr>
<td>class</td>
<td>为html元素定义一个或多个类名（classname）(类名从样式文件引入)</td>
</tr>
<tr>
<td>id</td>
<td>定义元素的唯一id</td>
</tr>
<tr>
<td>style</td>
<td>规定元素的行内样式（inline style）</td>
</tr>
<tr>
<td>title</td>
<td>描述了元素的额外信息 (作为工具条使用)</td>
</tr>
</tbody></table>

# 5 HTML标题

搜素引擎通过标题来为您的网页的结构和内容编制索引

按重要性从h1到h6排序

HTML水平线

元素<hr>在HTML页面中创建水平线用于分割内容

HTML注释

```
<!--这是一行注释-->
```

实例演示：

<!--这是一行注释-->

# 6 HTML段落

浏览器会自动地在段落前后添加空行

**br标签**

在不产生新段落的情况下换行

浏览器在显示页面时会移除多余的空格和空行，所有连续的空格和空行会被算作一个

# 7 HTML文本格式化

**文本格式化**

```
<b>This text is bold.</b>
<br/>
<strong>This text is strong.</strong>
<br/>
<big>This text is big.</big>
<br/>
<em>This text is emphasis.</em>
<br/>
<i>This test is italic.</i>
<br/>
<small>This test is small.</small>
<br/>
This test includes <sup> superscript.</sup>
<br/>
This test includes <sub>supscript.</sub>
```

**实例演示：**

<b>This text is bold.</b>
<strong>This text is strong.</strong>
<big>This text is big.</big>
<em>This text is emphasis.</em>
<i>This test is italic.</i>

<small>This test is small.</small>
This test includes<sup>subscript.</sup>
This test includes<sub>supscript.</sub>

**预格式文本**

```
<pre>
This example demonstrates how to use the pre tag
to control
blank lines and space.
</pre>
```

**Example demonstration:**

<pre>
This example demonstrates how to use the pre tag
to control
blank lines and space.
</pre>
**计算机输出标签**

```
<code>computer output</ceode>
<kbd>keyboard input</kbd>
<tt>teletype text</tt>
<samp>computer code sample</samp>
<var>computer variable</var>
<b>These tags are often used to display computer/programming code.</b>
```

**Example demonstration:**

<code>computer output</ceode>
<kbd>keyboard input</kbd>
<tt>teletype text</tt>
<samp>computer code sample</samp>
<var>computer variable</var>
<b>These tags are often used to display computer/programming code.</b>

**address:**

```
<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br/>
Visit us at:<br/>
Example.com<br/>
Box 564,Disneyland<br/>
USA
</address>
```

**Example demostration:**

<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br/>
Visit us at:<br/>
Example.com<br/>
Box 564,Disneyland<br/>
USA
</address>
**Abbreviations and aronyms 缩写和首字母缩写**

```
<abbr title="etcetera">etc.</abbr>
<acronym title="World Wide Web">WWW</acronym>
```

**Example demostration:**

<abbr title="etcetera">etc.</abbr>

<acronym title="World Wide Web">WWW</acronym>

**BiDirectional Override 文字方向（双向覆盖文本的方向**）

rtl right to left

ltr left to right

```
<p>This paragraph text displayed from left to right.</p>
<p><bdo dir=rtl>This paragraph text displayed from right to left.</bdo><p>
```

**Example demostration:**

<p>This paragraph text displayed from left to right.</p>
<p><bdo dir=rtl>This paragraph text displayed from right to left.</bdo><p>
**block quote 块引用**

```
<p>WWF's goal is to:
<q>Build a future where people live in harmony with nature.</q>
We hope they succeed.</p>
```

<p>WWF's goal is to:
    <q>Build a future where people live in harmony with nature.</q>
We hope they succeed.</p>

Delete words effect  and insert word effect

```
<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
```

<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>

HTMl text formatting tags HTML文本格式化标签

<table class="reference notranslate">
<tbody><tr>
<th width="20%" align="left">标签</th>
<th width="80%" align="left">描述</th>
</tr>
<tr>
<td><a href="/tags/tag-b.html">&lt;b&gt;</a></td>
<td>定义粗体文本</td>
</tr>
<tr>
<td><a href="/tags/tag-em.html">&lt;em&gt;</a></td>
<td>定义着重文字</td>
</tr>
<tr>
<td><a href="/tags/tag-i.html">&lt;i&gt;</a></td>
<td>定义斜体字</td>
</tr>
<tr>
<td><a href="/tags/tag-small.html">&lt;small&gt;</a></td>
<td>定义小号字</td>
</tr>
<tr>
<td><a href="/tags/tag-strong.html">&lt;strong&gt;</a></td>
<td>定义加重语气</td>
</tr>
<tr>
<td><a href="/tags/tag-sub.html">&lt;sub&gt;</a></td>
<td>定义下标字</td>
</tr>
<tr>
<td><a href="m/tags/tag-sup.html">&lt;sup&gt;</a></td>
<td>定义上标字</td>
</tr>
<tr>
<td><a href="/tags/tag-ins.html">&lt;ins&gt;</a></td>
<td>定义插入字</td>
</tr>
<tr>
<td><a href="/tags/tag-del.html">&lt;del&gt;</a></td>
<td>定义删除字</td>
</tr>
</tbody></table>

HTML “computer output” tags  HTML“计算机输出”标签

<table class="reference notranslate">
<tbody><tr>
<th width="20%" align="left">标签</th>
<th width="80%" align="left">描述</th>
</tr>
<tr>
<td><a href="/tags/tag-code.html">&lt;code&gt;</a></td>
<td>定义计算机代码</td>
</tr>
<tr>
<td><a href="/tags/tag-kbd.html">&lt;kbd&gt;</a></td>
<td>定义键盘码</td>
</tr>
<tr>
<td><a href="/tags/tag-samp.html">&lt;samp&gt;</a></td>
<td>定义计算机代码样本</td>
</tr>
<tr>
<td><a href="/tags/tag-var.html">&lt;var&gt;</a></td>
<td>定义变量</td>
</tr>
<tr>
<td><a href="/tags/tag-pre.html">&lt;pre&gt;</a></td>
<td>定义预格式文本</td>
</tr>
</tbody></table>
**HTML citations**

<table class="reference notranslate">
<tbody><tr>
<th width="20%" align="left">标签</th>
<th width="80%" align="left">描述</th>
</tr>
<tr>
<td><a href="/tags/tag-abbr.html">&lt;abbr&gt;</a></td>
<td>定义缩写</td>
</tr>
<tr>
<td><a href="/tags/tag-address.html">&lt;address&gt;</a></td>
<td>定义地址</td>
</tr>
<tr>
<td><a href="/tags/tag-bdo.html">&lt;bdo&gt;</a></td>
<td>定义文字方向</td>
</tr>
<tr>
<td><a href="/tags/tag-blockquote.html">&lt;blockquote&gt;</a></td>
<td>定义长的引用</td>
</tr>
<tr>
<td><a href="/tags/tag-q.html">&lt;q&gt;</a></td>
<td>定义短的引用语</td>
</tr>
<tr>
<td><a href="/tags/tag-cite.html">&lt;cite&gt;</a></td>
<td>定义引用、引证</td>
</tr>
<tr>
<td><a href="/tags/tag-dfn.html">&lt;dfn&gt;</a></td>
<td>定义一个定义项目。</td>
</tr>
</tbody></table>

# 8 HTML链接

```
<a href="www.baidu.com">baidu</a>
```

<a href="www.baidu.com">baidu</a>

**target attributes**

target 定义被链接文档显示位置

_blank 在新窗口打开

```
<a href="http://www.baidu.com" target="_blank">visit runoob</a>
```

<a href="http://www.baidu.com" target="_blank">visit runoob</a>

**Picture link**

<p>创建图片链接：
    <a href="http://www.baidu.com">
       <img border="10" src="https://img0.baidu.com/it/u=1514002029,2035215441&fm=26&fmt=auto&gp=0.jpg" alt="HTML教程" width="32" height="32"></a>
</p>

```
<p>创建图片链接：
    <a href="http://www.baidu.com">
       <img border="10" src="https://img0.baidu.com/it/u=1514002029,2035215441&fm=26&fmt=auto&gp=0.jpg" alt="HTML教程" width="32" height="32"></a>
</p>
```

Link to the specified location on the current page

<p>
    <a href="#T1">跳转到页尾</a>
</p>        

# 9 HTML头部

**Define the URL of all links**

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>菜鸟教程</title>
        <base href="http://www.runoob.com/images/" target="_blank">
    </head>

    <body>
        <img src="logo.png">
        <br/><br/>
        <a href="http://www.runoob.com">菜鸟教程</a>
    </body>
</html>
```

 **head元素**

插入脚本（script），样式文件（CSS），以及各种meta信息

可添加元素标签为title,style,meta,link,script,noscipt和base。

**title元素**

定义浏览器工具栏标题

收藏夹标题

搜索引擎结果标题

**base元素**

描述基本的链接地址和链接目标，所有链接标签的默认链接。

link元素

定义文档与外部资源的关系

通常用于链接到样式表

```
<head><link rel="stylesheet" type="txet/css" href="mystyle.css">
</head>
```

**style元素**

定义HTML文档的样式文件引用地址

可以再style元素中直接添加样式渲染文档

```
<head>
<style type="text/css">
body {background-color:yellow}
p {color:blue}
</style>
</head>
```

**meta元素**

描述基本的元数据

通常用于指定网页的描述，关键词，文件的最后修改时间，作者和其他元数据

```
<!--为搜索引擎定义关键字-->
<meta name="keywords" content="HTML,CSS,XML,XHTML,JavaScript">

<!--为网页定义描述内容-->
<meta name="desciption" content="免费 Web & 编程 教程">

<!--定义网页作者-->
<meta name="author" content="Runoob">

<!--每30秒钟刷新当前页面-->
<meta http-equiv="refresh" content="30">
```

**script元素**

加载脚本文件

<table class="reference">
<tbody><tr>
<th width="20%" align="left">标签</th>
<th width="80%" align="left">描述</th>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-head.html" rel="noopener noreferrer">&lt;head&gt;</a></td>
<td>定义了文档的信息</td>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-title.html" rel="noopener noreferrer">&lt;title&gt;</a></td>
<td>定义了文档的标题</td>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-base.html" rel="noopener noreferrer">&lt;base&gt;</a></td>
<td>定义了页面链接标签的默认链接地址</td>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-link.html" rel="noopener noreferrer">&lt;link&gt;</a></td>
<td>定义了一个文档和外部资源之间的关系</td>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-meta.html" rel="noopener noreferrer">&lt;meta&gt;</a></td>
<td>定义了HTML文档中的元数据</td>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-script.html" rel="noopener noreferrer">&lt;script&gt;</a></td>
<td>定义了客户端的脚本文件</td>
</tr>
<tr>
<td><a target="_blank" href="/tags/tag-style.html" rel="noopener noreferrer">&lt;style&gt;</a></td>
<td>定义了HTML文档的样式文件</td>
</tr>
</tbody></table>



# 10 HTML样式-CSS

**Cascading Style Sheet 级联样式表**

渲染HTML元素标签的样式

<div style="position:relative;">
	<div style="opacity:0.5;position:absolute;left:50px;top:-30px;width:300px;height:150px;background-color:#40B3DF"></div>
	<div style="opacity:0.3;position:absolute;left:120px;top:20px;width:100px;height:200px;background-color:#8AC007"></div>
	<div style="margin-top:30px;width:360px;height:130px;padding:20px;border-radius:10px;border:10px solid #EE872A;font-size:120%;">
		<h1>Look! Styles and colors</h1>
		<div style="letter-spacing:12px;font-size:15px;position:relative;left:25px;top:10px;">Manipulate Text</div>
		<div style="color:#40B3DF;letter-spacing:12px;font-size:15px;position:relative;left:25px;top:20px;">Colors, <span style="background-color:#B4009E;color:#ffffff;">&nbsp;Boxes</span></div>
		<div style="color:#000000;letter-spacing:-1px;font-size:15px;position:relative;top:15px;">and more...</div>
	</div>
</div>







```
<div style="position:relative;">
	<div style="opacity:0.5;position:absolute;left:50px;top:-30px;width:300px;height:150px;background-color:#40B3DF"></div>
	<div style="opacity:0.3;position:absolute;left:120px;top:20px;width:100px;height:200px;background-color:#8AC007"></div>
	<div style="margin-top:30px;width:360px;height:130px;padding:20px;border-radius:10px;border:10px solid #EE872A;font-size:120%;">
		<h1>Look! Styles and colors</h1>
		<div style="letter-spacing:12px;font-size:15px;position:relative;left:25px;top:10px;">Manipulate Text</div>
		<div style="color:#40B3DF;letter-spacing:12px;font-size:15px;position:relative;left:25px;top:20px;">Colors, <span style="background-color:#B4009E;color:#ffffff;">&nbsp;Boxes</span></div>
		<div style="color:#000000;letter-spacing:-1px;font-size:15px;position:relative;top:15px;">and more...</div>
	</div>
</div>
```

**CSS使用方法**

内联样式—在HTML元素中使用“style”属性

内部样式表—在文档头部head区域使用style元素来包含CSS

外部引用—使用外部CSS文件

最好的方式是外部引用

**内联样式**

特殊的样式应用到个别元素时，在相关的标签页使用样式属性。

改变段落的颜色和外边框

<p style="color:blue;margin-left:20px;">这是一个段落。</p>

```
<p style="color:blue;margin-left:20px;">这是一个段落。</p>
```

**背景颜色**

<body style="background-color:yellow;">

<h2 style="background-color:red;">这是一个标题</h2>

<p style="background-color:green;">这是一个段落</p>

```
<body style="background-color:yellow;">
<h2 style="background-color:red;">这是一个标题</h2>
<p style="background-color:green;">这是一个段落</p>
```

**字体、字体颜色、字体大小**

<h1 style="font-family:verdana">一个标题</h1>
<p style="font-family:arial;color:red;font-size:20px;">一个段落。</p>

```
<h1 style="font-family:verdana">一个标题</h1>
<p style="font-family:arial;color:red;font-size:20px;">一个段落。</p>
```

**文本对齐方式**

<h1 style="text-align:center;">居中对齐的标题</h1>

```
<h1 style="text-align:center;">居中对齐的标题</h1>
```

**内部样式表**

当单个文件需要特别样式时，使用内部样式表，可以在head部分通过style标签定义内部样式表。

```
<head>
<style type="text/css">
body {background-color:yellow;}
p {color:blue;}
</style>
</head>
```

外部样式表

当样式需要被应用到很多页面时，可以通过外部样式表更改一个文件来改变整个站点的外观。

```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css"
</head>
```

<table class="reference notranslate">
<tbody><tr>
<th align="left">标签</th>
<th align="left">描述</th>
</tr>
<tr>
<td><a href="/tags/tag-style.html">&lt;style&gt;</a></td>
<td>定义文本样式</td>
</tr>
<tr>
<td><a href="/tags/tag-link.html">&lt;link&gt;</a></td>
<td>定义资源引用地址 </td>
</tr>
</tbody></table>



# 11 HTML图像

**img标签（图像）和Src属性（源属性）**

图像由img定义，空标签，即只包含属性，没有闭合标签。

Src source 源属性的值是图像的URL地址。

```
<img src="url" alt="some_text">
```

**Alt属性**

为图像定义一串预备的可替换文本，在图像无法载入时显示

**width和height属性**

属性值默认单位为像素

```
<img src="pulpit.jpg" alt="Pulpit rock" width="304" height="228">
```

<table class="reference notranslate">
<tbody><tr>
<th align="left">标签</th>
<th align="left">描述</th>
</tr>
<tr>
<td><a href="/tags/tag-img.html">&lt;img&gt;</a></td>
<td>定义图像</td>
</tr>
<tr>
<td><a href="/tags/tag-map.html">&lt;map&gt;</a></td>
<td>定义图像地图</td>
</tr>
<tr>
<td><a href="/tags/tag-area.html">&lt;area&gt;</a></td>
<td>定义图像地图中的可点击区域</td>
</tr>
</tbody></table>

**排列图片**

```
<h4>默认对齐的图像（align="bottom"):</h4>
<p>这是一些文本。<img src="https://www.runoob.com/try/demo_source/smiley.gif" alt="smailey face" width="32" height="32">这是一些文本。</p>

<h4>图片使用align="middle":</h4>
p>这是一些文本。<img src="https://www.runoob.com/try/demo_source/smiley.gif" alt="smailey face" align="middle" width="32" height="32">这是一些文本。</p>

<h4>图片使用align="top":</h4>
p>这是一些文本。<img src="https://www.runoob.com/try/demo_source/smiley.gif" alt="smailey face" align="top" width="32" height="32">这是一些文本。</p>
```

**float属性**

图片在段落左右浮动，已弃用

**area标签**

带有可点击区域的图像映射

```
<img loading="lazy" src="planets.gif" width="145" height="126" alt="Planets" usemap="#planetmap"

<map name="planetmap">
	<area shape="ret" coords="0,0,82,126" alt="Sun" href="sun.htm"
	<area shape="circle" coords="90,58,3" alt="Mercury" href="mercur.htm"
	<area shape="circle" coords="124,58,8" alt="Venus" href="venus.htm"
</map>
```



# 12 HTML表格

由table标签定义，tr标签定义行，td标签定义每行的单元格，td定义单元数据内容，可以包括文本、图片、列表、段落、表单、水平线、表格等等。

<table border="1">
    <tr>
        <td>row 1,cell 1</td>
    	<td>row 2,cell 2</td>
    </tr>
    <tr>
    	<td>row 2,cell 1</td>
    	<td>row 2,cell 2</td>
    </tr>
</table>

```
<table border="1">
    <tr>
        <td>row 1,cell 1</td>
    	<td>row 2,cell 2</td>
    </tr>
    <tr>
    	<td>row 2,cell 1</td>
    	<td>row 2,cell 2</td>
    </tr>
</table>
```



HTML表格和边框属性

border定义边框的粗细

不定义或为0没有边框

<table border="1">     <tr>         <td>Row 1, cell 1</td>         <td>Row 1, cell 2</td>     </tr> </table>



HTML表格表头

th定义 显示为粗体居中的文本

<table>
    <tr>
    	<th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>row 1,cell 1</td>
        <td>row 1,cell 2</td>
    </tr>
    <tr>
    	<td>row 2,cell 1</td>
        <td>row 2,cell 2</td>
    </tr>
</table>

```
<table>
    <tr>
    	<th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>row 1,cell 1</td>
        <td>row 1,cell 2</td>
    </tr>
    <tr>
    	<td>row 2,cell 1</td>
        <td>row 2,cell 2</td>
    </tr>
</table>
```



垂直表头

<h4>垂直表头:</h4>
<table border="1">
<tr>
  <th>First Name:</th>
  <td>Bill Gates</td>
</tr>
<tr>
  <th>Telephone:</th>
  <td>555 77 854</td>
</tr>
<tr>
  <th>Telephone:</th>
  <td>555 77 855</td>
</tr>
</table>

```
<h4>垂直表头:</h4>
<table border="1">
<tr>
  <th>First Name:</th>
  <td>Bill Gates</td>
</tr>
<tr>
  <th>Telephone:</th>
  <td>555 77 854</td>
</tr>
<tr>
  <th>Telephone:</th>
  <td>555 77 855</td>
</tr>
</table>
```

<table border="1">
  <caption>Monthly savings</caption>

```
<table border="1">
  <caption>Monthly savings</caption>
```

caption定义标题

跨行或跨列的表格单元格

<h4>单元格跨两列:</h4>
<table border="1">
<tr>
  <th>Name</th>
  <th colspan="2">Telephone</th>
</tr>
<tr>
  <td>Bill Gates</td>
  <td>555 77 854</td>
  <td>555 77 855</td>
</tr>
</table>

<h4>单元格跨两行:</h4>
<table border="1">
<tr>
  <th>First Name:</th>
  <td>Bill Gates</td>
</tr>
<tr>
  <th rowspan="2">Telephone:</th>
  <td>555 77 854</td>
</tr>
<tr>
  <td>555 77 855</td>
</tr>
</table>

```
<h4>单元格跨两列:</h4>
<table border="1">
<tr>
  <th>Name</th>
  <th colspan="2">Telephone</th>
</tr>
<tr>
  <td>Bill Gates</td>
  <td>555 77 854</td>
  <td>555 77 855</td>
</tr>
</table>

<h4>单元格跨两行:</h4>
<table border="1">
<tr>
  <th>First Name:</th>
  <td>Bill Gates</td>
</tr>
<tr>
  <th rowspan="2">Telephone:</th>
  <td>555 77 854</td>
</tr>
<tr>
  <td>555 77 855</td>
</tr>
</table>
```



表格内的标签

<table border="1">
<tr>
  <td>
   <p>这是一个段落</p>
   <p>这是另一个段落</p>
  </td>
  <td>这个单元格包含一个表格:
   <table border="1">
   <tr>
     <td>A</td>
     <td>B</td>
   </tr>
   <tr>
     <td>C</td>
     <td>D</td>
   </tr>
   </table>
  </td>
</tr>
<tr>
  <td>这个单元格包含一个列表
   <ul>
    <li>apples</li>
    <li>bananas</li>
    <li>pineapples</li>
   </ul>
  </td>
  <td>HELLO</td>
</tr>
</table>

```
<table border="1">
<tr>
  <td>
   <p>这是一个段落</p>
   <p>这是另一个段落</p>
  </td>
  <td>这个单元格包含一个表格:
   <table border="1">
   <tr>
     <td>A</td>
     <td>B</td>
   </tr>
   <tr>
     <td>C</td>
     <td>D</td>
   </tr>
   </table>
  </td>
</tr>
<tr>
  <td>这个单元格包含一个列表
   <ul>
    <li>apples</li>
    <li>bananas</li>
    <li>pineapples</li>
   </ul>
  </td>
  <td>HELLO</td>
</tr>
</table>
```



单元格边距

<h4>没有单元格边距:</h4>
<table border="1">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>有单元格边距:</h4>
<table border="1" 
cellpadding="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

```
<h4>没有单元格边距:</h4>
<table border="1">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>有单元格边距:</h4>
<table border="1" 
cellpadding="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>
```

单元格间距

<h4>没有单元格间距:</h4>
<table border="1">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>单元格间距="0":</h4>
<table border="1" cellspacing="0">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>单元格间距="10":</h4>
<table border="1" cellspacing="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

```
<h4>没有单元格间距:</h4>
<table border="1">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>单元格间距="0":</h4>
<table border="1" cellspacing="0">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>单元格间距="10":</h4>
<table border="1" cellspacing="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>
```



# 13 HTML列表

HTML支持有序、无序和定义列表



HTML有序列表

start定义起始序号

<ol>
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

HTML无序列表

<ul>
<li>Coffee</li>
<li>Milk</li>
</ul>

```
<ul>
<li>Coffee</li>
<li>Milk</li>
</ul>
```



HTML自定义列表

项目term及其注释description的集合

<dl>
    <dt>Coffee</dt>
    <dd>- black hot drink</dd>
    <dt>Milk</dt>
    <dd>- white cold drink</dd>
</dl>

```
<dl>
    <dt>Coffee</dt>
    <dd>- black hot drink</dd>
    <dt>Milk</dt>
    <dd>- white cold drink</dd>
</dl>
```



不同类型的有序列表

type属性定义列表序号形式，如type="A","a","I","i"等

<h4>编号列表：</h4>
<ol>
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>大写字母列表：</h4>
<ol type="A">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>小写字母列表：</h4>
<ol type="a">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>罗马数字列表：</h4>
<ol type="I">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>小写罗马数字列表：</h4>
<ol type="i">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

```
<h4>编号列表：</h4>
<ol>
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>大写字母列表：</h4>
<ol type="A">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>小写字母列表：</h4>
<ol type="a">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>罗马数字列表：</h4>
<ol type="I">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  

<h4>小写罗马数字列表：</h4>
<ol type="i">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ol>  
```



不同类型的无序列表

使用CSS属性style="list-style-type:disc, circle, square"定义圆点圆圈和正方形列表

<h4>圆点列表：</h4>
<ul style="list-style-type:disc">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ul>  

<h4>圆圈列表：</h4>
<ul style="list-style-type:circle">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ul>  

<h4>正方形列表：</h4>
<ul style="list-style-type:square">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ul>

```
<h4>圆点列表：</h4>
<ul style="list-style-type:disc">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ul>  

<h4>圆圈列表：</h4>
<ul style="list-style-type:circle">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ul>  

<h4>正方形列表：</h4>
<ul style="list-style-type:square">
 <li>Apples</li>
 <li>Bananas</li>
 <li>Lemons</li>
 <li>Oranges</li>
</ul>

```



嵌套列表

<h4>嵌套列表：</h4>
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea
        <ul>
          <li>China</li>
          <li>Africa</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>Milk</li>
</ul>

```
<h4>嵌套列表：</h4>
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea
        <ul>
          <li>China</li>
          <li>Africa</li>
        </ul>
      </li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```



# 14 HTML中div和span

HTML区块元素div如h1, p, ul, table等，以新行来开始或结束，组合其他HTML元素的容器

HTML内联元素span如td, a, img等，不会以新行开始，文本的容器

使用div元素布局的网页

<div id="container" style="width:500px">

<div id="header" style="background-color:#FFA500;">
<h1 style="margin-bottom:0;">主要的网页标题</h1></div>

<div id="menu" style="background-color:#FFD700;height:200px;width:100px;float:left;">
<b>菜单</b><br>
HTML<br>
CSS<br>
JavaScript</div>

<div id="content" style="background-color:#EEEEEE;height:200px;width:400px;float:left;">
内容在这里</div>

<div id="footer" style="background-color:#FFA500;clear:both;text-align:center;">
版权 © runoob.com</div>


```
<div id="container" style="width:500px">

<div id="header" style="background-color:#FFA500;">
<h1 style="margin-bottom:0;">主要的网页标题</h1></div>

<div id="menu" style="background-color:#FFD700;height:200px;width:100px;float:left;">
<b>菜单</b><br>
HTML<br>
CSS<br>
JavaScript</div>

<div id="content" style="background-color:#EEEEEE;height:200px;width:400px;float:left;">
内容在这里</div>

<div id="footer" style="background-color:#FFA500;clear:both;text-align:center;">
版权 © runoob.com</div>
```



# 15 HTML表单和输入

HTML表单用于收集不同类型的用户的输入

HTML表单

表单是一个包含表单元素的区域，表单元素允许用户在表单中输入内容，比如文本域（textarea）、下拉列表、单选框（radio-buttons）、复选框（checkboxes）等等。

表单使用标签form设置

输入标签input，输入类型由type定义

文本域（Text Fields）

<form>
    First name: <input type="text" name="firstname"><br>
    Last name: <input type="text" name="lastname"
</form>

```
<form>
    First name: <input type="text" name="firstname"><br>
    Last name: <input type="text" name="lastname"
</form>
```

文本域的默认宽度是20个字符

密码字段

<form>
    Password: <input type="password" name="pwd">
</form>

<form>
    Password: <input type="password" name="pwd">
</form>

密码字段不会明文显示，以星号或圆点代替

单选按钮（Radio Buttons）

<form>
    <input type="radio" name="sex" value="male">Male<br>
    <input type="radio" name="sex" value="female">Female
</form>

```
<form>
    <input type="radio" name="sex" value="male">Male<br>
    <input type="radio" name="sex" value="female">Female
</form>
```

复选框（Checkboxes）

<form>
    <input type="checkbox" name="vehicle" value="Bike">I have a bike<br>
    <input type="checkbox" name="vehicle" value="Car">I have a car
</form>

提交按钮

type="submit"定义了提交按钮

用户单击确认按钮时，表单的内容会被传送到另一个文件。表单的动作属性定义了目的文件的文件名。

<form name="input" action="html_form_action.php" method="get">
    Username: <input type="text" name="user">
    <input type="submit" value="Submit">
</form>

```
<form name="input" action="html_form_action.php" method="get">
    Username: <input type="text" name="user">
    <input type="submit" value="Submit">
</form>
```

简单的下拉列表

<form action="">
    <select name="cars">
        <option value="v01vo">Vo1vo</option>
        <option value="saab">Saab</option>
        <option value="fiat">Fiat</option>
        <option value="audi">Audi</option>
    </select>
</form>

```
<form action="">
    <select name="cars">
        <option value="v01vo">Vo1vo</option>
        <option value="saab">Saab</option>
        <option value="fiat">Fiat</option>
        <option value="audi">Audi</option>
    </select>
</form>
```

预选下拉列表

<form action="">
<select name="cars">
<option value="volvo">Volvo</option>
<option value="saab">Saab</option>
<option value="fiat" selected>Fiat</option>
<option value="audi">Audi</option>
</select>
</form>

```
<form action="">
<select name="cars">
<option value="volvo">Volvo</option>
<option value="saab">Saab</option>
<option value="fiat" selected>Fiat</option>
<option value="audi">Audi</option>
</select>
</form>
```

文本域-多行文本输入控件

<textarea rows="10" cols="30">
    我是一个文本框
</textarea>

```
<textarea rows="10" cols="30">
    我是一个文本框
</textarea>
```

创建按钮

<form action="">
    <input type="button" value="Hello world!">
</form>

```
<form action="">
    <input type="button" value="Hello world!">
</form>
```

带边框的表单

<form action="">
    <fieldset>
        <legend>Personal information:</legend>
        Name: <input type="text" size="30"><br>
        E-mail: <input type="text" size="30"<br>
        Date of birth: <input type="text" size="10">
    </fieldset>
</form>

```
<form action="">
    <fieldset>
        <legend>Personal information:</legend>
        Name: <input type="text" size="30"><br>
        E-mail: <input type="text" size="30"<br>
        Date of birth: <input type="text" size="10">
    </fieldset>
</form>
```

带有输入框和确认按钮的表单

<form action="demo-form.php">
    First name: <input type="text" name="FirstName" value="Mickey"><br>
    Last name: <input type="text" name="LastName" value="Mouse"><br>
    <input type="submit" value="提交">
</form>

```
<form action="demo-form.php">
    First name: <input type="text" name="FirstName" value="Mickey"><br>
    Last name: <input type="text" name="LastName" value="Mouse"><br>
    <input type="submit" value="提交">
</form>
```

从表单发送电子邮件

<form action="MAILTO:someone@example.com" method="post" enctype="text/plain">
Name:<br>
<input type="text" name="name" value="your name"><br>
E-mail:<br>
<input type="text" name="mail" value="your email"><br>
Comment:<br>
<input type="text" name="comment" value="your comment" size="50"><br><br>
<input type="submit" value="发送">
<input type="reset" value="重置">
</form>

```
<form action="MAILTO:someone@example.com" method="post" enctype="text/plain">
Name:<br>
<input type="text" name="name" value="your name"><br>
E-mail:<br>
<input type="text" name="mail" value="your email"><br>
Comment:<br>
<input type="text" name="comment" value="your comment" size="50"><br><br>
<input type="submit" value="发送">
<input type="reset" value="重置">
</form>
```



# 16 HTML框架

使用框架，可以在同一个浏览器中显示不止一个页面

<iframe src="readme.md"></iframe>

```
<iframe src="readme.md"></iframe>
```

高度和宽度

height和width定义高度和宽度

Iframe-移除边框

frameborder="0"

```
<iframe src="demo_iframe.htm" frameborder="0"></iframe>
```

使用iframe来显示目标链接网页

```
<iframe src="demo_iframe.htm" name="iframe_a"></iframe>
<p><a href="http://www.runoob.com" target="iframe_a" rel="noopener">RUNOOB.COM</a></p>
```



# 17 HTML颜色

HTML由红绿蓝混合而成

HTML颜色由一个十六进制符号来定义，由三原色的值组成

最小值为0（#00），最大值为255（#FF）

#000000 rgb(0,0,0)  黑色

#FFFFFF rgb(255,255,255) 白色

1600万色 255×255×255

web安全色

RGBA 的意思是（Red-Green-Blue-Alpha）它是在 RGB 上扩展包括了 **“alpha”** 通道，运行对颜色值设置透明度。

```
div {
background:rgba(255,0,0,0.5);
}
```

相对于使用 rgb(255,255,0)，使用 rgba(255,255,0,0.5) 可以实现设置颜色透明度的功能，这里的 0.5 表示透明度，范围 0~1，0 表示全透明。通常我们为了省略一个 0:

```
div {
    background:rgba(255,0,0,.5);
}
```

<p style="background-color:rgb(255,255,0)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,0.25)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,0.5)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,0.75)">
通过 rbg 值设置背景颜色
</p>

<p style="background-color:rgba(255,255,0,1)">
通过 rbg 值设置背景颜色
</p>

```
<p style="background-color:rgb(255,255,0)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,0.25)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,0.5)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,0.75)">
通过 rbg 值设置背景颜色
</p>
<p style="background-color:rgba(255,255,0,1)">
通过 rbg 值设置背景颜色
</p>
```

HTML颜色名

141个颜色名称是在HTML和CSS颜色规范定义的（17标准颜色，再加124）。下表列出了所有颜色的值，包括十六进制值。

![Remark](https://www.runoob.com/images/lamp.gif) **提示:** 17标准颜色：黑色，蓝色，水，紫红色，灰色，绿色，石灰，栗色，海军，橄榄，橙，紫，红，白，银，蓝绿色，黄色。点击其中一个颜色名称（或一个十六进制值)就可以查看与不同文字颜色搭配的背景颜色。



参考列表：[HTML 颜色 | 菜鸟教程 (runoob.com)](https://www.runoob.com/html/html-colors.html)

# HTML脚本

JavaScript使HTML页面具有更强的动态和交互性

插入一段脚本

<script>
    document.write("Hello World!")
</script>

使用noscript标签

<script>
document.write("Hello World!")
</script>
<noscript>抱歉，你的浏览器不支持 JavaScript!</noscript>

<p>浏览器禁用或不支持 JavaScript 会使用 &lt;noscript&gt; 元素中定义的内容（文本）来替代。</p>

script标签用于定义客户端脚本，比如 JavaScript

script元素既可包含脚本语句，也可通过 src 属性指向外部脚本文件。

JavaScript 最常用于图片操作、表单验证以及内容动态更新。



JavaScript事件响应:

```
<p id="demo">
JavaScript 可以触发事件，就像按钮点击。</p>

<script>
function myFunction()
{
	document.getElementById("demo").innerHTML="Hello JavaScript!";
}
</script>

<button type="button" onclick="myFunction()">点我</button>
```



JavaScript处理 HTML 样式:

```
<p id="demo">
JavaScript 能改变 HTML 元素的样式。
</p>
<script>
function myFunction()
{
	x=document.getElementById("demo") // 找到元素
	x.style.color="#ff0000";          // 改变样式
}
</script>
```



# HTML字符实体

HTML 中的预留字符必须被替换为字符实体。

一些在键盘上找不到的字符也可以使用字符实体来替换。

在 HTML 中，某些字符是预留的。

在 HTML 中不能使用小于号（<）和大于号（>），这是因为浏览器会误认为它们是标签。



如果希望正确地显示预留字符，我们必须在 HTML 源代码中使用字符实体（character entities）。 字符实体类似这样：

&*entity_name*;

或

&#*entity_number*;

如需显示小于号，我们必须这样写：**<** 或 **<** 或 **<**

```
&lt; 或 &#60; 或 &#060;
```



不间断空格(Non-breaking Space)

HTML 中的常用字符实体是不间断空格(&nbsp;)。

浏览器总是会截短 HTML 页面中的空格。如果您在文本中写 10 个空格，在显示该页面之前，浏览器会删除它们中的 9 个。如需在页面中增加空格的数量，您需要使用 &nbsp; 字符实体。



## 结合音标符

发音符号是加到字母上的一个"glyph(字形)"。

一些变音符号, 如 尖音符 ( ̀) 和 抑音符 ( ́) 。

变音符号可以出现字母的上面和下面，或者字母里面，或者两个字母间。

变音符号可以与字母、数字字符的组合来使用。



参考列表：[HTML 字符实体 | 菜鸟教程 (runoob.com)](https://www.runoob.com/html/html-entities.html)

HTML 统一资源定位器（Uniform Resource Locators)

URL是一个网页地址，可以由字母（www.baidu.com）或互联网协议（IP：192.168.1.1）组成。



URL - 统一资源定位器

Web浏览器通过URL从Web服务器请求页面。

当您点击 HTML 页面中的某个链接时，对应的 <a> 标签指向万维网上的一个地址。

一个统一资源定位器(URL) 用于定位万维网上的文档。

一个网页地址实例: http://www.runoob.com/html/html-tutorial.html 语法规则:

```
scheme://host.domain:port/path/filename
```

说明:

- - scheme - 定义因特网服务的类型。最常见的类型是 http
  - host - 定义域主机（http 的默认主机是 www）
  - domain - 定义因特网域名，比如 runoob.com
  - :port - 定义主机上的端口号（http 的默认端口号是 80）
  - path - 定义服务器上的路径（如果省略，则文档必须位于网站的根目录中）。
  - filename - 定义文档/资源的名称



Scheme	访问	用于...
http	超文本传输协议	以 http:// 开头的普通网页。不加密。
https	安全超文本传输协议	安全网页，加密所有信息交换。
ftp	文件传输协议	用于将文件下载或上传至网站。
file	 	您计算机上的文件。



URL 字符编码

URL 只能使用 [ASCII 字符集](https://www.runoob.com/tags/html-ascii.html).

来通过因特网进行发送。由于 URL 常常会包含 ASCII 集合之外的字符，URL 必须转换为有效的 ASCII 格式。

URL 编码使用 "%" 其后跟随两位的十六进制数来替换非 ASCII 字符。

URL 不能包含空格。URL 编码通常使用 + 来替换空格。



# HTML - XHTML

XHTML 是以 XML 格式编写的 HTML。

什么是 XHTML?

- XHTML 指的是可扩展超文本标记语言
- XHTML 与 HTML 4.01 几乎是相同的
- XHTML 是更严格更纯净的 HTML 版本
- XHTML 是以 XML 应用的方式定义的 HTML
- XHTML 是 [2001 年 1 月](https://www.runoob.com/w3c/w3c-xhtml.html)发布的 W3C 推荐标准
- XHTML 得到所有主流浏览器的支持



与 HTML 相比最重要的区别：

文档结构

- XHTML DOCTYPE 是*强制性的*
- <html> 中的 XML namespace 属性是*强制性的*
- <html>、<head>、<title> 以及 <body> 也是*强制性的*

元素语法

- XHTML 元素必须*正确嵌套*
- XHTML 元素必须始终*关闭*
- XHTML 元素必须*小写*
- XHTML 文档必须有*一个根元素*

属性语法

- XHTML 属性必须使用*小写*
- XHTML 属性值必须用*引号包围*
- XHTML 属性最小化也是*禁止的*



参考列表：

[HTML 标签列表(字母排序) | 菜鸟教程 (runoob.com)](https://www.runoob.com/tags/html-reference.html)

[HTML 全局属性 | 菜鸟教程 (runoob.com)](https://www.runoob.com/tags/ref-standardattributes.html)

[HTML 速查列表 | 菜鸟教程 (runoob.com)](https://www.runoob.com/html/html-quicklist.html)

