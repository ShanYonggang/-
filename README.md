# 零基础学院学习内容
目前是一个上班族，工作中接触了python数据分析，需要用到爬虫，所有简单的了解了一下前端知识，后来发现前端能实现各种意向不到的 视觉效果，所有想学习前端知识，最终可以写出一个属于自己的网站，正好看到百度前端学院有如此好的课程，所有来学习下，希望可以坚 持
到底。

### 第一堂课 2019/7/18

##### 一些闲话
今天是学习的第一天，其实以前也多少学习了HTML、CSS、JSP等相关知识，不过都是现学现差，也一直学习JAVASCRIPT知识，最近有脑袋发 热，想重新学习一遍前端的基础知识，正好看到百度前端学院的这个课程。今天学习的内容已经写入百度前端学院LESSON_1.HTML中,具体如下:
- **前端简单介绍:**
1. html:类似于人体的骨架
2. css:类似于人穿的衣服
3. javscript:类似于人所采取的某个动作
4. sql:用于存储数据，类似于存储东西的仓库
5. python、php、java:用于前端与数据库交互的后端语言
6. 客户端（前台用户看到的）、服务端（存储数据、数据查找）
- **日期，学习的总用时，学习目标是什么，是否达成**
- **哪些东西今天了解的比较透彻，说说自己的理解**
- **哪些东西今天了解到了一些，还有哪些点需要后续继续深入阅读**
- **哪些东西今天学了之后还有很多疑问没被解答，记录下来**
##### 第一课作业 FLAG
66天的学习时间，说长也长，说短也短，基于以前学习的一些内容，希望自己可以提前完成此课程

------------
### 第二堂课 2019/7/19

随便写了个个人简历，没有加任何样式，具体代码参见github上的百度前端学院lesson_2.html
本堂课主要学习了html相关知识，针对问题做如下解答：
- **HTML是什么，HTML5是什么** 

1. html: 超文本标记语言，使用html标签描述网页
1. html5: HTML、XHTML 以及 HTML DOM 的新标准，由W3C与WHATWG合作制定
- **TML元素标签、属性都是什么概念？** 

HTML页面是由标签组成的，标签包围的是HTML元素，每个标签拥有自己的属性
- **文档类型是什么概念，起什么作用** 

DOCTYPE，表明web制作过程中用的HTML或XHTML类型，用来提示浏览器或其他阅读程序按照什么规则集去解释文档标记。
- **链接是什么概念，对应什么标签？** 

链接可以实现网页的跳转，对应的标签为 a 标签
- **ol, ul, li, dl, dd, dt等这些标签都适合用在什么地方，举个例子？** 

列表标签，例如网页导航；在文档要分层的时候，像这个READNE用HTML表现就会用到。
- **meta标签都用来做什么？** 

提供页面的元信息，通过‘name、content’属性给页面添加关键词啊，表明作者，页面简介等；还可以通过这个属性设置自适应屏幕
‘http-equiv、content’属性指示传送给服务器的文档头部信息。
- **常用标签都有哪些，都适合用在什么场景？** 

一般用的多的： 
布局划分：header,section,div,nav,footer 
文档格式：h1-h6,p,a,span 
有序列表、无序列表、自定义列表：ul,ol,li,dl,dt,dd 
表格：table,tr,th,td 
- **表单标签都有哪些，对应着什么功能，都有哪些属性？** 

表单form里的标签，input，select/option，textarea； 
input通过type值来调整功能（文本框，密码框，单选/多选按钮，图片按钮...）
select是下拉列表，option是列表值 
textarea文本域，rows,cols属性值决定大小；
最多的表单标签属性还是name,value用来与js编码或后台交互。
- **Web语义化是什么，是为了解决什么问题？** 

web语义化是为了让计算机更了解人类，通过新的html标准让计算机更快速的实现网页的解析

------------
### 第三堂课 2019/7/19
##### 第一部分：css设置字体
 - 每个人在设计网页时需要确定网页所使用的字体：用**font-family**属性设置，通常我们可用字体栈的形式进行设置，确保字体在相应浏览器中的可用性，具体代码如下：
```
p {
  font-family: "Trebuchet MS", Verdana, sans-serif;
}
```
 - 解释下**font-size**中**em**的含义：1em 等于我们设计的当前元素的父元素上设置的字体大小
 - 四个改变文本样子的属性：
	 - **font-style**：normal(普通)、italic(斜体)
	 - **font-weight**：bold、light、lighter、bolder
	 - **text-decoration**：none、underline、overline
	 - **text-transform**：none、uppercase、lowercase、capitalize:（其首字母大写）、full-width:（将所有字形转换成固定宽度的正方形）
##### 第二部分：不常用的css属性
 - 文本阴影：**text-shadow**
 - 文本缩进：**text-indent**属性
 - 字间隔：**word-spacing**属性：改变单词之间的间隔，**letter-spacing**属性：改变字母之间的间距
 - @-规则(At-rules)在CSS中被用来传递元数据、条件信息或其它描述性信息。它由（@）符号开始，紧跟着一个表明它是哪种规则的描述符
 - 嵌套语句 是@-规则中的一种，它的语法是 CSS 规则的嵌套块，只有在特定条件匹配时才会应用到文档上。例如 **@media** ：
```
@media (min-width: 801px) {
  body {
    margin: 0 auto;
    width: 800px;
  }
}
```
只有当页面宽度超过801px时候才会应用body属性。
##### 第三部分：css选择器问题
 - **选择器作用**：定位网页html元素位置
 - **简单选择器**：元素选择器、类选择器、ID选择器、通用选择器（*）、
 - **属性选择器**：[attr]（包含attr属性的）、[attr=value]（attr属性为value）、 [attr~=value] (包含value知)
 - **伪正则选择器**：[attr|=val] 、[attr^=val]、[attr$=val]、[attr*=val]
##### 第四部分：补充部分
 - css工作原理：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190719155837192.PNG?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mjk2NDYxMA==,size_16,color_FFFFFF,t_70)
 - 字体图标（类似于下图中的图标显示）：
![图标](https://img-blog.csdnimg.cn/20190719154839982.PNG) 
此处提供一个 [Font Awesome](http://www.fontawesome.com.cn/faicons/) ，在设计网页时可以直接引用`<link href="//netdna.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">`，然后通过css修改其样式。



