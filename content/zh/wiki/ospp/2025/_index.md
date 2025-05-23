---
title: '2025'
linkTitle: '2025'
weight: 1
---

# 介绍

BMF（Babit Multimedia Framework）是字节跳动开发的一个跨平台、多语言、可定制的多媒体处理框架。经过超过4年的测试与打磨，BMF已被深度定制以应对真实生产环境中的多种挑战。目前该框架已广泛应用于字节跳动的视频点播、直播转码、云剪辑及移动端前后处理等场景中，每天处理的视频数量超过20亿条。

这是我们为 [`开源软件供应链点亮计划 2025`](https://summer-ospp.ac.cn) 准备的项目想法页面。请参阅 OSPP 时间表 以获取重要日期信息。

# 面向学生的信息

## 入门指南
1. `了解 BMF` 如果你是对贡献 BMF 感兴趣的学生，推荐你首先加入我们的 [飞书交流群](https://applink.feishu.cn/client/chat/chatter/add_by_link?link_token=4cev1bee-4d94-42c8-972b-4ae4a12c9da1)。如果你有任何问题，欢迎随时联系我们。如果你知道其他同学提出问题的答案，也请不要犹豫，积极参与解答。
2. `寻找项目` 本页面列出的是带有导师的项目。这些项目定义明确，且已经有导师自愿提供指导。如果你对某个项目的描述不够清晰，或者有任何问题，请联系项目导师，或加入我们的飞书群咨询。
3. `联系我们` 如果你决定参与某个项目，请与我们社区联系并告知你的意愿。如果你希望从一个适合初学者的问题入手，请通知相关导师，以避免重复工作。
4. `提交申请`  学生需在 6 月 9 日之前 提交申请。项目开发的“正式工作期”将从 7 月 1 日 开始，到 9 月结束。请参考 OSPP 时间表 获取更多信息。

## 项目想法

### CPP动态流式处理接口实现
---

`项目描述`：在BMF中 python和cpp的builder层都是基于connector层构建的，其中python利用了binding技术，目前BMF支持通过python调用dynamic系列接口，支持在BMF graph运行时动态更改节点，比如新增、删除、重置。此项目的实现可以借鉴现有的python builder实现，来补齐cpp缺失的dynamic系列接口。

`项目难度`：基础

`技术领域、编程语言`：多媒体处理、C++

`项目产出要求`：用C++实现dynamic_remove，dynamic_add，dynamic_reset，update接口，并完成测试用例。

`项目技术要求`：
1. 良好的C++编程能力 
2. 了解基本的多媒体处理

`项目成果仓库`：https://github.com/BabitMF/bmf

`预估工时`：45 小时

`导师`: 刘奇翰 (jacklau1222@qq.com)

`项目备注`：https://github.com/BabitMF/bmf/discussions/154#discussioncomment-11442021，https://babitmf.github.io/docs/bmf/multiple_features/dynamic_graph/

### BMF DiffusionFlow
---

`Project Description`: BabitMF（BMF）是字节开源的多媒体处理框架，已支持音视频及 AI 算法的模块化调度。本项目将 Stable Diffusion（SD）端到端生成流程，封装为一系列可在 BMF Graph 中以节点化方式调用的 Module，进一步丰富框架在 AIGC 场景下的表现力。

`Project Difficulty`: Advanced

`Technical Domain, Programming Language`: AI, C++ Python

`Project Output Requirements`: 
1. 完成 SD 全链路基础 BMF Module 的设计、开发与单元测试，比如  Text Encoder、 Diffusion Scheduler、VAE Decoder 等
2. 产出 Text-to-Image、Image-to-Image 两个场景的完整示例
3. 实现点击／拖拽式 Graph 编辑器，并能预览生成结果

`Project Technical Requirements`: 
1. Python、C++
2. PyTorch，了解 SD 架构

`Project Completion Repository`: https://github.com/BabitMF/bmf

`Estimated Work Hours`: 80 小时

`Mentor:` Li Hu (huli.bruce@bytedance.com)

### Performance trace optimization in the multimedia framework
---

`Project Description`: BabitMF(https://github.com/BabitMF/bmf) is a multimedia framework which is widely used in media processing and AI related scenarios, there is a previous trace machenism for performance measurement already exists, but it will impact the latency (~10% more time cost occured) of whole pipeline once BMF_TRACE is enabled. This is a problem that needs to be solved urgently.

`Project Difficulty`: Advanced

`Technical Domain, Programming Language`: Perf, C++

`Project Output Requirements`: 
1. To root cause of the latency impacted by TRACE
2. To optimize the trace machenism to be lightweight, make the time cost bring by trace under 3%

`Project Technical Requirements`: 
1. Understanding of multimedia framework
2. Performance trace design and analytic capability

`Project Completion Repository`: https://github.com/BabitMF/bmf

`Estimated Work Hours`: 60   Hours

`Mentor:` Jonah (jonah.vanpraag@bytedance.com)

### 模版项目
---

`项目名称`：项目名称应明确直观的体现出项目的技术和目标任务；

`项目描述`：项目的相关背景、已有的工作、存在的不足、希望改进的要点、最终项目实现的目标等。

`项目难度`：结合项目要求、项目规模、技术难度、项目开发预估工作量、资源限制等因素设置。

`技术领域、编程语言`:

`项目产出要求`：明确学生需要做什么，预期达到什么效果。

`项目技术要求`：可从编程语言、技术栈、开发经验等角度提出要求。

`项目成果仓库`：本社区已有项目仓库地址，而非新建空仓。

`预估工时`：根据项目难度、产出要求、学生水平等因素给出预估的开发工时参考。

`导师`： 姓名（邮箱）

`项目备注`：项目自身的相关参考资料，比如书籍、论文、博客和相关的项目或 issue 的链接。