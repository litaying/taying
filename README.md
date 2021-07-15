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

br标签

在不产生新段落的情况下换行

浏览器在显示页面时会移除多余的空格和空行，所有连续的空格和空行会被算作一个

# 7 HTML文本格式化

文本格式化

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

实例演示：

<b>This text is bold.</b>
<strong>This text is strong.</strong>
<big>This text is big.</big>
<em>This text is emphasis.</em>
<i>This test is italic.</i>

<small>This test is small.</small>
This test includes<sup>subscript.</sup>
This test includes<sub>supscript.</sub>

预格式文本

```
<pre>
This example demonstrates how to use the pre tag
to control
blank lines and space.
</pre>
```

Example demonstration:

<pre>
This example demonstrates how to use the pre tag
to control
blank lines and space.
</pre>
计算机输出标签

```
<code>computer output</ceode>
<kbd>keyboard input</kbd>
<tt>teletype text</tt>
<samp>computer code sample</samp>
<var>computer variable</var>
<b>These tags are often used to display computer/programming code.</b>
```

Example demonstration:

<code>computer output</ceode>
<kbd>keyboard input</kbd>
<tt>teletype text</tt>
<samp>computer code sample</samp>
<var>computer variable</var>
<b>These tags are often used to display computer/programming code.</b>

address:

```
<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br/>
Visit us at:<br/>
Example.com<br/>
Box 564,Disneyland<br/>
USA
</address>
```

Example demostration:

<address>
Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br/>
Visit us at:<br/>
Example.com<br/>
Box 564,Disneyland<br/>
USA
</address>

Abbreviations and aronyms 缩写和首字母缩写

```
<abbr title="etcetera">etc.</abbr>
<acronym title="World Wide Web">WWW</acronym>
```

Example demostration:

<abbr title="etcetera">etc.</abbr>

<acronym title="World Wide Web">WWW</acronym>

BiDirectional Override 文字方向（双向覆盖文本的方向）

rtl right to left

ltr left to right

```
<p>This paragraph text displayed from left to right.</p>
<p><bdo dir=rtl>This paragraph text displayed from right to left.</bdo><p>
```

Example demostration:

<p>This paragraph text displayed from left to right.</p>
<p><bdo dir=rtl>This paragraph text displayed from right to left.</bdo><p>

block quote 块引用

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

HTML citations

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

target attributes

target 定义被链接文档显示位置

_blank 在新窗口打开

```
<a href="http://www.baidu.com" target="_blank">visit runoob</a>
```

<a href="http://www.baidu.com" target="_blank">visit runoob</a>

Picture link

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










































参考文件：

[HTML 标签列表(字母排序) | 菜鸟教程 (runoob.com)](https://www.runoob.com/tags/html-reference.html)

[HTML 全局属性 | 菜鸟教程 (runoob.com)](https://www.runoob.com/tags/ref-standardattributes.html)

<p><a id="T1">here</a></p>

