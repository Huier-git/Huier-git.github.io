---
layout: page
permalink: /side/index.html
title: Side Projects
---

# Side Projects

> Personal, curiosity-driven builds outside the main research line &mdash; where I get to tinker with new platforms, ship to app stores, and see what sticks.

<br>

#### [Cadenza &mdash; watchOS Rhythm Training App](#)

<div class="img-row">
<img src="/images/projects/cadenza-playhub.png" alt="Cadenza Play Hub — daily goal ring with heart-rate-tinted counter">
<img src="/images/projects/cadenza-datacenter.png" alt="Cadenza Data Center — weekly distribution and by-challenge breakdown">
</div>
<p class="img-caption">Left: Play Hub with daily goal ring &nbsp;&middot;&nbsp; Right: Data Center &mdash; weekly distribution and by-challenge breakdown</p>

A personal watchOS app that turns wrist rhythm and heart-rate signals into structured training data. Fully local, zero backend &mdash; no analytics SDK, no cloud upload.

- **Role** &mdash; Solo designer, developer, and submitter
- **Platform** &mdash; watchOS 10+ &middot; Swift &middot; SwiftUI &middot; Combine
- **Timeline** &mdash; 2026.03 &ndash; Present &middot; v2.0.1 (2026-04)
- **Status** &mdash; Submission-ready, TestFlight in prep (Health & Fitness, 17+)

**Highlights**

1. **Rhythm detection** &mdash; CoreMotion-based wrist-shake recognition with EWMA smoothing and magnitude auto-calibration; per-rep haptic feedback tuned by sensitivity profile.
2. **HealthKit training loop** &mdash; Live HR stream, HRV (SDNN 30d), resting HR, wrist-temperature deltas; Karvonen HRR + Tanaka HRmax for zone targeting; 4 challenge modes (Frequency / Surge / Endurance / HR Zone) with S&ndash;D grade scoring.
3. **Widget complications** &mdash; 3 family types (accessoryCircular / Rectangular / Corner) sharing an App Group snapshot pipeline; color-temperature progress arc, 7-day mini-sparkline drawn via Canvas.
4. **Progression system** &mdash; 32+ achievements (Bronze &rarr; Platinum tiers), XP curve, combo streaks, 28-day history heatmap, and 11 rule-based AI insight cards across 7d / 30d / 90d windows.
5. **Engineering craft** &mdash; Localized to 5 languages (xcstrings, 500+ keys, Bundle-swizzle runtime hot-switch), Reduce Motion auto-degrade, scene-phase-driven widget refresh, MetricKit-only local diagnostics.

**Tech stack** &mdash; `Swift` `SwiftUI` `Combine` `HealthKit` `CoreMotion` `CoreBluetooth` `WidgetKit` `Apple Charts` `xcstrings`

**Privacy** &mdash; All data stays on device. No analytics, no crash-reporting SDK.
