# 具身智能项目记录 / Embodied AI Portfolio

我是张壮志，北京理工大学硕士生、原力灵机 AI Infra 实习生。这里记录我参与的机器人模型评测、数据采集、训推回归与基础设施工程工作，重点说明做了什么、如何检查结果，以及结论适用于什么条件。

[个人主页](https://zsevene077-cyber.github.io) · [项目说明仓库](https://github.com/zsevene077-cyber/embodied-ai-portfolio) · [编辑与实验记录方法](CONTRIBUTING.md)

## 项目索引 / Projects

| 项目 | 参与内容 | 本次记录的结果与范围 | 详情 |
| --- | --- | --- | --- |
| VLA 评测 | 仿真评测执行、并发与微批配置、覆盖审计 | DM0 / LIBERO Spatial，500 episodes 的单 seed 对比，耗时 55.8 → 32.0 分钟 | [VLA evaluation](projects/vla-evaluation.md) |
| NexArm 数据采集 | 多相机录制、状态读取、转码队列与完整性检查 | 同两条封存录制、3,090 帧，转码耗时 63.517 → 41.265 秒 | [Robot data](projects/robot-data.md) |
| 多模态评测协议 | 任务接入、媒体映射、评分与异常诊断 | 32 个入口：31 个功能出分，27 个严格零异常；各入口测试范围不同 | [Multimodal protocols](projects/multimodal-protocols.md) |
| 评测平台与模型服务 | 配置、提交、服务检查、监控、归档与资源回收 | 按本地检查、云端执行与结果审计分别记录验证范围 | [Evaluation infrastructure](projects/evaluation-infra.md) |
| 训练后回归 | checkpoint 推理检查、四套 LIBERO 评测、恢复执行与覆盖审计 | 2,000 个唯一 episode，1,933 次成功，缺失、重复、越界均为零 | [Training regression](projects/training-regression.md) |

## 如何阅读 / Reading Guide

每篇说明都保留问题背景、本人参与的工作、实验条件、结果及适用边界。性能改善、任务成功率、功能出分和覆盖完整性是不同指标，不能互相替代；仿真或静止设备读取的结果也不能直接视为机械臂运动验收。

这是公开项目说明与个人学习记录仓库。当前内容根据保存的实验记录整理，原始日志、预测数据、模型权重和工作源码不在本仓库中；公开摘要提供的条件尚不足以独立复现全部实验。文中的团队模型、既有框架与本人实习贡献分别描述，不将使用或适配它们写成个人算法成果。

目前没有在此发布项目源代码，也没有提供源代码许可。后续若增加可以公开的材料，会逐项注明来源、验证范围与适用许可。

## 后续编辑 / Future Updates

项目想法与改进记录采用“现状 → 想法 → 实验条件 → 结果 → 结论”的顺序。未执行的想法、局部检查和完整验证分别标注，具体方法及可复制模板见 [CONTRIBUTING.md](CONTRIBUTING.md)。

整理日期：2026-11-20。指标描述的是相应历史实验，不表示当前线上服务状态。
