# Karma
> A distributed/decentralized framework for interactable data and network infrastructure, included IoT.

---

#### 维护：

- [tiannian](https://github.com/tiannian) <dtiannian@aliyun.com, dtiannian@gmail.com>

## 目标

- 适配更多廉价高效的设备，降低物联网设备的硬件成本。
- 适配更多的网络协议，模块化的，层次化的设计，降低物联网设备的开发成本。
- 提供可靠的连接协议与去中心化的节点发现机制，避免单点失效与网络波动对设备的影响。
- 为节点设计可靠的重连与自动恢复机制，降低设备使用者的维护成本与心智负担。
- 提供完善的加密策略与认证和机制，保证节点的安全性，为用户提供更好的隐私保护机制。
- 提供规范化的协议设计，提供便于移植的代码，一定程度上解决数据孤岛的问题。

## 网络特性
Karma希望能够为网络提供一些特性：

1. 采用DHT网络进行去中心化的节点发现，降低网络中单点失效与网络路径中断而对网络产生的影响。
2. 节点可以快速且自主的加入网络，无需更多的调整即可向网络提供基本功能。
3. 节点可以利用缓存的路由信息自主进行网络组网调整，解决传输过程中网络波动问题，实现自动恢复连接。
4. 在节点网络无法直接到达时，可借助其余节点转发数据流量。
5. 网络提供节点上资源发现的机制，节点可以快速的发现理解资源。
6. 节点可以自主缓存请求数据，并可以将单一节点的请求访问平衡至其余节点上。
7. 提供高性能加密方案，利用签名机制验证节点，加密网络通讯流量，保证数据安全性。
8. 用户可以自由控制节点权限与访问限制。
9. 提供对多种网络接入方式的支持。
10. 提供统一抽象的编程接口与标准，方便开发者开发，方便在不同平台上进行移植。
11. 提供基础传感与基础控制的原始支持，避免高层应用，降低对节点的性能需求。
12. 利用虚拟机机制，实现通用的执行环境。（可选项）
13. 基于OEM预置密钥对实现的节点密钥安全生成。
14. 网络会为节点提供动态和升级与固件更新支持。

## 规范结构

Karma的规范中包含以下部分：

- [Karma](https://github.com/Karma-IoT/Karma) - 分布式/去中心化的数据交互框架与网络基础设施。
- [Chest](https://github.com/Karma-IoT/Chest) - 通用化的包管理器，可管理包括源代码，预编译文件，工具链等。

## 规范目录

1. 简介
   - [现状](specs/1.1-Status.md)
   - [设计](specs/1.2-Design.md)
2. 设计
   - [节点](specs/2.1-Node.md)
   - [资源](specs/2.2-Resources.md)
   - [权限](specs/2.3-Permission.md)
   - [分层]()

## 实现项目
- [Chepp](https://github.com/Karma-IoT/Chepp) - 通用包管理器 `Chest` 的C++实现。
- [TweetNacl](https://github.com/tiannian/TweetNaCl) 来自 [tweetnacl](https://tweetnacl.cr.yp.to) 的Public Domain加密算法库。
- [er-coap](http://github.com/Karma-IoT/er-coap) 来自`contiki`的CoAP协议栈实现。
- [ascl](https://github.com/Karma-IoT/ascl) 抽象不同平台的抽象系统适配层定义。
- [ascl-type](https://github.com/Karma-IoT/ascl-type) 用于ascl中的跨平台数据类型定义。

## 参与项目
我们欢迎对Karma项目感兴趣，志同道合的朋友参与。

规范采用提交issues的方式来改进系统与设计。
