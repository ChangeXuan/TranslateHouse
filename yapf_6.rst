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
In essence, the algorithm takes the code and reformats it to the
best formatting that conforms to the style guide, even if the original code
didn't violate the style guide. The idea is also similar to the 'gofmt' tool for
the Go programming language: end all holy wars about formatting - if the whole
codebase of a project is simply piped through YAPF whenever modifications are
made, the style remains consistent throughout the project and there's no point
arguing about style in every code review.

The ultimate goal is that the code YAPF produces is as good as the code that a
programmer would write if they were following the style guide. It takes away
some of the drudgery of maintaining your code.
