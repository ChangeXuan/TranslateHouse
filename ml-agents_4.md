# 原文来自[Unity-Technologies/ml-agents](https://github.com/Unity-Technologies/ml-agents)
<img src="https://github.com/Unity-Technologies/ml-agents/blob/master/docs/images/unity-wide.png" align="middle" width="3000"/>

# Unity 机器学习代理工具集(Beta)
**Unity机器学习代理工具集** (ML-Agents)是一个开源的unity插件，它可以使开发者在游戏或者模拟环境下使用训练好的机器学习代理。
我们能够使用多种方法去训练代理，如强化学习，模仿学习，神经网络，或者通过一个简单易用的Python API来去使用其他的机器学习方法。
我们也提供了使用最先进的算法的实现方式(基于TensorFlow)，并能够使得开发者和业余爱好者能够在自己的2D，3D甚至是VR/AR游戏中去很好的训练和使用机器学习智能代理。
这些被训练好的代理能够被用于多个不同的目的，包括控制NPC的行为(在一个多样化设置的游戏中，可以使用代理让自己游戏的敌人拥有智能)
对游戏进行自动测试和对不同的游戏设计进行评估和预发布。
这个机器学习代理工具集对于游戏开发者和AI研究员两者来说都有较大的益处，它提供了一个良好的中心平台，让AI能够在研究员和Unity游戏开发者社区中得到长足的发展。

## 特性
* 使用Python对Unity进行配置
* 有超过10个样例
* 支持复杂的环境配置以及训练脚本
* 使用深度增强学习模型来训练记忆增强代理
* 容易去定义脚本去完成机器学习中的课程学习
* 广播代理的行为为了监督式学习
* 支持模仿学习
* Flexible Agent control with On Demand Decision Making
* 在环境中输出可视化的网格信息
* 可以使用Docker简化设置
