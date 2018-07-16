# 原文来自[svermeulen/Zenject](https://github.com/svermeulen/Zenject)

## 简介
Zenject是一个专门为Unity3D设计的轻量级的依赖注入框架(当然，它在Unity之外也能运行得很好)。
它能够把你的应用改变为一个低耦合并且高度分离的集合。
Zenject能够把不同的部分链接在一起，允许在许多不同的配置环境中进行简单的编写，重用，重构以及测试你的代码。

下面列出的平台都使用unity测试过: 
* PC/Mac/Linux
* iOS
* Android
* WebGL
* PS4 (with IL2CPP backend)
* Windows Store (including 8.1, Phone 8.1, Universal 8.1 and Universal 10 - both .NET and IL2CPP backend)
IL2CPP得到支持，但是仍然有一些缺陷 - 请看 <a href="#aot-support">这里</a>的缺点详细信息。
这个工程是开源的。
你能够找到官方的仓库在[这里](https://github.com/modesttree/Zenject).

## 特点

* Injection注入
    * 支持正常的C#类和MonoBehaviours的IDE
    * 构造器注入
    * 字段注入
    * 性能注入
    * 方法注入
* 条件绑定 (eg. by type, by name, etc.)
* 可以选择的依赖项
* 支持使用工厂类初始化后来对对象进行创建
* 嵌套容器，又名子容器
* 注入不同的Unity场景，将信息从一个场景传递到下一个场景
* 允许一个场景继承另一个场景的绑定项
* 支持全局，项目范围绑定，以添加所有场景的依赖项
* 基于约定的绑定，基于类名的绑定，基于命名空间的绑定，或者基于其他标准的绑定
* 有能力去验证在编辑器时间的对象图(包括使用工厂动态创建的对象图)
* 自动使用ZenjectBinding组件来绑定场景中的组件
* 使用Moq库进行自动模拟
* 内置内存池支持
* 支持使用装饰器绑定来完成装饰器模式
* 支持自动映射开发泛型类型
* 内置单元测试，集成测试以及场景测试
* 使用LazyInject<>构造来完成及时注入

