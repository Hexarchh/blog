---
author: Hexarchh
pubDatetime: 2026-09-24T00:15:00Z
title: 我想做的是 Systems for AI
slug: systems-for-ai
featured: false
draft: false
tags:
  - 随笔
  - 系统
  - AI Infra
description: "从 vLLM 到操作系统：真正吸引我的不是某个框架，而是系统本身。"
---

过去一段时间，我经常会看到各种各样的技术名词。

LLM。

Agent。

vLLM。

CUDA。

分布式系统。

数据库。

操作系统。

AI Infra。

每一个方向看起来都很重要。

每一个方向又好像都值得学。

最危险的状态就是：

什么都想学。

---

我之前也陷入过这种状态。

今天觉得后端不错，于是学 Go、Gin、GORM、Redis、gRPC。

过一段时间又觉得 AI 是未来，于是开始学 Python、PyTorch。

后来接触到系统方向，又发现操作系统、体系结构、虚拟化这些东西非常有意思。

再后来看到 vLLM、推理系统、GPU 编程，我又突然发现：

这些东西似乎全部连起来了。

---

慢慢地，我发现我真正感兴趣的并不是某一个具体框架。

我感兴趣的是：

**系统。**

比如一个大模型为什么可以同时服务成千上万个请求？

GPU 显存不够怎么办？

KV Cache 怎么管理？

多个 GPU 怎么通信？

为什么 batching 可以提高吞吐？

操作系统应该怎样为 AI workload 调度资源？

模型部署到底经过了哪些软件层？

如果未来的 Agent 可以执行越来越复杂的任务，那么它运行的基础设施应该是什么样？

这些问题，比"某个 API 应该怎么调用"更让我兴奋。

---

所以我现在给自己的方向，大概可以画成这样：

```text
             AI / LLM / Agent
                   │
                   │
              AI Infra
             /        \
            /          \
      Distributed      OS
        System          │
            \           │
             \          │
              Database
```

它们看起来是不同方向。

实际上却有大量交叉。

例如 vLLM。

表面上它是一个 LLM inference engine。

但继续往下看：

PagedAttention 本质上涉及内存管理。

Continuous Batching 涉及调度。

Tensor Parallel 涉及分布式通信。

KV Cache 涉及资源管理。

Scheduler 涉及系统设计。

突然之间，大模型推理变成了一道系统问题。

这也是我现在最感兴趣的地方。

---

我并不打算把自己限制成：

"我是做操作系统的。"

或者：

"我是做 AI 的。"

我更希望自己未来能站在两者的交界处。

去做类似：

**Systems for AI。**

也就是：

怎样设计更好的系统，让 AI 跑得更快、更便宜、更安全。

---

当然，现实是：

现在的我距离这些东西还很远。

NEMU 还在写。

操作系统也没有真正实现过。

CUDA 还没有系统学习。

分布式系统很多经典论文也没有读。

PyTorch 的内部机制也了解得很浅。

但我开始觉得：

不知道并不是一件特别可怕的事情。

真正危险的是不知道自己为什么学。

---

所以现阶段，我给自己的目标反而变得简单了。

把基础补扎实。

计算机组成原理。

操作系统。

计算机网络。

数据库。

分布式系统。

C/C++。

Python。

然后一点点接触 AI Infra。

不急着成为"AI Infra Engineer"。

先成为一个真正理解计算机的人。

剩下的事情，

慢慢来。
