---
title: 'DID：创建用户友好、安全且可互操作的区块链身份'
coverImage: 'images/image1.png'
category: Popular
subtitle: '去中心化身份（DID）是区块链技术中数字身份管理的革命性方法。'
date: '2023-08-21T16:00:00.000Z'
author: 
- github:explainCKBot
---

DID（Decentralized Identifier，去中心化身份）通过为去中心化应用程序提供独特、用户友好且安全的身份标识，为用户带来了极大的便利。本文将探讨两个著名的基于不同区块链平台构建的 DID 解决方案：以太坊域名服务（ENS）和搭建在 Nervos L1 CKB 上的 .bit。




## 什么是 DID？

DID（Decentralized Identifier，去中心化身份）是一种数字标识，允许个人、组织甚至设备创建和管理自己独特的、自主的身份。不同于传统的用户名、电子邮件地址或社会保障号码等标识，DID 不受中心化机构控制，避免了单点故障。DID 由身份持有者生成、拥有和管理，让持有者能够与数字世界中其他应用进行安全、私密的交互。

DID 借助区块链技术创建了去中心化、防篡改且高度安全的身份管理基础设施。DID 是在区块链或其他分布式账本上注册的唯一标识符，由身份持有者独立验证和更新，无需中间商。相对于中心化身份管理系统，这种去中心化方法带来更好的安全性、隐私性和用户控制。


### 以太坊域名服务（ENS）

ENS（Ethereum Name Service，以太坊域名服务）是建立在以太坊区块链上的去中心化域名系统，将复杂的机器可读标识符转换为更易理解的人类可读名称。通过将诸如 "alice.eth" 之类的名称映射到以太坊地址或其他机器可读数据，ENS 简化了基于区块链的身份共享和使用。

ENS 架构包含两个主要组件：注册表和解析器。注册表是一组智能合约，维护所有域名和子域名的列表，存储有关所有者、解析器和有效期等信息以供缓存使用。解析器负责将名称转换为地址或其他数据，不同的解析器支持不同类型的记录。

ENS 域名可以通过支持的钱包或应用程序进行注册和管理，为用户提供用户友好的界面来管理数字身份。ENS 还支持反向解析，允许元数据与以太坊地址关联。


### 搭建在 Nervos CKB 上的 .bit 

.bit 是基于 Nervos CKB（Layer 1 区块链）构建的跨链去中心化账户系统。该系统提供以 .bit 为后缀的独特命名系统，可用于加密货币转账、域名解析、身份认证等多种场景。.bit 账户可以使用任何公链的地址甚至电子邮件进行注册和管理。

.bit 系统由五个主要组件构成：核心协议、Keeper、解析服务、客户端 SDK 和 Dapp UI。核心协议包括部署在 Nervos CKB 上的一系列智能合约，定义了 .bit 账户的操作标准。Keeper 是一组链下程序，负责触发符合核心协议的交易。解析服务建立在 Nervos CKB 交易之上，向公众提供账户解析服务。客户端 SDK 简化了与 .bit 相关应用程序的集成，而 Dapp UI 允许用户通过多种接口与系统交互。

.bit 系统的独特之处在于其广泛的兼容性，允许用户使用比特币或以太坊等其他公链的私钥来管理 Nervos CKB 上的资产。这一点通过 Nervos CKB 平台上灵活的签名算法支持得以实现。




## ENS 和 .bit 的区别 

ENS 和 .bit 都是去中心化的命名服务，利用区块链技术构建以用户为中心的互联网。尽管它们的共同目标是将人类可读的名称映射为机器可读的标识符，但两者仍然存在许多关键差异。

首先，ENS 建立在以太坊区块链上，而 .bit 依赖于 Nervos CKB（Layer 1区块链）。底层技术的不同决定了这两个系统的兼容性和用途。ENS 主要针对以太坊地址和相关资源，但也支持其他加密货币地址和内容哈希。与此相比，.bit 允许用户使用任何公链的地址甚至电子邮件地址进行注册和管理，提供了更广泛的兼容性。

另一个显著差异是域名后缀。ENS 域名带有 ".eth" 后缀，如 "alice.eth"，而 .bit 域名使用 ".bit" 后缀，如 "alice.bit"。这种区别对用户识别正在与哪个基于区块链的命名系统进行交互至关重要。

这两个系统的架构也不同。ENS 包括注册表和解析器两个主要组件。注册表是一组智能合约，跟踪所有域名和子域名，记录所有者、解析器和每个域名的有效期等信息，而解析器则负责将名称转换为地址。作为对比，.bit 有五个主要组件：核心协议、Keeper、解析服务、客户端 DK 和 Dapp UI。 核心协议包括一系列部署在 Nervos CKB 上的锁脚本和类型脚本，它们建立 .bit 账户并设定操作标准。

此外，ENS 和 .bit 中的账户所有权和管理方式也不同。在 ENS 中，账户所有者可以是外部账户（用户）或智能合约。在 .bit 中，账户的所有者或管理者可以是任何公链的私钥，甚至是电子邮件地址，为用户提供了更大的灵活性。

最后，ENS 和 .bit 使用的解析机制也有所不同。ENS 采用两步流程来解析名称，它先查询注册表以识别负责的解析器，然后查询该解析器获取答案。与此相反，.bit 使用的解析服务，则根据 Nervos CKB 上的交易解析 .bit 的全局状态，向公众提供账户解析服务。




## DID 与 DNS 的比较

DID（去中心化身份）和 DNS（域名系统）有一个共同的目标：将人类可读的名称映射为机器可读的标识符。然而，在架构、控制机制和底层技术方面，两者存在显著差异。

在架构方面，DNS 是中心化的分层系统，受域名注册商和 ICANN（互联网名称与数字地址分配机构）等可信机构监管。相对地，DID 建立在去中心化、无需信任的区块链架构之上，ENS 和 .bit 只是 DID 的两个示例。

在控制权和所有权方面，两者也不同。通过 DNS，域名注册商等第三方通常管理域名的控制和所有权，这可能引发审查、域名扣押或其他争议等问题。相比之下，DID 让用户能够直接控制其身份，减少了对中心化机构的依赖，赋予用户更大的自治权。

DNS 和 DID 之间的安全和信任模型也不同。DNS 依赖于证书颁发机构和其他中心化实体来建立安全连接，而 DID 利用区块链技术的内在安全性，创造了一个无需信任的环境，允许对数字身份进行安全、防篡改的验证，而无需中心化的信任方。

另一个显著差异是跨平台兼容性。DID 提供跨各种平台和应用程序的互操作性和兼容性，让用户能够跨多个区块链和去中心化应用程序管理其身份。与此相反，DNS 主要是将域名映射到 IP 地址。

用户隐私和控制权是 DID 和 DNS 之间的核心区别。DID 让用户能够更好地控制其数字身份，让他们在无需第三方服务的情况下管理自己的信息和隐私。DNS 则依赖于中心化服务，所以 DNS 可能不会总是充分考虑用户的隐私和控制权。




## 总结

去中心化身份代表了数字身份和互联网运作方式的重大转变。 与传统 DNS 模型相比，通过利用区块链技术的力量，DID 提供了更好的安全性、隐私性和用户控制。 借助 ENS 和 .bit 等解决方案，用户可以从去中心化的命名系统中受益，这些系统将用户置于主导地位，从而在管理其数字身份方面实现更大的自主性和灵活性。
