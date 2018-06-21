# 原文来自[onevcat/APNGKit](https://github.com/onevcat/APNGKit)

<p align="center">
<img src="https://raw.githubusercontent.com/onevcat/APNGKit/master/images/logo.png" alt="APNGKit" title="APNGKit" width="1000"/>
</p>
<p align="center">
<a href="https://travis-ci.org/onevcat/APNGKit"><img src="https://img.shields.io/travis/onevcat/APNGKit/master.svg"></a>
<a href="https://github.com/Carthage/Carthage/"><img src="https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat"></a>
<a href="http://cocoadocs.org/docsets/APNGKit"><img src="https://img.shields.io/cocoapods/v/APNGKit.svg?style=flat"></a>
<a href="https://raw.githubusercontent.com/onevcat/APNGKit/master/LICENSE"><img src="https://img.shields.io/cocoapods/l/APNGKit.svg?style=flat"></a>
<a href="http://cocoadocs.org/docsets/APNGKit"><img src="https://img.shields.io/cocoapods/p/APNGKit.svg?style=flat"></a>
<img src="https://img.shields.io/badge/made%20with-%3C3-blue.svg">
</p>

APNGKit是一种在iOS和macOS平台上用来加载和显示APNG图像的高性能框架。它是建立在[modified version of libpng](https://github.com/onevcat/libpng)之上具有APNG支持，并使用Swift语言进行编写的框架。
这是一个属于Cocoa Touch高层级的抽象API，使用时十分方便。
正因如此，当你使用APNKit去播放APNG格式的图片集合时，你会感到十分自在和快乐。

## APNG，它是什么，为什么要使用它？

APNG的全称为[Animated Portable Network Graphics](https://en.wikipedia.org/wiki/APNG)，它是从PNG格式拓展出来的一种新的文件格式。
它允许具有动画效果的PNG文件像GIF动画那样播放，同时它具有GIF没有的特点，能够支持24bit图像和8bit的透明图像。
这就意味着它会拥有更好的动画质量。
同时，如果去创建一个紧密的GIF，那APNG文件的大小可能与其相等甚至会小于GIF图的大小。

光说不练假把式；
下面的我来展示GIF和APNG的效果。
你可以去点击播放按钮来查看它们之间的动画效果。

<p align="center">
<a href="http://apng.onevcat.com/demo" target="_blank"><img src="https://raw.githubusercontent.com/onevcat/APNGKit/master/images/demo.png" alt="APNGKit Demo" title="APNGKit Demo"/></a>
</p>

上面的演示很酷吧。
和GIF图像相比起来，APNG的效果好多了！
等等。。。为什么我以前从来没有听说锅APNG呢？
因为它不是一个流行的格式。既然这样，为什么我要在我的下一个伟大的iOS/macOS应用程序中使用它呢？

这是个好问题！
APNG是一个很优秀的PNG拓展格式，同时它在不违背当前PNG标准的前提下具有较为简单的使用方法（
它由标准的PNG报头组成，所以如果你使用的平台不支持APNG，它将被识别成一副普通的PNG图像，PNG静态图像的内容为APNG图像序列的第一帧。）。
但不幸的是，它不是一种正规的被PNG组织接受的格式。
尽管这样，APNG依旧被许多厂商所接受，并在[W3C Standards](http://www.w3.org/TR/html5/embedded-content-0.html#the-img-element)多次被提及和称赞。
还有一种格式与APNG类似，它的名字叫MNG(Multiple-image Network Graphics)，并且它是由创建PNG的那个团队开发出来的。
MNG是一种综合的格式，但十分十分十分的复杂。
它太复杂了，以至于成立了一套"标准"，所以MNG几乎被所有的厂商和开发者所拒绝。
现在只有一个名叫[Konqueror](https://konqueror.org)的浏览器在默默支持这MNG格式，这真是个悲伤却很合理的事情。

尽管目前APNG没有被的接受，但我们仍然看到了它宽广的前景。
Apple公司最近在[桌面版和移动端的Safari](http://www.macrumors.com/2014/09/28/ios-8-safari-supports-animated-png-images/)对APNG进行了支持。
并且[微软的Edge](https://wpdev.uservoice.com/forums/257854-microsoft-edge-developer/suggestions/6513393-apng-animated-png-images-support-firefox-and-sa)以及[谷歌的Chrome](https://code.google.com/p/chromium/issues/detail?id=437662)也已经在他们的[WebKit核心](https://bugs.webkit.org/show_bug.cgi?id=17022)添加了有关APNG相关的东西，并正在考虑是否对APNG提供支持。



 
