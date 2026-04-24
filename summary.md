# AI的淘金年代：11期访谈文档集

生成日期：2026-04-24

## 资料来源与处理说明

- 合集入口：https://www.bilibili.com/video/BV1iVoVBgERD/
- 元数据来源：`bili video <BV> --yaml` 与 B 站公开视频 API。
- 字幕状态：11 期 `subtitle.available` 均为 `false`，没有可直接使用的公开字幕。
- 音频处理：使用 `bili audio <BV> --segment 300` 下载并切分音频。
- 转写处理：使用 `mlx_whisper --model mlx-community/whisper-large-v3-turbo --language zh` 本地转写。
- 缓存位置：`data/audio/<序号-主题>/transcripts-large/`。
- 输出边界：本文档集只输出结构化总结、时间线、分析和少量短引文，不输出完整逐字稿。

## 一句话总览

这 11 期共同记录了 2025-2026 年中国 AI 产业从“模型能力追赶”进入“Agent 产品、Agentic LLM、Post-train/RL、世界模型、数据闭环、形式化数学和组织工程”的新阶段。早期几期讲应用创业如何找形态，中段讲模型公司如何处理开源、商业化和终端，后段把问题推进到环境、数据、世界表征和可验证推理。

## 11期索引

| 序号 | 访谈 | BV | 发布时间 | 时长 | 单篇总结 |
| --- | --- | --- | --- | --- | --- |
| 01 | 肖弘 / Manus 诞生复盘 | `BV1N7oBYNEoU` | 2025-03-23 22:17:45 CST | 1:10:50 | [01-xiaohong-manus.md](videos/01-xiaohong-manus.md) |
| 02 | 明超平 / YouWare 与 Agent 浪潮 | `BV1PDKozTEZJ` | 2025-06-26 18:17:34 CST | 2:38:17 | [02-mingchaoping-youware.md](videos/02-mingchaoping-youware.md) |
| 03 | 陈冕 / Lovart 垂类 Agent | `BV1N2uXzNEBa` | 2025-07-19 11:37:52 CST | 1:44:57 | [03-chenmian-lovart.md](videos/03-chenmian-lovart.md) |
| 04 | 杨植麟 / Kimi K2 与 Agentic LLM | `BV1hFe1zSEXp` | 2025-08-27 13:48:00 CST | 1:39:39 | [04-yangzhilin-kimi.md](videos/04-yangzhilin-kimi.md) |
| 05 | 季逸超 / Manus 出售前访谈 | `BV1knvYBDEjs` | 2025-12-30 18:22:49 CST | 3:31:01 | [05-jiyichao-manus-sale.md](videos/05-jiyichao-manus-sale.md) |
| 06 | 张鹏 / 智谱上市访谈 | `BV1awiDBDEWS` | 2026-01-08 11:25:04 CST | 2:24:36 | [06-zhangpeng-zhipu.md](videos/06-zhangpeng-zhipu.md) |
| 07 | 印奇 / 阶跃星辰与 AI 2.0 | `BV1ZczaBJE58` | 2026-01-26 11:04:24 CST | 2:00:05 | [07-yinqi-stepfun.md](videos/07-yinqi-stepfun.md) |
| 08 | 谢赛宁 / 世界模型与 AMI Labs | `BV1tew5zVEDf` | 2026-03-16 11:30:00 CST | 6:44:38 | [08-xiesaining-world-model.md](videos/08-xiesaining-world-model.md) |
| 09 | 谢晨 / AI 和机器人数据 | `BV1sLX9B4EqD` | 2026-03-30 11:00:00 CST | 2:36:51 | [09-xiechen-data.md](videos/09-xiechen-data.md) |
| 10 | 洪乐潼 / AI for Math 与 Lean | `BV13BdfBoELd` | 2026-04-20 11:00:00 CST | 4:23:11 | [10-hongletong-ai-math.md](videos/10-hongletong-ai-math.md) |
| 11 | 罗福莉 / Post-train 与 Agent 范式 | `BV1iVoVBgERD` | 2026-04-24 11:30:00 CST | 3:34:39 | [11-luofuli-post-train.md](videos/11-luofuli-post-train.md) |

## 三条主线

### Agent 产品创业线

肖弘、明超平、陈冕、季逸超共同回答“Agent 公司到底卖什么”：

- 肖弘强调入口、上下文和非线性判断：应用公司要成为博弈变量。
- 明超平强调创作容器：coding 可能成为大众创作方式。
- 陈冕强调垂直深度：设计场景需要画布、审美、工作流和交付标准。
- 季逸超强调系统实现：Manus 是模型、环境、工具、workflow 和高 token 成本的统一体。

这条线的共同结论是：Agent 不是聊天 UI，而是把模型放进真实工作环境；应用公司的壁垒来自任务上下文、交互、数据飞轮、分发和特定工作流。

### 模型公司路线线

杨植麟、张鹏、印奇、罗福莉共同回答“模型公司下一阶段怎么赢”：

- 杨植麟讲 Agentic LLM：工具泛化、token efficiency、test-time scaling、开源和 API。
- 张鹏讲智谱上市：清华认知智能、GLM/ChatGLM、开源与 2B 商业化。
- 印奇讲 AI 2.0：基础模型、车/机器人终端、软硬一体和商业闭环。
- 罗福莉讲范式切换：Pre-train 到 Post-train，Agent 时代的 RL Infra 和用卡结构。

这条线的共同结论是：Pre-train 追赶之后，模型公司要同时处理 post-train、工具环境、开源生态、终端数据、商业化和组织重构。

### 数据 / 世界模型 / 数学线

谢赛宁、谢晨、洪乐潼共同回答“模型如何获得更可靠的反馈”：

- 谢赛宁指向真实世界和表征学习：语言不是全部，世界模型需要视觉、视频、行动和环境。
- 谢晨指向数据 recipe：数据不是石油，而是教育系统和持续反馈闭环。
- 洪乐潼指向形式系统：Lean 和数学证明提供强验证、强 reward 的推理环境。

这条线的共同结论是：下一阶段能力提升越来越依赖可反馈环境，而不是静态语料。世界、任务轨迹、仿真、证明系统和用户真实 workflow 都会成为训练资源。

## 主题矩阵

| 主题 | 代表访谈 | 核心判断 |
| --- | --- | --- |
| 通用 Agent | 肖弘、季逸超、罗福莉 | 通用 Agent 是产品、系统和训练范式问题，不只是 UI。 |
| 垂类 Agent | 明超平、陈冕、洪乐潼 | 垂直场景有清晰角色、交付物和验证标准，更容易形成早期闭环。 |
| Agentic LLM | 杨植麟、罗福莉 | 模型要围绕工具、环境、长链路任务和 post-training 重新优化。 |
| Post-train / RL Infra | 罗福莉、杨植麟、季逸超 | 真实 Agent 能力需要环境反馈、过程数据和异构训练/推理基础设施。 |
| 数据闭环 | 谢晨、季逸超、罗福莉 | 过程数据、失败到成功轨迹和用户真实任务比静态答案更有价值。 |
| 世界模型 | 谢赛宁、印奇、谢晨 | 物理世界智能需要视觉、终端、机器人/车数据和仿真闭环。 |
| AI for Math | 洪乐潼、罗福莉、谢晨 | 形式化证明提供强验证 feedback，是训练可靠推理的关键入口。 |
| 开源策略 | 肖弘、杨植麟、张鹏 | 开源改变成本、生态和技术传播，但不能简单等同免费商业服务。 |
| 软硬一体 | 印奇、罗福莉、谢晨 | 车、手机、机器人、IoT 终端会牵引模型数据、成本和产品形态。 |
| 组织能力 | 全部访谈 | AI 时代 idea 变便宜，执行密度、人才密度、资源配置和反馈环境更关键。 |

## 人物 / 公司 / 技术路线对照

| 人物 | 公司/产品 | 核心路线 | 主要矛盾 |
| --- | --- | --- | --- |
| 肖弘 | Monica / Manus | 应用入口 + 通用 Agent | 应用层壁垒 vs 模型公司下沉 |
| 明超平 | YouWare | coding as creation | 大众创作需求 vs 模型原生工具竞争 |
| 陈冕 | Lovart | 设计垂类 Agent | 垂直深度 vs 通用 Agent 覆盖 |
| 杨植麟 | Kimi / K2 | Agentic LLM + 开源/工具泛化 | 模型能力 vs 商业化与生态位置 |
| 季逸超 | Manus | 云端环境 + workflow + 数据飞轮 | 通用性 vs 成本、复杂性、可靠性 |
| 张鹏 | 智谱 / GLM | 开源基座 + 2B 商业化 + IPO | AGI 叙事 vs 上市公司收入责任 |
| 印奇 | 阶跃星辰 / 千里科技 | 基础模型 + 终端 + 软硬一体 | 模型投入 vs 硬件/商业长链路 |
| 谢赛宁 | AMI Labs | 世界模型 + 表征学习 | 长期研究路线 vs LLM 主流叙事 |
| 谢晨 | 数据产业 | 数据 recipe + 数据闭环 | 数据价值归因 vs 采集/验证成本 |
| 洪乐潼 | Axiom | AI for Math + Lean | 形式化可靠性 vs 语料/落地稀缺 |
| 罗福莉 | 小米大模型 / MiMo-V2 | Post-train + RL Infra + Agent 范式 | 训练范式切换 vs 组织/算力重排 |

## 推荐阅读顺序

1. 想理解 Agent 应用创业：先读 [肖弘](videos/01-xiaohong-manus.md)、[季逸超](videos/05-jiyichao-manus-sale.md)，再读 [明超平](videos/02-mingchaoping-youware.md)、[陈冕](videos/03-chenmian-lovart.md)。
2. 想理解模型公司路线：先读 [杨植麟](videos/04-yangzhilin-kimi.md)，再读 [罗福莉](videos/11-luofuli-post-train.md)，然后读 [张鹏](videos/06-zhangpeng-zhipu.md)、[印奇](videos/07-yinqi-stepfun.md)。
3. 想理解下一代训练资源：先读 [谢晨](videos/09-xiechen-data.md)，再读 [谢赛宁](videos/08-xiesaining-world-model.md)、[洪乐潼](videos/10-hongletong-ai-math.md)。
4. 想快速建立全局图：按本索引 01-11 顺序读，能看到从应用、模型、终端、数据到形式化反馈的递进。

## 综合判断

1. Agent 的本质是环境化。它把模型从一次问答带入工具、文件、浏览器、代码、车、机器人、数学证明等环境。
2. Post-train 的地位上升。Pre-train 仍重要，但 Agent 能力更依赖任务环境、RL、过程数据、评测和推理系统。
3. 数据变成动态教育系统。未来更有价值的是过程、反馈、失败修正、仿真和可验证任务，而不是静态语料规模。
4. 终端会重新变重要。手机、车、机器人、IoT 不是单纯分发入口，而是模型获取世界反馈和商业闭环的地方。
5. 商业化不会自动发生。应用公司、模型公司、数据公司、Neo Labs 都要证明自己能从能力转化为现金流或长期资本可接受的里程碑。
6. 组织能力是共同瓶颈。新范式下经验折旧更快，最重要的是把人放进高反馈、高实验密度、跨职能协作的环境。

## 文件结构

```text
summaries/ai_taojinniandai/
├── summary.md
├── README.md
└── videos/
    ├── 01-xiaohong-manus.md
    ├── 02-mingchaoping-youware.md
    ├── 03-chenmian-lovart.md
    ├── 04-yangzhilin-kimi.md
    ├── 05-jiyichao-manus-sale.md
    ├── 06-zhangpeng-zhipu.md
    ├── 07-yinqi-stepfun.md
    ├── 08-xiesaining-world-model.md
    ├── 09-xiechen-data.md
    ├── 10-hongletong-ai-math.md
    └── 11-luofuli-post-train.md
```
