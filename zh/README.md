# Karma
> A IoT framework based P2P network.

Karma是一个基于P2P网络，安全，多层次的物联网(IoT)框架。Karma的目标是提供一个不同于传统中心化设计的物联网方案，以试图解决传统中心化物联网方案中单点失效，数据安全，网络稳定性等方面的问题。

---

#### 维护：

- [tiannian](https://github.com/tiannian) dtiannian@aliyun.com

## 网络特性(设计目标)
Karma希望能够提供一些特性：

1. 采用DHT网络进行节点发现，降低网络中单点失效与网络路径中断而对网络产生的影响。
2. 物联网节点可以快速且自主的加入网络，并向网络提供基本功能。
3. 节点利用缓存的路由信息自主进行网络组网调整。
4. 在节点网络无法直接到达时，可借助其余节点转发数据流量。
5. 节点可以快速的进行发现并进行通讯，提高节点通讯效率。
6. 节点可以自主缓存请求数据，并可以将单一节点的请求访问平衡至其余节点上。
7. 利用密码学验证节点，加密网络通讯流量，保证数据安全性。
8. 用户可以自由控制节点权限与访问限制。
9. 提供对多种网络接入方式的支持。
10. 提供统一抽象的编程接口与标准，方便开发者开发，方便在不同平台上进行移植。
11. 提供基础传感与基础控制，避免高层应用，降低对硬件芯片的性能需求。
12. 使用WASM作为通用执行环境，实现无`Consensus`的`DAPP`环境。（可选项）
13. 局部`Conensus`保证K-cluster数据一致性。（可选项，更新第6项）

## 规范目录

[规范目录](specs/SUMMARY.md)

## 实现项目
- [KBT](https://github.com/tiannian/KBT) (Karma Build Tool) 用于构建与组织Karma项目。
- [TweetNacl](https://github.com/tiannian/TweetNaCl) 来自 [tweetnacl](https://tweetnacl.cr.yp.to) 的Public Domain加密算法库。
- [libkademlia](#) Improved P2P algorithm protocol Kademlia achieve.
- [libascl](#) Abstract system compatible layer.
- [libcbor](#) Concise Binary Object Representation.
- [librouter](#) Router table manager module with static cache.
- [libkeystore](#) Private key , Public key and some meta information manager
- [libpfs](#) 提供对数据传输中PFS(完美前向安全)支持。
- [libkarma](#) karma框架核心库。

## 参与项目
我们欢迎对Karma项目感兴趣，志同道合的朋友参与。

