来源： http://product.pconline.com.cn/itbk/bkxt/1707/9684244.html
# Markdown学习笔记

# 目录
> 1. Markdown是什么？
> 2. 谁创造了它？
> 3. 为什么要使用它？
> 4. 谁在用？
> 5. 怎么使用？
> 6. 尝试一下

# 内容
## 1. Markdown是什么？
Markdown是一种轻量级「**标记语言**」，它的目标是实现「**易读易写**」。  
可以简单理解成为，用markdown语法编写的内容转换成html的「**工具**」。

## 2. 谁创造了它？
它由[**Aaron Swartz**](http://www.aaronsw.com/)和**John Gruber**共同设计。

![Aaron Swartz](https://github.com/chen-s-y/mv20170724/blob/master/2017-10-13-markdown/about-markdown/Aaron%20Swartz.jpg)

**Aaron Swartz**于*2013年1月11日*自杀,有着**开挂**一般人生经历的程序员。维基百科对他的[介绍](http://zh.wikipedia.org/wiki/%E4%BA%9A%E4%BC%A6%C2%B7%E6%96%AF%E6%B2%83%E8%8C%A8)是：**软件工程师、作家、政治组织者、互联网活动家、维基百科人**。    

![John Gruber](https://github.com/chen-s-y/mv20170724/blob/master/2017-10-13-markdown/about-markdown/John%20Gruber.jpg)

**John Gruber**，知名独立博主，Markdown创始人，UI设计师，苹果狂热粉。相比于Markdown创始人这个头衔，Gruber更出名的是对苹果的狂热，和由狂热外化出来的[Daring Fireball](https://daringfireball.net/)博客（一个每年可以赚取 50 万美元的博客）。博客上还提供下载一些由 Gruber 自己开发的软件。最初 Gruber 只是利用空闲时间打理，但从 2006 年 4 月开始，运作这个博客成了 Gruber 的全职工作，并通过收取会费、投放广告、售卖 T 恤等方式获得收入。

## 3. 为什么要使用它？
+ 它是易读（看起开舒服）、易写（语法简单）、易更改**纯文本**。处处体现着**极简主义**的影子。
+ 兼容HTML，可以转换为HTML格式发布。
+ 跨平台使用。
+ 越来越多的网站支持Markdown。
+ 更方便清晰的组织你的电子邮件。（Markdown-here, Airmail）
+ 摆脱Word（我不是认真的）。

## 4. 谁在用？
Markdown的使用者：
+ GitHub
+ 简书
+ Stack Overflow
+ Apollo
+ Moodle
+ Reddit
+ gitee
+ coding
+ 公司内部文档，等等

## 5. 怎么使用？
- 标题
- 加粗，斜体，高亮
- 段落
- 列表
- 图片，链接
- 引用
- 代码
- 代码区块
- 表格

### 标题
使用`#` 可表示1-6级标题, 即：
``` bash
    # 一级标题
    ## 二级标题
    ### 三级标题
    #### 四级标题
    ##### 五级标题
    ###### 六级标题
```
效果：
> # 一级标题   
> ## 二级标题   
> ### 三级标题   
> #### 四级标题   
> ##### 五级标题   
> ###### 六级标题

### 斜体，加粗
```
    *斜体*, 或 _斜体_
    **加粗**, 或 __加粗__
    ~~删除线~~
```
效果：
> *斜体* 或 _斜体_  
> **加粗** 或 __加粗__  
> ~~删除线~~

### 段落
段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用**两个以上**空格加上回车（引用中换行省略回车）。

### 列表
使用`+`、或`-`标记无序列表，使用`1.`数字标记有序列表，如：
``` bash
    1. 第一节
        + 第一节第一课
        + 第一节第二课
    2. 第二节
    3. 第三节
        - 第三节第一课
        - 第三节第二课
        - 第三节第三课
            - 第三节第三课第一段
            - 第三节第三课第二段
    4. 第四节
    5. 第五节
```
效果：  
1. 第一节
    + 第一节第一课
    + 第一节第二课
2. 第二节
3. 第三节
    - 第三节第一课
    - 第三节第二课
    - 第三节第三课
        - 第三节第三课第一段
        - 第三节第三课第二段
4. 第四节
5. 第五节

### 图片，链接
+ 链接语法：[]()
+ 图片语法：![]()

``` bash
    [百度](http://www.baidu.com/ "链接描述(可省略)")  
    \![图片描述](http://dcs.conac.cn/image/red.png "描述(可省略)")
```
效果：
> 链接: [百度](http://www.baidu.com/ "百度")  
> 图片: ![党政机关](http://dcs.conac.cn/image/red.png "党政机关")

高级用法
``` bash
    [**链接**][null-link]
    [*有效链接*][csy-link]
    I get 10times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].

    注意： 链接必须另起一行(即：不能在同一个段落中)
    [csy-link]: http://www.baidu.com/ "鼠标滑入的时候, 显示该字段"
    [null-link]: chrome://not-a-link
    [1]: http://google.com/        "Google"
    [2]: http://search.yahoo.com/  "Yahoo Search"
    [3]: http://search.msn.com/    "MSN Search"

    ![Alt text][id]
    [id]: url/to/image  "Optional title attribute"

    ![](http://img3.douban.com/mpic/s1108264.jpg "title text")
```
效果：
> [**无效链接**][null-link]  
> [*有效链接*][csy-link]  
> I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].  
>
> [null-link]: chrome://not-a-link
> [csy-link]: http://baidu.com/ "鼠标滑入的时候, 显示该字段"
> [1]: http://google.com/        "Google"
> [2]: http://search.yahoo.com/  "Yahoo Search"
> [3]: http://search.msn.com/    "MSN Search"
> 注意： 链接必须另起一行(即：不能在同一个段落中)

### 引用
使用 > 符号，进行引用
``` bash
    > This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
    consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
    Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

    > 
    > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
    > id sem consectetuer libero luctus adipiscing.
    > > id sem consectetuer libero luctus adipiscing.
```
效果：
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
> > id sem consectetuer libero luctus adipiscing.

### 代码
如果要标记一小段行内代码，你可以用 ` 反引号把它包起来，例如：
``` bash
    Use the `printf()` function.
```
效果：
> Use the `printf()` function.

### 代码区块
代码块就是将源码直接进行展示，可在开始的 ``` 后面加上代码语种名称
``` javascript
    var str = "hello world!";
    alert(str);
```

### 表格
用`|`表示表格纵向边界，表头和内容用`-`隔开，用`:`进行对齐设置，两边都有表示居中，默认左对齐。

学号 | 姓名 | 成绩
---: | :--- | :---:
001 | 张三 | 60
02 | 阿尔及利亚 | 898998






## 6. 尝试一下
+ **Chrome**下的插件诸如`stackedit`与`markdown-here`等非常方便，也不用担心平台受限。
+ **在线**的dillinger.io评价也不错   
+ **Windowns**下的MarkdownPad也用过，不过免费版的体验不是很好。    
+ **Mac**下的Mou是国人贡献的，口碑很好。
+ **Linux**下的ReText不错。   


*********************************************************
# Markdown 免费编辑器

Windows 平台

- [GitHub Atom][11]
- [MarkdownPad][12]
- [MarkPad][13]

Linux 平台

- [ReText][14]

Mac 平台

- [Mou][15]

在线编辑器

- [Markable.in][16]
- [Dillinger.io][17]

浏览器插件

- [MaDe][18] (Chrome)

高级应用(Sublime Text 2 + MarkdownEditing 教程)

- [Sublime Text 2][19]
- [MarkdownEditing][20]
- [教程][21]

[11]: https://atom.io/
[12]: http://markdownpad.com/
[13]: http://code52.org/DownmarkerWPF/
[14]: http://sourceforge.net/p/retext/home/ReText/
[15]: http://mouapp.com/
[16]: http://markable.in/
[17]: http://dillinger.io/
[18]: https://chrome.google.com/webstore/detail/oknndfeeopgpibecfjljjfanledpbkog
[19]: http://www.sublimetext.com/2
[20]: http://ttscoff.github.com/MarkdownEditing/
[21]: http://lucifr.com/2012/07/12/markdownediting-for-sublime-text-2/










## 主要内容
> #### Markdown*是什么*？
> #### *谁*创造了它？
> #### *为什么*要使用它？
> #### *怎么*使用？
> #### *谁*在用？
> #### 尝试一下

## 正文
### 1. Markdown*是什么*？
**Markdown**是一种轻量级**标记语言**，它以纯文本形式(*易读、易写、易更改*)编写文档，并最终以HTML格式发布。    
**Markdown**也可以理解为将以MARKDOWN语法编写的语言转换成HTML内容的工具。    

### 2. *谁*创造了它？
它由[**Aaron Swartz**](http://www.aaronsw.com/)和**John Gruber**共同设计，**Aaron Swartz**就是那位于去年（*2013年1月11日*）自杀,有着**开挂**一般人生经历的程序员。维基百科对他的[介绍](http://zh.wikipedia.org/wiki/%E4%BA%9A%E4%BC%A6%C2%B7%E6%96%AF%E6%B2%83%E8%8C%A8)是：**软件工程师、作家、政治组织者、互联网活动家、维基百科人**。    

他有着足以让你跪拜的人生经历：    
+ **14岁**参与RSS 1.0规格标准的制订。     
+ **2004**年入读**斯坦福**，之后退学。   
+ **2005**年创建[Infogami](http://infogami.org/)，之后与[Reddit](http://www.reddit.com/)合并成为其合伙人。   
+ **2010**年创立求进会（Demand Progress），积极参与禁止网络盗版法案（SOPA）活动，最终该提案被撤回。   
+ **2011**年7月19日，因被控从MIT和JSTOR下载480万篇学术论文并以免费形式上传于网络被捕。     
+ **2013**年1月自杀身亡。    

![Aaron Swartz](https://github.com/younghz/Markdown/raw/master/resource/Aaron_Swartz.jpg)

天才都有早逝的归途。

### 3. *为什么*要使用它？
+ 它是易读（看起开舒服）、易写（语法简单）、易更改**纯文本**。处处体现着**极简主义**的影子。
+ 兼容HTML，可以转换为HTML格式发布。
+ 跨平台使用。
+ 越来越多的网站支持Markdown。
+ 更方便清晰的组织你的电子邮件。（Markdown-here, Airmail）
+ 摆脱Word（我不是认真的）。

### 4. *怎么*使用？
如果不算**扩展**，Markdown的语法绝对**简单**到让你爱不释手。

Markdown语法主要分为如下几大部分：
**标题**，**段落**，**区块引用**，**代码区块**，**强调**，**列表**，**分割线**，**链接**，**图片**，**反斜杠 `\`**，**符号'`'**。

#### 4.1 标题
两种形式：  
1）使用`=`和`-`标记一级和二级标题。
> 一级标题   
> `=========`   
> 二级标题    
> `---------`

效果：
> 一级标题   
> =========   
> 二级标题
> ---------  

2）使用`#`，可表示1-6级标题。
> \# 一级标题   
> \## 二级标题   
> \### 三级标题   
> \#### 四级标题   
> \##### 五级标题   
> \###### 六级标题    

效果：
> # 一级标题   
> ## 二级标题   
> ### 三级标题   
> #### 四级标题   
> ##### 五级标题   
> ###### 六级标题

#### 4.2 段落
段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用**两个以上**空格加上回车（引用中换行省略回车）。

#### 4.3 区块引用
在段落的每行或者只在第一行使用符号`>`,还可使用多个嵌套引用，如：
> \> 区块引用  
> \>> 嵌套引用  

效果：
> 区块引用  
>> 嵌套引用

#### 4.4 代码区块
代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）。如    
普通段落：

void main()    
{    
    printf("Hello, Markdown.");    
}    

代码区块：

    void main()
    {
        printf("Hello, Markdown.");
    }

**注意**:需要和普通段落之间存在空行。

#### 4.5 强调
在强调内容两侧分别加上`*`或者`_`，如：
> \*斜体\*，\_斜体\_    
> \*\*粗体\*\*，\_\_粗体\_\_

效果：
> *斜体*，_斜体_    
> **粗体**，__粗体__

#### 4.6 列表
使用`·`、`+`、或`-`标记无序列表，如：
> \-（+\*） 第一项
> \-（+\*） 第二项
> \- （+\*）第三项

**注意**：标记后面最少有一个_空格_或_制表符_。若不在引用区块中，必须和前方段落之间存在空行。

效果：
> + 第一项
> + 第二项
> + 第三项

有序列表的标记方式是将上述的符号换成数字,并辅以`.`，如：
> 1 . 第一项   
> 2 . 第二项    
> 3 . 第三项    

效果：
> 1. 第一项
> 2. 第二项
> 3. 第三项

#### 4.7 分割线
分割线最常使用就是三个或以上`*`，还可以使用`-`和`_`。

#### 4.8 链接
链接可以由两种形式生成：**行内式**和**参考式**。    
**行内式**：
> \[younghz的Markdown库\]\(https:://github.com/younghz/Markdown "Markdown"\)。

效果：
> [younghz的Markdown库](https:://github.com/younghz/Markdown "Markdown")。

**参考式**：
> \[younghz的Markdown库1\]\[1\]    
> \[younghz的Markdown库2\]\[2\]    
> \[1\]:https:://github.com/younghz/Markdown "Markdown"    
> \[2\]:https:://github.com/younghz/Markdown "Markdown"    

效果：
> [younghz的Markdown库1][1]    
> [younghz的Markdown库2][2]

[1]: https:://github.com/younghz/Markdown "Markdown"
[2]: https:://github.com/younghz/Markdown "Markdown"

**注意**：上述的`[1]:https:://github.com/younghz/Markdown "Markdown"`不出现在区块中。

#### 4.9 图片
添加图片的形式和链接相似，只需在链接的基础上前方加一个`！`。
#### 4.10 反斜杠`\`
相当于**反转义**作用。使符号成为普通符号。
#### 4.11 符号'`'
起到标记作用。如：
>\`ctrl+a\`

效果：
>`ctrl+a`    

#### 5. *谁*在用？
Markdown的使用者：
+ GitHub
+ 简书
+ Stack Overflow
+ Apollo
+ Moodle
+ Reddit
+ 等等

#### 6. 尝试一下
+ **Chrome**下的插件诸如`stackedit`与`markdown-here`等非常方便，也不用担心平台受限。
+ **在线**的dillinger.io评价也不错   
+ **Windowns**下的MarkdownPad也用过，不过免费版的体验不是很好。    
+ **Mac**下的Mou是国人贡献的，口碑很好。
+ **Linux**下的ReText不错。    

**当然，最终境界永远都是笔下是语法，心中格式化 :)。**

****
**注意**：不同的Markdown解释器或工具对相应语法（扩展语法）的解释效果不尽相同，具体可参见工具的使用说明。
虽然有人想出面搞一个所谓的标准化的Markdown，[没想到还惹怒了健在的创始人John Gruber]
(http://blog.codinghorror.com/standard-markdown-is-now-common-markdown/)。
****
以上基本是所有traditonal markdown的语法。

### 其它：
列表的使用(非traditonal markdown)：

用`|`表示表格纵向边界，表头和表内容用`-`隔开，并可用`:`进行对齐设置，两边都有`:`则表示居中，若不加`:`则默认左对齐。

|代码库                              |链接                                |
|:------------------------------------:|------------------------------------|
|MarkDown                              |[https://github.com/younghz/Markdown](https://github.com/younghz/Markdown "Markdown")|
|MarkDownCopy                              |[https://github.com/younghz/Markdown](https://github.com/younghz/Markdown "Markdown")|


关于其它扩展语法可参见具体工具的使用说明。
