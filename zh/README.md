# Karma
> A distributed/decentralized framework for interactable data.

Karma是一个分布式/去中心化，安全，多层次，为物联网设备设计乃至更高级设备设计的数据交互框架。Karma目标是提供一个不同于传统中心化设计的数据交互框架，以试图解决传统中心化数据传感，交互方案中单点失效，数据安全，网络稳定性等方面的问题。

---

#### 维护：

- [tiannian](https://github.com/tiannian) <dtiannian@aliyun.com, dtiannian@gmail.com>

## 网络特性(设计目标)
Karma希望能够为网络提供一些特性：

1. 采用DHT网络进行去中心化的节点发现，降低网络中单点失效与网络路径中断而对网络产生的影响。
2. 节点可以快速且自主的加入网络，并向网络提供基本功能。
3. 节点可以利用缓存的路由信息自主进行网络组网调整。
4. 在节点网络无法直接到达时，可借助其余节点转发数据流量。
5. 网络提供节点上资源发现的机制，节点可以快速的发现理解资源。
6. 节点可以自主缓存请求数据，并可以将单一节点的请求访问平衡至其余节点上。
7. 利用密码学验证节点，加密网络通讯流量，保证数据安全性。
8. 用户可以自由控制节点权限与访问限制。
9. 提供对多种网络接入方式的支持。
10. 提供统一抽象的编程接口与标准，方便开发者开发，方便在不同平台上进行移植。
11. 提供基础传感与基础控制的原始支持，避免高层应用，降低对节点的性能需求。
12. 使用WASM作为通用执行环境，实现通用的执行环境。（可选项）
13. 基于OEM预置密钥对实现的节点密钥安全生成。
14. 网络会为节点提供动态和升级与更新支持。

## 规范目录

[目录](SUMMARY.md)

## 实现项目
- [KBT](https://github.com/tiannian/KBT) (Karma Build Tool) 用于构建与组织Karma项目。
- [TweetNacl](https://github.com/tiannian/TweetNaCl) 来自 [tweetnacl](https://tweetnacl.cr.yp.to) 的Public Domain加密算法库。
- [er-coap](http://github.com/Karma-IoT/er-coap) 来自`contiki`的CoAP协议栈实现。
- [ascl](https://github.com/Karma-IoT/ascl) 抽象不同平台的抽象系统适配层定义。
- [ascl-type](https://github.com/Karma-IoT/ascl-type) 用于ascl中的跨平台数据类型定义。
- [kbucket](https://github.com/Karma-IoT/kbucket) 用于记录管理Kademlia协议的路由表。

## 参与项目
我们欢迎对Karma项目感兴趣，志同道合的朋友参与。

规范采用提交rfcs的方式来改进系统与设计。
