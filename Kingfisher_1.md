# 原文来自[onevcat/Kingfisher](https://github.com/onevcat/Kingfisher)

<p align="center">

<img src="https://raw.githubusercontent.com/onevcat/Kingfisher/master/images/logo.png" alt="Kingfisher" title="Kingfisher" width="557"/>

</p>

<p align="center">
<a href="https://travis-ci.org/onevcat/Kingfisher"><img src="https://img.shields.io/travis/onevcat/Kingfisher/master.svg"></a>
<a href="https://github.com/Carthage/Carthage/"><img src="https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat"></a>
<a href="http://onevcat.github.io/Kingfisher/"><img src="https://img.shields.io/cocoapods/v/Kingfisher.svg?style=flat"></a>
<a href="https://raw.githubusercontent.com/onevcat/Kingfisher/master/LICENSE"><img src="https://img.shields.io/cocoapods/l/Kingfisher.svg?style=flat"></a>
<a href="http://onevcat.github.io/Kingfisher/"><img src="https://img.shields.io/cocoapods/p/Kingfisher.svg?style=flat"></a>
<a href="https://codebeat.co/projects/github-com-onevcat-kingfisher"><img alt="codebeat badge" src="https://codebeat.co/assets/svg/badges/A-398b39-669406e9e1b136187b91af587d4092b0160370f271f66a651f444b990c2730e9.svg" /></a>
<a href="#backers" alt="sponsors on Open Collective"><img src="https://opencollective.com/Kingfisher/backers/badge.svg" /></a>
<a href="#sponsors" alt="Sponsors on Open Collective"><img src="https://opencollective.com/Kingfisher/sponsors/badge.svg" /></a>
</p>

Kingfisher 是一个轻量级的，纯粹使用Swift语言进行编写的库，它用来从web中下载并缓存图片。
这个项目深受[SDWebImage](https://github.com/rs/SDWebImage)的启发（它是一个十分流行的图片下载和缓存的库）。
Kingfisher给你提供了一个机会，就是在你的下一个应用程序中去只Swift语言与完成整个开发过程(而不是需要让OC和Swift进行桥接调用)。

## 特性

- [x] 异步的进行网络图片的下载和缓存。
- [x] `URLSession`-based networking. 提供基础的图片处理功能和滤镜功能。
- [x] 使用内存和磁盘的多层缓存机制。
- [x] 能够去取消下载任务和处理任务以提高性能。
- [x] 独立的功能组件。能够根据跟人需要去分开使用下载器或者缓存系统。
- [x] Prefetching images and showing them from cache later when necessary.
- [x] 对`UIImageView`，`NSImage`和`UIButton`进行了拓展，能够直接使用URL来设置图像。
- [x] 设置图像时会播放内置的过渡动画。
- [x] 加载图像时可以使用自定义的占位图。
- [x] 可拓展的图像处理过程和新的图像格式的支持。

最简单的使用样例如下：
通过给`UIImageView`的拓展加上网络图片的URL即可完成。
```swift
let url = URL(string: "url_of_your_image")
imageView.kf.setImage(with: url)
```
Kingfisher将会从`url`中下载图片，并把图片发送到内存缓存和磁盘缓存，并显示到`imageView`这个控件上。
当你稍后使用相同的代码时(译者：这里说的应该是url相同)，图像将会从缓存中检索得到并立即显示。

有关Kingfisher更多的使用例子，可以去查看[Cheat Sheet](https://github.com/onevcat/Kingfisher/wiki/Cheat-Sheet)。


