---
title: "HTML答卷"
date: 2020-01-01T09:22:54+08:00
draft: false
---

# HTML答卷
## 首先要知道HTML的发明者叫Berners-Lee，他写了第一个浏览器、第一个服务器同时还发明了www（万维网），再深层一点就需要知道HTML的起手式以及全局属性、默认样式、基本的章节标签和内容标签。

## HTML的起手式：  ![](/static/1.png)   
        (我感觉用这张图可以很轻松的理解)

## 章节标签：表示文章/书的层级
    标题h1~h6  段落p 主要内容main 章节section 头部header 旁支内容aside
    文章article 脚部footer 划分div
* 标题h1~h6：文章的标题均是加粗加，只不过字体逐级递减
* 头部header：可以实现在文章最上面做个广告
* 脚部footer：和header相反，可以在最下面做个广告或者版权说明（版权标志：&copy;=圆圈里面套个C）
* 章节section：标题之后可以用标签section，section标签中还可以继续用section但是注意最后都要闭合
* 段落p：可以一段话
* 主要内容main：用于body标签之内（不包括头部后脚部）p标签也在main标签之内，p标签可能只是一部分而main标签就是所有p标签的组合体（不知道该怎么表达了，反正是懂的）
* 旁支内容aside：在main标签之外
* 划分div：在div标签之内的内容就是一个整体，标题h1~h6、章节section、主要内容main和旁支内容aside都在div标签中但不包括header标签和footer标签
## 全局属性（任何一个标签都可以有这个属性）
    class  contenteditable   hidden   id    style    tabindex     title 
* class为章节标签分类 语法： div class="111"  大括号class=111然后中括号背景：颜色;  文字：颜色;   (英文打起来费劲用中文代替，而且还好懂)
* contenteditable: 可以实现让用户直接编辑页面上的文字也可以做一个自己的编辑器（任何一个元素都可以被编辑）
* style:每一个style可以写一个style属性。如果在css中和style（HTML属性）都写了会优先显示后者，如果在JS中也有那么会依JS为准（JS会覆盖HTML）
* id：说实话听的有点懵圈圈，按照目前的实力还是用calss吧，有两个作用第一个在CSS中加#会加样式第二个在JS里面直接通过id获取对应元素
* hidden：可以让你什么也看不见  语法：div hidden..... 意思就是div里面的内容就看不见了
* tabindex：写在标题、内容、最后或者各个部分的标签中（控制tab的顺序）鼠标坏了可以用tab键替代。tabindex等于0时代表顺序是最后一个，tabindex等于-1时代表不要到这里来
* title：当行文字溢出时可以用title。
  
## 默认样式
* 查看默认样式：右键打开开发者工具
* 更改默认样式：CSS reset （进入大厂首页开发者工具找到类似代码复制到自己的项目中命名为reset.css）


## 内容标签：
        ol+li    ul=li    dl+dt+dd   pre   hr   br   a   em   strong   code   quote   blockquote
* ol+li:有序列表   ul+li:无序列表
* dl+dt+dd:用来描述列表  描述事物之后加dl+dt+dd dt之后接主人公  dd之后接对事物的描述内容
* pre：可以保留多个空格 语法： h1  pre标题/pre /h1 就可以保留标题这段内容中的多个空格
* code：被包含的内容是等宽的（所有的字都是等宽的）
* hr： 水平中界线
* br:换行
* a:一般包裹网页链接 语法： a herf=引号+网页链接 >qq /a 会在当前网页打开。如果在引号+网页链接之后加上target=引号_blank会重新打开一个网页
* em:表示强调  语法:em强调词em  em语气很重要
* strong:表示强调 举例：strong强调词strong  strong本身很重要 
* qutoe:表示引用 语法：qutoe 三上 马上 厕上 枕上 /qutoe    代表的是不换行，内联
* blockqutoe：也表示引用  语法：blockqutoe 三上 马上 厕上 枕上 /blockqutoe  代表的意思是块级引用，换行