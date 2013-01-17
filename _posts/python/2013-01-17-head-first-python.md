---
layout: post
title: "Head First Python"
category: learning 
tags: [python]
description: Reading Head First Python book notes.
---
{% include JB/setup %}

## 1 meet python  **Everyone loves lists**

1. P20 `isinstance(var, type)` 判断变量是哪个类型,类型匹配，返回True,否则,False。
    
    {% highlight python %}
    >>> names = ['Michael', 'Terry']
    >>> isinstance(names, list)
    True
    >>> num_names = len(names)
    >>> isinstance(num_names, list)
    False
    {% endhighlight %}

2. P21 查看built-in functions `dir(__builtins__)`,查看帮助文档`help(BIF_name)`。
3. P31 Python default recursion limit 1000, 可以用`sys.getrecursionlimit()`查看。如果需要更大，可以修改。

## 2 sharing your code **Modules of functions**

`PyPI` is short for Python Package Index.
1. P38 查看Python模块路径，`import sys; sys.path`,用`;`可以把多行放在一行中。 or 

    {% highlight python linenos %}
    >>>import sys
    >>>sys.path
    {% endhighlight %}

2. P40 distribute module
    1. Create a folder and put module files into it.
    2. Create a file called `setup.py` in the new folder, and input the following code.
    3. Build a distribution file.`python3 setup.py sdist`.
    4. Install your distribution into your local coypy of Python.`sudo spython3 setup.py install`.
    
{% highlight python %}
from distutils.core import setup

setup(
        name            = 'module name',
        version         = '1.0.0',
        py_modules      = ['module name'],
        author          = '',
        author_email    = '',
        url             = '',
        description     = '',
    )
{% endhighlight %}

    

files structure:
<pre>
nester
|-- MANIFEST
|-- build
|   |-- lib
|   |   |-- nester.py
|-- dist
|   |-- nester-1.0.0.tar.gz
|-- nester.py
|-- nester.pyc
`-- setup.py
</pre>

3. P63 `def func(argv_1, argv_2=0)`, argv_2是可选的，`func(arg,1)`与`func(arg)`都可以。带默认值的参数要在最后。
4. P71
>* BIFs have their own namespaces called `__builtins__`, and they are alutomatically included in every python program.
>* `range()` returns an iterator.
>* `print("\t", end='')`, including `end=''` as an argument to `print()` switches off its automatic inclusion of a new-line on output.

## 3 files and exceptions **Dealing with errors**



    
