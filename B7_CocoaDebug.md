# 原文来自：[CocoaDebug/CocoaDebug](https://github.com/CocoaDebug/CocoaDebug)

| <img alt="logo" src="https://raw.githubusercontent.com/CocoaDebug/CocoaDebug/master/pic/logo.png" width="250"/> | <ul align="left"><li><a href="https://github.com/CocoaDebug/CocoaDebug/wiki/%E4%B8%AD%E6%96%87%E4%BB%8B%E7%BB%8D">中文介绍</a><li><a href="#introduction">Introduction</a><li><a href="#installation">Installation</a><li><a href="#usage">Usage</a><li><a href="#parameters">Parameters</a></ul> |
| -------------- | -------------- |
| Travis CI | [![Build Status](https://travis-ci.org/CocoaDebug/CocoaDebug.svg?branch=master)](https://travis-ci.org/CocoaDebug/CocoaDebug) |
| Codacy | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/6aac8606d10f403a811cafdf870bb552)](https://www.codacy.com/app/CocoaDebug/CocoaDebug?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CocoaDebug/CocoaDebug&amp;utm_campaign=Badge_Grade) |
| Codecov | [![codecov](https://codecov.io/gh/CocoaDebug/CocoaDebug/branch/master/graph/badge.svg)](https://codecov.io/gh/CocoaDebug/CocoaDebug) |
| Frameworks | [![Carthage Compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage) [![CocoaPods Compatible](https://img.shields.io/cocoapods/v/CocoaDebug.svg)](https://img.shields.io/cocoapods/v/CocoaDebug.svg) |
| Languages | ![Languages](https://img.shields.io/badge/languages-Swift%20%7C%20ObjC-blue.svg) |
| Platform | ![Platform](https://img.shields.io/badge/platforms-iOS%208.0+-blue.svg) |
| Licence | <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat" alt="License MIT"/> |

<span style="float:none" />

## 介绍

![example](https://raw.githubusercontent.com/CocoaDebug/CocoaDebug/master/pic/example.gif)

- [x] 通过摇晃来显示和隐藏黑色气泡(支持手机设备和模拟器)。

- [x] 长按黑色气泡来显示`UIDebuggingInformationOverlay`。(苹果的私有API，支持iOS 10/11)。

- [x] 应用内存使用和`FPS`.

- [x] 列举出全部的`print()`和`NSLog()`的信息显示在xcode的开发者控制台。

- [x] 列举出全部的应用发出的网络请求。

- [x] 在`Network Details`也面中抖动设备或者模拟器，能够把网络请求的详细信息发送到邮件或者复制到黏贴版。

- [x] 复制logs信息(长按文本信息, 可以进行全选复制或者选择部分进行复制)。

- [x] 使用关键字来查找logs信息。

- [x] 列举出应用和蛇别的信息, 包括 `version` `build` `bundle name` `bundle id` `screen resolution` `device` `iOS version`

- [x] 列出全部的沙盒文件夹和文件，支持展现和编辑。

- [x] 列出错误的崩溃信息。(可选)
