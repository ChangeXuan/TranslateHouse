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
The Python Bindings depend on the following libraries:
- Python (2.7 or later)
- Boost Python(1.54.0 or later)
```
Note:
    Make sure that your Boost Python and Python versions match,i.e. that Boost Python was linked against the correct Python version.
```
The Python Bindings are automatically built with OpenMesh. The generated files are written to the Build/python subdirectory of the build tree.For more information on how to build OpenMesh see Compiling OpenMesh.
if CMake does not find your Python installation (or finds the wrong one)you can explicitly specify an installation by setting the following variables:
```
PYTHON_LIBRARY          - Path to the python library
PYTHON_INCLUDE_DIR      - Path to where Python.h if found
```
Similarly, if CMake does not find your Boost Python installation, set the following variables.
```
BOOST_ROOT              - Preferred installation prefix
BOOST_INCLUDEDIR        - Preferred include directory e.g. <prefix>/include
BOOST_LIBRARYDIR        - Preferred library directory e.g. <prefix>/lib
```
