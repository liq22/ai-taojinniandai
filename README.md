# AI的淘金年代

这是对 B 站张小珺商业访谈录合集“AI的淘金年代”11 期长访谈的结构化总结，由codex生成。文档基于公开视频元数据、本地音频转写和视频章节信息整理，目标是帮助读者快速理解 2025-2026 年中国 AI 创业、模型公司、Agent、Post-train、世界模型、数据和 AI for Math 的关键观点。

## 阅读入口

- 合集总览与主题矩阵：[summary.md](summary.md)
- 单期详细总结：[videos/](videos/)

## 访谈索引

| 序号 | 访谈 | 单篇总结 |
| --- | --- | --- |
| 01 | 肖弘 / Manus 诞生复盘 | [01-xiaohong-manus.md](videos/01-xiaohong-manus.md) |
| 02 | 明超平 / YouWare 与 Agent 浪潮 | [02-mingchaoping-youware.md](videos/02-mingchaoping-youware.md) |
| 03 | 陈冕 / Lovart 垂类 Agent | [03-chenmian-lovart.md](videos/03-chenmian-lovart.md) |
| 04 | 杨植麟 / Kimi K2 与 Agentic LLM | [04-yangzhilin-kimi.md](videos/04-yangzhilin-kimi.md) |
| 05 | 季逸超 / Manus 出售前访谈 | [05-jiyichao-manus-sale.md](videos/05-jiyichao-manus-sale.md) |
| 06 | 张鹏 / 智谱上市访谈 | [06-zhangpeng-zhipu.md](videos/06-zhangpeng-zhipu.md) |
| 07 | 印奇 / 阶跃星辰与 AI 2.0 | [07-yinqi-stepfun.md](videos/07-yinqi-stepfun.md) |
| 08 | 谢赛宁 / 世界模型与 AMI Labs | [08-xiesaining-world-model.md](videos/08-xiesaining-world-model.md) |
| 09 | 谢晨 / AI 和机器人数据 | [09-xiechen-data.md](videos/09-xiechen-data.md) |
| 10 | 洪乐潼 / AI for Math 与 Lean | [10-hongletong-ai-math.md](videos/10-hongletong-ai-math.md) |
| 11 | 罗福莉 / Post-train 与 Agent 范式 | [11-luofuli-post-train.md](videos/11-luofuli-post-train.md) |

## 资料来源与处理方式

- 合集入口：https://www.bilibili.com/video/BV1iVoVBgERD/
- 元数据：使用 `bili video <BV> --yaml` 获取。
- 字幕：11 期公开视频均未提供可直接使用的公开字幕。
- 音频：使用 `bili audio <BV> --segment 300` 本地切分。
- 转写：使用 `mlx_whisper --model mlx-community/whisper-large-v3-turbo --language zh` 本地转写。
- 输出：只保留结构化总结、时间线、分析和少量短引文，不包含完整逐字稿。

## 引用与版权边界

本文档是学习和研究用途的二次整理，不替代原视频内容。建议引用观点时同时标注原视频 BV 号和对应单篇总结；需要完整语境时请回到 B 站原视频观看。

本仓库不包含原始音频、视频、完整逐字稿或本地转写缓存。

## 目录结构

```text
.
├── README.md
├── summary.md
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
