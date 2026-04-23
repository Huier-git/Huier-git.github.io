---
layout: page
permalink: /cn/side/index.html
title: 杂七杂八
lang: zh
---

# 杂七杂八

> 主研究线之外的个人兴趣项目 &mdash; 拿来折腾不同平台、送去上架、看看能不能跑出来。

<br>

#### [Cadenza &mdash; watchOS 节奏训练 App](#)

<div class="img-row">
<img src="/images/projects/cadenza-playhub.png" alt="Cadenza Play Hub — 日目标环与随心率着色的计数 hero">
<img src="/images/projects/cadenza-datacenter.png" alt="Cadenza Data Center — 周活跃分布与按挑战分类占比">
</div>
<p class="img-caption">左：Play Hub 日目标环 &nbsp;&middot;&nbsp; 右：Data Center &mdash; 周活跃分布与按挑战分类占比</p>

个人独立 watchOS app，将手腕节奏与心率信号转换为结构化训练数据。全本地运行、零后端 &mdash; 无分析 SDK、无云端上传。

- **角色** &mdash; 独立设计、开发、提审
- **平台** &mdash; watchOS 10+ &middot; Swift &middot; SwiftUI &middot; Combine
- **时间** &mdash; 2026.03 &ndash; 至今 &middot; v2.0.1（2026-04）
- **状态** &mdash; 代码侧提审就绪，TestFlight 筹备中（健康健美类 17+）

**亮点**

1. **节奏检测** &mdash; 基于 CoreMotion 的摇腕识别，EWMA 平滑 + 幅度自适应标定，按灵敏度档位触发逐拍触觉反馈
2. **HealthKit 训练闭环** &mdash; 实时心率、HRV（SDNN 30天）、静息心率、腕温增量；Karvonen HRR + Tanaka HRmax 推算训练区间；4 种挑战模式（频率 / 起伏 / 时长 / 心率区间）附 S&ndash;D 评级
3. **表盘复杂功能** &mdash; 3 种 family（圆形 / 矩形 / 四角），App Group 快照共享，色温渐变进度弧，Canvas 自绘 7 天 mini-sparkline
4. **成长系统** &mdash; 32+ 成就（Bronze &rarr; Platinum 四档），XP 曲线，连击 streak，28 天历史热力图，11 条规则驱动的 AI 洞察卡（7d / 30d / 90d 多窗）
5. **工程细节** &mdash; 5 种语言本地化（xcstrings，500+ key，Bundle swizzle 运行时热切换）、Reduce Motion 自动降级、scenePhase 驱动的 Widget 刷新、MetricKit 本地诊断

**技术栈** &mdash; `Swift` `SwiftUI` `Combine` `HealthKit` `CoreMotion` `CoreBluetooth` `WidgetKit` `Apple Charts` `xcstrings`

**隐私** &mdash; 所有数据驻留设备，不联网、无分析、无崩溃上报
