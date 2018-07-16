原文来自[google/yapf](https://github.com/google/yapf)
====
YAPF
====

.. image:: https://badge.fury.io/py/yapf.svg
    :target: https://badge.fury.io/py/yapf
    :alt: PyPI version

.. image:: https://travis-ci.org/google/yapf.svg?branch=master
    :target: https://travis-ci.org/google/yapf
    :alt: Build status

.. image:: https://coveralls.io/repos/google/yapf/badge.svg?branch=master
    :target: https://coveralls.io/r/google/yapf?branch=master
    :alt: Coverage status


介绍
============
当前大多数的Python格式化程序--- e.g., autopep8, and pep8ify ---都是为了去移除代码中的格式错误。
但是这样子会有一些明显的局限性。
举一个例子，有些代码符合PEP 8的准则可能不需要重新格式化。
但这并不意味这那些代码看起来很好看。
YAPF使用了一个不同的方法。
它是基于有Daniel Jasper提出的clang格式。
本质上，该算法会将代码格式化为符合代码样式指南的最佳格式，
即使源代码没有违反代码样式指南。
这个想法类似于GO语言的编程工具‘gofmt’:
结束所有关于格式化的圣战 - 
如果全部的代码库都使用YAPF对代码的格式进行简单的修改，
那么我们的工程代码格式就会保持一致，这样在review代码的时候就不会有人因为代码的格式而进行没有意义的争论。
最终的目标
The ultimate goal is that the code YAPF produces is as good as the code that a
programmer would write if they were following the style guide. 
It takes away
some of the drudgery of maintaining your code.
