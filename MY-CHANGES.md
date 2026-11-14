# 我的改动记录

本仓库基于 [Snailclimb/interview-guide](https://github.com/Snailclimb/interview-guide) 二次开发，遵循原项目的 **AGPL-3.0** 协议，保留原作者署名与 LICENSE。

- 上游仓库：https://github.com/Snailclimb/interview-guide
- 同步上游：`git fetch upstream && git merge upstream/master`
- 本仓库定位：个人学习与工程实践，非商业发行

## 我在做什么

目标：在这个项目上完成一套**能演示、能讲清取舍**的改造，重点放在工程化能力（异步任务、失败处理、可观测），而不是把功能再抄一遍。

## 进度

| 阶段 | 内容 | 状态         |
|---|---|------------|
| 环境 | 本地跑通（PostgreSQL/pgvector、Redis、RustFS、模型 API） | ⬜ 搭建中尚未跑通 |
| 主链路 | 简历解析 → 出题 → 多轮问答 → 评估 → 报告 | ⬜ 未开始      |
| 深挖 | 评估异步化（Redis Stream + 状态机） | ⬜ 未开始      |
| 打磨 | 失败场景测试、模块 README、demo 录屏 | ⬜ 未开始      |

## 改动记录

| 日期 | 模块 | 改了什么 | 为什么 | commit |
|---|---|---|---|---|
| 2026-11-14 | 构建 | gradle 发行包地址改为腾讯云镜像 | 官方源下载超时，镜像才拉得到 gradle-9.6.1 | `cb02e7f` |

## 约定

- 模型 Key、数据库口令一律走 `.env`，不入库；
- 每个改动写清「做了什么 / 为什么 / 验证了什么」；
- 保留上游 LICENSE，不修改协议声明。