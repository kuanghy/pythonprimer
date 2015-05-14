## 1.  概述
Python由Guido van Rossum于1989年底发明，第一个公开发行版发行于1991年。Python是一种解释型、面向对象、动态数据类型的高级程序设计语言。Python是一种少有的可以称得上是即简单又功能强大的编程语言。
<br />
####简介
Python语言的语法结构非常简单，适合初学者，Python是一个高层次的结合了解释性、编译性、互动性和面向对象的脚本语言。它支持广泛的应用程序开发，从简单的文字处理到 WWW 浏览器再到游戏。Python的官方简介：
> Python是一种简单易学，功能强大的编程语言，它有高效率的高层数据结构，简单而有效地实现面向对象编程。Python简洁的语法和对动态输入的支持，再加上解释性语言的本质，使得它在大多数平台上的许多领域都是一个理想的脚本语言，特别适用于快速的应用程序开发。

**Python语言特点：**

* 易于学习：Python有相对较少的关键字，结构简单，和一个明确定义的语法，学习起来更加简单。

 * 易于阅读：Python代码定义的更清晰。

* 易于维护：Python的成功在于它的源代码是相当容易维护的。

 * 一个广泛的标准库：Python的最大的优势之一是丰富的库，跨平台的，在UNIX，Windows和Macintosh兼容很好。

* 互动模式：互动模式的支持，您可以从终端输入并获得结果的语言，互动的测试和调试代码片断。

* 便携式：Python可以运行在多种硬件平台和所有平台上都具有相同的接口。

* 可扩展：可以添加低层次的模块到Python解释器。这些模块使程序员可以添加或定制自己的工具，更有效。

* 数据库：Python提供所有主要的商业数据库的接口。

* GUI编程：Python支持GUI可以创建和移植到许多系统调用。

* 可扩展性：相比 shell 脚本，Python 提供了一个更好的结构，且支持大型程序。

**Python设计的定位:**

Python的设计哲学是“优雅”、“明确”、“简单”。因此，Perl语言中“总是有多种方法来做同一件事”的理 念在Python开发者中通常是难以忍受的。Python开发者的哲学是“用一种方法，最好是只有一种方法来做一件事”。在设计Python语言时，如果 面临多种选择，Python开发者一般会拒绝花俏的语法，而选择明确的没有或者很少有歧义的语法。由于这种设计观念的差异，Python源代码通常被认为 比Perl具备更好的可读性，并且能够支撑大规模的软件开发。这些准则被称为Python格言。在Python解释器内运行import this可以获得完整的列表。

Python开发人员尽量避开不成熟或者不重要的优化。一些针对非重要部位的加快运行速度的补丁通常不会被合并到 Python内。所以很多人认为Python很慢。不过，根据二八定律，大多数程序对速度要求不高。在某些对运行速度要求很高的情况，Python设计师 倾向于使用JIT技术，或者用使用C/C++语言改写这部分程序。可用的JIT技术是PyPy。

Python是完全面向对象的语言。函数、模块、数字、字符串都是对象。并且完全支持继承、重载、派生、多继承，有益于增强源代码的复用性。Python支持重载运算符和动态类型。相对于Lisp这种传统的函数式编程语言，Python对函数式设计只提供了有限的支持。有两个标准库(functools, itertools)提供了Haskell和Standard ML中久经考验的函数式程序设计工具。

虽然Python可能被粗略地分类为“脚本语言”（script language），但实际上一些大规模软件开发计划例如Zope、Mnet及BitTorrent，Google也广泛地使用它。Python的支持者较喜欢称它为一种高级动态编程语言，原因是“脚本语言”泛指仅作简单程序设计任务的语言，如shellscript、VBScript等只能处理简单任务的编程语言，并不能与Python相提并论。

Python本身被设计为可扩充的。并非所有的特性和功能都集成到语言核心。Python提供了丰富的API和 工具，以便程序员能够轻松地使用C语言、C++、Cython来编写扩充模块。Python编译器本身也可以被集成到其它需要脚本语言的程序内。因此，很 多人还把Python作为一种“胶水语言”（glue language）使用。使用Python将其他语言编写的程序进行集成和封装。在Google内部的很多项目，例如Google Engine使用C++编写性能要求极高的部分，然后用Python或Java/Go调用相应的模块。《Python技术手册》的作者马特利（Alex Martelli）说：“这很难讲，不过，2004 年，Python 已在 Google 内部使用，Google 召募许多 Python 高手，但在这之前就已决定使用Python，他们的目的是 Python where we can, C++ where we must，在操控硬件的场合使用 C++，在快速开发时候使用 Python。”
<br />
####语句
如果在阅读本文之前你接触过编程，那么你大概应该知道，我们学习一门编程语言的入门程序通常是“Hello World”。那我我们就从“Hello World”开始吧。
```python
#!/usr/bin/python
# Filename : helloworld.py
print 'Hello World' 
```
这段代码会在系统的输出流中输出“Hello World”字符串。代码中包含一个 print 语句，你所见到的一行一行的代码都是由语句组成的。所谓语句，就是告诉计算机做一件什么样的事。这里先说一下表达式。
```python
x = 2 + 2
print x
```
表达式是要告诉计算机做什么样的运算，例如上例中 `2 + 2` 就是要让计算机计算出加的结果。计算机最基本的组成结构是门电路，然后由门电路组成加法器，加法器是计算机最基本的运算单元，其他的高级运算器例如减法、乘法、除法等都是在加法器的基础上构建的。所以我觉得**表达式是程序代码的核心**，这只是我的个人见解，或许这种说法不对。我只是觉得表达式是在用最原始的方式来描述计算机的计算原理。

语句和表达式的区别是，表达式是某事，而语句是做某事。所以语句要告诉计算机做什么事就得包含表达式。在大部分的编程语言中，语句都以分号结尾。但是在 Python 中不是这样的，它没一行就是一个语句，不需要分号。如果你接触过 shell 脚本语言，你就会知道，Python大部分的语法结构都继承了 shell 脚本，或许是它们同属脚本语言的原因。

Python中也有分号，它的作用是需要把多个简单语句（比如赋值语句，print，函数调用）放在同一行的时候，使用分号把它们隔开，组成一个复合语句。实际上，你在每个语句的结尾加上分号程序也会正常运行，Python解释器会认为分号后边接了一个空的语句。但这不是Python设计的本意。说实话，刚开始接触 Python 的时候真的很不习惯，总是不自觉的在结尾加上分号，这就是传说中的**分号结尾综合症**。
<br />
####中文编码问题
从上面所谈的“语句”开始，我们就开始 Python 的编程了。之所以先讲语句，是因为程序代码都是又由一行一行 的语句构成，其他的内容都是用来构成语句的。我想来打个比喻，也不知道挣不正确。就比如说建房子吧，语句就好比时砖，代码就好比是房子，房子是由一块一块的砖堆砌而成的。在建房子之前，我们得先造好砖。之后我们所学习的一些基础的内容都是构成砖块的原材料，例如数据类型、变量、数据结构等；而像一些更高级的内容，例如算法等，则是讲述构建房子的方法，我们建房子的时候当前得考虑怎么样建才结实，才好看。

好像扯得有点远了，就当是承前启后吧。其实这里要说的是关于 Python 源代码文件的中文编码问题。按照上面的例子，我们来写个一中文版的 “Hello world!”。

```python
#!/usr/bin/python
# Filename : helloworld.py

print "你好，世界！"
```

这里先申明一下，**本教程所有示例的运行都是基于 Linux 平台**。接下来我们打开终端，运行以上程序：

> $ python helloworld.py

结果：
```
  File "hello_zh.py", line 4
SyntaxError: Non-ASCII character '\xe4' in file hello_zh.py on line 4, but no encoding declared; see http://python.org/dev/peps/pep-0263/ for details
```

这段信息告诉我们，在文件 hello_zh.py 的第4行有语法错误，他说我们没有指定编码，并让我们从这里 http://python.org/dev/peps/pep-0263/ 获取详细资料。那我们去那个网址看看，发现后如下内容：

```
Python will default to ASCII as standard encoding if no other encoding hints are given.

To define a source code encoding, a magic comment must be placed into the source files either as first or second line in the file, such as:

	# coding=<encoding name>

or (using formats recognized by popular editors)

    #!/usr/bin/python
    # -*- coding: <encoding name> -*-

or

    #!/usr/bin/python
    # vim: set fileencoding=<encoding name> :
```
 
他说，如果没有指定其他的编码，**Python将采用 ASCII 作为默认的编码**。如果你要为源代码重新指定编码，则需要在源代码文件的第一行或者第二行进行说明。他提供了三种指定文件编码的方式。下面我们改一下上面的代码：

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-
# Filename : helloworld.py

print "你好，世界！"
```

再次运行代码，正常输出“你好，世界！”。也就是说，**当我们的代码中含有中文的时候，就需要指定文件的编码方式为 utf-8**。这里的 print 是一个输出语句，它会在终端打印其后所列的字符串，可以有多个字符串，字符串间用逗号隔开，遇到逗号时会输出一个空格，在末尾会自动输出一个换行符。如下所示：

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-
# Filename : print.py

print "My name is huoty,", "age is 24."
```
输出结果：
```
My name is huoty, age is 24.
```

Print 还有很多高级的用法，我们以后会接触到。

你是不是觉得我所谈的**中文编码问题**其实是一个很简单的问题。其实不然，假如你是刚基础这门语言，如果你不明所以，你会走很多弯路。在本教程中，**我所单独列出来的条目，都是我认为比较重要的内容**。说实话，我自己也觉得自己啰嗦，就一个编码问题就花了这么大的篇幅，而且还说了很多不相关的内容。**我写本教程的本意就是要记录一些关于编程中要注意的细节，我希望将我所了解和理解的一切都记录在这里**。其实我已经很努力的在控制篇幅了，但每说到一个内容都觉得意犹未尽。
<br />
#### 代码块
如果你接触过编程，你会发现大部分的语言都采用“{}”来区分代码块。我没有想到一个合理的说法来解释什么是代码块，这里我先用C语言来讲一个例子：
```c
if (a > 5)
{
	b = a + 1;
	b = b * b;
	return b;
}
else
{
	b = a * a;
	b = b / a;
	return b;
}
```

以上代码只是举的一个例子，没有任何意义。在 if 条件为真的情况下，if 下边被“{}”包裹的内容会被执行。在if条件为假时，else 下边被“{}”包裹的内容会被执行。程序中两个被“{}”包裹的内容就是两个不同的代码块。**代码块的作用是用来体现代码的层次关系**。在 Python 中，则采用缩进来区分代码块，具有相同缩进的代码行组成一个代码块。也就是说，**在 Python 中，行首的空白符（空格和制表符）是非常重要的**。在逻辑行首的空白用来决定逻辑行的缩进层次，从而用来决定语句的分组。同一层次的语句必须有相同的缩进，每一组这样的语句称为一个块，也就是代码块。下面我们用 Python 改写上边的代码：

```python
#!/usr/bin/python
# -*- coding: utf-8 -*-
# Filename : codeblock.py

a = 2

if a > 5:
    b = a + 1 
    b = b * b 
    print b
else:
    b = a * a 
    b = b / a 
    print b
```
运行程序会输出结果`2`。错误的缩进会产生语法错误，例如下面的代码：
```python
#!/usr/bin/python
# -*- coding: utf-8 -*-
# Filename : error.py

print "My name is huoty."
  print "What's your name?"
print "end."
```
运行代码出现如下错误：
```
  File "error.py", line 6
    print "What's your name?"
    ^
IndentationError: unexpected indent
```
不同的代码块采用不同的缩进方式是被允许的，但是不建议这么做，例如下面的代码能够正常运行：
```python
#!/usr/bin/python
# -*- coding: utf-8 -*-
# Filename : codeblock.py

a = 2

if a > 5:
    b = a + 1 
    b = b * b 
    print b
else:
    	b = a * a 
    	b = b / a 
    	print b
```
虽然这样的代码没有任何错误，但我们在编码的时候应该注意代码的整洁和美观，尽量采用相同的缩进方式。不要混合使用制表符和空格来缩进，因为这在跨越不同的平台的时候，无法正常工作。我 强烈建议 你在每个缩进层次使用 单个制表符 或 两个或四个空格 。选择这三种缩进风格之一。更加重要的是，选择一种风格，然后一贯地使用它，即 只 使用这一种风格。 
<br />
#### 执行方式
