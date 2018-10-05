# Python Tutorial
这个教程将会介绍Python去使用OpenMesh的基本概念。
我们讲讨论以下几个主题：
- 怎么去建立Python与OpenMesh之间的链接。
- 怎么去创建一个空的网格。
- 怎么为一个网格添加顶点和面。
- 怎么使用迭代器去遍历网格数据。
- 怎么添加和移除自定义的属性。
- 怎么读取网格文件和把网格文件输出为模型网格文件
此外, 我们将简要的讨论使用Python和C++去调用OpenMesh时它们之间的不同之处。
# Building the Python Bindings
使用Python Bindings需要依赖一下的库:
- Python (2.7 or later)
- Boost Python(1.54.0 or later)
```
注意:
    要确保你的Boost Python和Python的版本是匹配的，也就是说，需要把Boost Python与和它对应的Python链接起来。
```
OpenMesh会自动构建出Python Bindings。生成的文件将会被写入构建树中的Build/python的子目录。关于如果构建OpenMesh的更多信息，请参见[Compiling OpenMesh](http://www.openmesh.org/media/Documentations/OpenMesh-6.3-Documentation/a00017.html)。
如果CMake不能找到你已经安装好的Python(或者找到了错误的那个)，你能够通过设置下边的变量来显示的进行安装:
```
PYTHON_LIBRARY          - Path to the python library
PYTHON_INCLUDE_DIR      - Path to where Python.h if found
```
类似的，如果CMake没有找到你已经安装好的Boost Python，你可以按照下边进行设置:
```
BOOST_ROOT              - Preferred installation prefix
BOOST_INCLUDEDIR        - Preferred include directory e.g. <prefix>/include
BOOST_LIBRARYDIR        - Preferred library directory e.g. <prefix>/lib
```
# Getting Started
如果要使用OpenMesh的Python Bindings，我们第一步是需要在python文件中导入openmesh模块:
```
from openmesh import *
```
这个模块提供了两个网格类：一个是多边形网格(PolyMesh)，另一个是三角形网格(TriMesh)。 如果可能的话，你应该去使用三角形网格，因为它们通常更有效。此外， 一些算法仅仅适用于三角形网格，当然，三角形网格继承了多边形网格的全部功能。
以下代码是初始化一个新的三角形网格:
```
mesh = TriMesh()
```
