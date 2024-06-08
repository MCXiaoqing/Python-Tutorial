# Python基础

> 现在开始正式学习Python3!

## 创建第一个Python程序

Python程序的拓展名是`.py`(或`.pyw`, `.pyi`)。

在任意位置创建一个Python文件, 例如`hello.py`, 然后在编辑器中输入以下代码:

```python
print("Hello, world!")
```

保存文件, 然后在命令行中运行或直接双击运行该文件:

```bash
python hello.py
```

如果一切顺利, 你应该看到输出:

```
Hello, world!
```

这就是一个最简单的Python程序了。下面会解释这个代码...

## 使用交互模式

Python还有一种交互模式, 可以在命令行中输入代码并立即执行, 而不是保存到文件中。

在命令行中输入`python`命令, 然后按下`Enter`键, 进入Python交互模式。

交互模式通常适用于测试一些小程序, 或者临时使用一些功能。我们通常不使用交互模式来编写程序。


## Python关键字

以下是Python3中所有的关键字:

```python
['False', 'None', 'True', 'and', 'as',
 'assert', 'break', 'class', 'continue', 'def',
 'del', 'elif', 'else', 'except', 'finally',
 'for', 'from', 'global', 'if', 'import',
 'in', 'is', 'lambda', 'nonlocal', 'not',
 'or', 'pass', 'raise', 'return', 'try',
 'while', 'with', 'yield']
```

这些关键字已经被Python的语法规则所使用, 因此这些关键字不能用作变量名, 函数名, 类名等。你并不需要死记硬背它们, 代码敲多了自然就熟悉了。

Python自带了一个`keywords`模块, 下列代码可以打印出所有的关键字:

```python
import keyword
print(keyword.kwlist)
```

## Python源文件编码

默认情况下，Python 源码文件的编码是 UTF-8。这种编码支持世界上大多数语言的字符，可以用于字符串字面值、变量、函数名及注释 —— 尽管标准库只用常规的 ASCII 字符作为变量名或函数名，可移植代码都应遵守此约定。要正确显示这些字符，编辑器必须能识别 UTF-8 编码，而且必须使用支持文件中所有字符的字体。

如果不使用默认编码，则要声明文件的编码，文件的 第一 行要写成特殊注释。句法如下：

```python
# -*- coding: encoding -*-
```

其中，`encoding` 是你所使用的编码，例如 `utf-8`、`gbk`、`gb2312` 等。

例如，要声明一个 UTF-8 编码的文件，第一行应该写成 `# -*- coding: utf-8 -*-`。

第一行 的规则也有一种例外情况，源码以 UNIX "shebang" 行 开头。此时，编码声明要写在文件的第二行。例如：

```python
#!/usr/bin/env python3
# -*- coding: utf-8 -*-
```

## 注释

注释是程序员用来解释代码的文字。注释不会被执行，添加注释可以提高代码的可读性和可维护性。

Python有多种注释方式:

- 单行注释: 以 `#` 开头，直到行尾。例如:
  ```python
  # 这是一个单行注释
  ```

- 多行注释: 三个双引号 `"""` 或 三个单引号 `'''` 开始，直到相应的结束符。例如:
  ```python
  """
  这是一个多行注释的第一行
  这是一个多行注释的第二行
  """

  '''
  这也是一个多行注释
  这也是一个多行注释
  '''
  ```

## 变量

变量是存储数据的地方。在Python中，变量不需要声明类型，变量可以改变类型。

变量名必须以字母或下划线开头，后面可以跟任意的字母、数字或下划线。例如:`name`, `age`, `my_name`, `total_count`, `result_1`, `_version`等。

声明变量的一般语法如下:

```python
variable_name = value
```

例如:

```python
name = "Alice"
age = 25
```

上面示例中, name和age是变量, 它们的值分别为"Alice"和25。通过下面的学习, 你将学到更多有关变量的知识。











