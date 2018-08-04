# 原文来自：[Yalantis/Koloda](https://github.com/Yalantis/Koloda/blob/master/README.md)

KolodaView [![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage) ![Swift 4.0.x](https://img.shields.io/badge/Swift-4.0.x-orange.svg)
--------------

[![Yalantis](https://raw.githubusercontent.com/Yalantis/PullToMakeSoup/master/PullToMakeSoupDemo/Resouces/badge_dark.png)](https://Yalantis.com/?utm_source=github)

可以通过我们[博客](https://yalantis.com/blog/how-we-built-tinder-like-koloda-in-swift/)的文章来解决您的一些问题。
和其他事情我们也会在[博客](https://yalantis.com/blog/koloda-tinder-like-animation-version-2-prototyping-in-pixate-and-development-in-swift/)的文章中描述出来。

![Preview](https://github.com/Yalantis/Koloda/blob/master/Koloda_v2_example_animation.gif)
![Preview](https://github.com/Yalantis/Koloda/blob/master/Koloda_v1_example_animation.gif)

目的
--------------
KolodaView是一个专门为了简化实现iOS上火柴卡片效果而设计的一个类。
它添加了方便使用的方法，类似UITableView中dataSource/delegate的接口用来动态的加载view视图，并且做到了高效率的加载和释放view

线程安全
--------------
KolodaView是UIView的一个子类(也是属于UIKit组件)，所以它只能运行在主线程上。你可能会想使用其他线程去加载或更新KolodaView的内容或某一项,如果你要这样做，就必须要确保你的内容已经被加载，并且在你切换回主线程之前更新KolodaView。


