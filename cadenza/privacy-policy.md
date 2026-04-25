---
layout: default
title: "Privacy Policy · 鹿动 Cadenza"
permalink: /cadenza/privacy-policy/
last_updated: 2026-04-25
---

# 鹿动 Cadenza — 隐私政策 / Privacy Policy

**生效日期 / Effective**: 2026-04-22  
**适用版本 / Applies to**: Cadenza Watch App 1.0 及之后所有版本

---

## 一、数据收集

Cadenza **不会**收集任何可识别到你本人的数据(姓名、邮箱、手机、设备唯一标识等)。
app 在本机保存以下会话数据:

| 数据 | 来源 | 用途 | 是否上传 |
|---|---|---|---|
| 挑战 / 训练会话(时长、计数、频率) | 用户交互 + CoreMotion | 统计回顾、成就判定 | ❌ 不上传 |
| 实时心率(bpm) | HealthKit | 心率区间挑战、卡路里估算 | ❌ 不上传 |
| 手腕温差、HRV(可选) | HealthKit | 长期趋势 | ❌ 不上传 |
| 用户模式(自由 / 投入 / 自律) | 用户选择 | 决定 app 可见功能 | ❌ 不上传 |
| 加速度 / 陀螺仪 | CoreMotion | 计数、节奏检测 | ❌ 不上传 |

---

## 二、数据存储

- 所有上述数据都保存在**你手表本机**的 `UserDefaults` 中。
- app **没有服务器**,不使用任何第三方云存储。
- app **没有**集成第三方分析 SDK(Firebase / Sentry / Mixpanel 等)、广告 SDK、A/B 测试平台。

---

## 三、数据共享

Cadenza 自己**从不**主动共享你的数据。以下两个场景由**你自己**决定是否分享:

1. **导出 JSON**:设置 → 数据 → 导出。生成本地 JSON,由你通过 AirDrop / 消息发给你选的接收方。
2. **HealthKit 写回**(未来版本):如果你明确授权,会把挑战时长/心率写入 Apple 健康。数据仅留在你的苹果账户内,不经过我们。

---

## 四、HealthKit

- **读取**: 心率、静息心率(在心率区间挑战 / 边缘挑战期间)。
- **写入**: 暂无。未来版本计划写入挑战 Workout,届时会单独弹授权提示。

HealthKit 数据 **永不会** 被 app 传输出设备。

---

## 五、权限

| 权限 | 作用 | 拒绝后的降级行为 |
|---|---|---|
| Motion & Fitness | 挑战计数、节奏检测 | 挑战无法正常工作 |
| HealthKit | 心率区间挑战 / 卡路里 | 该挑战不可用,其他挑战正常 |
| Bluetooth | 连接兼容的 BLE 触觉反馈外设(可选) | 仅无法使用外设联动 |
| 本地通知 | 到期释放日 9 点提醒 | 仅无提醒 |

---

## 六、数据删除

你可以随时:

- **设置 → 数据 → 清除所有记录** — 清空挑战/训练记录
- **设置 → 数据 → 重置所有进度** — 同时清除成就、XP、连击、最佳纪录、连续天数状态、手动打卡等

重置后无法恢复。

---

## 七、儿童隐私

Cadenza 面向成年人设计,**仅供 18 岁以上成年人使用**。app 首次启动会要求年龄确认。
我们不会故意收集 13 岁以下儿童的数据,也不对未成年使用承担任何责任。

---

## 八、外设免责

如你将本 app 与第三方触觉反馈类外设配对使用:

- 请严格遵守该外设厂家的说明书与安全提示。
- 装有起搏器、妊娠、癫痫、严重心脏病等情况的人群,禁止使用任何形式的电刺激外设。
- 从低强度开始,出现任何不适立即停止使用并断开连接。
- 开发者不对因错误使用外设导致的人身或健康风险负责。

---

## 九、变更

本政策变更时我们会更新顶部的 "Effective" 日期,并在 app 内的隐私政策页反映新内容。
重大变更(例如新增远程数据上传)会在下一次 app 启动时弹窗提示。

---

## 十、联系

- GitHub Issue: https://github.com/Huier-git/Cadenza/issues
- Email: 请在 GitHub profile 查看

---

# English version (summary)

Cadenza stores all workout / challenge / heart-rate data **on your Apple Watch only**.
We don't have a server. We don't use third-party analytics or ads SDKs.
HealthKit data is read only for the features you use, and never leaves your device.
You can wipe all data via Settings → Data → Reset All Progress.
The app is intended for users 18 or older.
