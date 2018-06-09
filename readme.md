# Hello Markdown
## 我应该不只是会个标题那么简单
## 接下来抄写markdown 快速入门
### ……开头表示后期要修改的段落。（已修改）
## Getting the Gist of Markdown's Formatting Syntax
此页提供了Markdown的简单概念，[语法说明页](https://www.appinn.com/markdown/index.html "markdowm syntax")提供了完整详细的文档，说明了每项功能。

## 段落、标题、区块代码
一个段落是由一个以上的连接的行句组成，而一个以上的空行则会划分出不同的段落（空行的定义是显示上看起来像空行，就被视为空行，例如一行只有空白和tab，那么该行也会被视为空行），一般的段落不需要空白或换行缩进。

Markdown支持两种标题的语法，Setext 和 atx 形式。Setext 形式是用底线的形式，利用= （最高阶标题）和- （第二阶标题），Atx形式在行首插入1到6个`#`，对应1到6阶。

**区块引用**则使用email形式的 `>`角括号。

Markwown 语法：
以下是区块引用和标题组合
> A First Level Header
> ===
> A Second Level Header
> -
> ### Header 3
## 修辞和强调
Markdown 使用星号和底线来标记需要强调的区段

Markwown 语法：
> 这些话中有被 *强调* 的词语。
> 
> Some of these words _are emphasized also_.
>
> 这一句中有**更强的强调**。（星号asterisk）
>
>Or, if u prefer, __usr two underscores instead__.
## 分隔线

你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：

* * *

***

*****

- - -

-----------


## 列表
无序列使用*，+和-来作为列表的项目标记，这些符号都是可以使用的。
>* Candy
>+ Gum
>- Booze

有序的列表则是使用一般的数字接着一个英文句点作为项目标记：
>1. Red
>2. Green
>3. Blue

如果你在项目之间插入空行，那项目的内容会用< p>包起来，你也可以在一个项目内放上多个段落，只要在它前面缩排4个空白或一个tab。
>* A list item.
><p With multiple paragraphs.>
>
>* Another item in the list.

## 链接
Markdown 支持两种形式的链接语法： **行内**和**参考**两种形式，两种都是使用角括号来把文字转化为链接。

**行内形式**是直接在后面用括号直接接上链接:
> This is an [example link](http://baidu.com "baidu").

**参考形式**的链接让你可以为链接定一个名称（随便，但为了理解也不能任性），之后你可以在文件的其他地方定义该链接的内容（注意换行）：
>My favorite  websites: [Qzone][qzone]and [Baidu][2]. 
>
>[qzone]: https://user.qzone.qq.com/1179855517/ "qq空间"
>[2]:www.baidu.com "baidu"

## 图片
图片的语法和链接很像。

**行内形式**（title是选择性的，括号要有）：

 ![董香](C:\Users\wssysh\Pictures\Screenshots\董香.png "董香")

**参考形式**：

>![alt text][id]
>
>[id]: C:\Users\wssysh\Pictures\lovewallpaper\test68 "Title"

## 代码
在一般的段落文字中，你可以使用反引号` 来标记代码区段，区段内的&、<和>都会被自动地转换为html实体，这项特性很容易地在在代码区段内插入html码：

I strongly recommend against using any `<blink>` tags.

I wish SmartyPants used named entities like `&mdash;`
instead of decimal-encoded entites like `&#8212;`.

如果要建立一个已经格式化好的代码区块，只要每行都缩进 4 个空格或是一个 tab 就可以了，而 &、< 和 > 也一样会自动转成 HTML 实体。

Markdown 语法:

If you want your page to validate under XHTML 1.0 Strict,
you've got to put paragraph tags in your blockquotes:

<blockquote>
<p>For example.</p>
</blockquote>
