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
