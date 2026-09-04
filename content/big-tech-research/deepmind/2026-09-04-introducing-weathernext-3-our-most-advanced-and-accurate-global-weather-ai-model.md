---
title: "Introducing WeatherNext 3, our most advanced and accurate global weather AI model"
date: 2026-09-04
draft: false
tags: ["big-tech-research", "deepmind"]
---

**[Introducing WeatherNext 3, our most advanced and accurate global weather AI model](https://deepmind.google/blog/introducing-weathernext-3-our-most-advanced-and-accurate-global-weather-ai-model/)** — _Google DeepMind · Sep 4_

**Main takeaway:** Google DeepMind and Google Research released WeatherNext 3, which they call the most advanced and accurate global weather model to date based on independent live evaluations by Brightband. It learns directly from real-time observations, including raw satellite data, and puts out an hourly forecast at five times the resolution of the previous version.

**Main methods:**
- **Learns from real-time observations instead of physics simulation.** The model takes raw satellite data as input rather than relying on traditional numerical weather prediction, which is what lets it track fast-changing local weather.
- **Hourly refresh at 5× sharper resolution.** Earlier AI weather models were limited by spatial resolution and had trouble ingesting live observational feeds; WeatherNext 3 regenerates a high-resolution global forecast every hour.
- **New forecast variables.** The release adds more precise precipitation forecasting (rain and snow) plus clean energy variables aimed at renewable generation planning.
- **Independent evaluation.** The "most accurate to date" claim is attributed to live evaluations run by Brightband, not to an internal benchmark.
- **Shipped across Google surfaces.** The model is integrated into Search, Gemini, Maps, Google Maps Platform, and Cloud, so the data is reachable both as consumer forecasts and as an API for third-party projects.
- **Caveat.** The available article text is truncated partway into the resolution section, so architecture, training setup, and head-to-head numbers against WeatherNext 2 aren't in what was fetched.

**[WeatherNext 3：直接吃卫星原始数据的全球天气模型](https://deepmind.google/blog/introducing-weathernext-3-our-most-advanced-and-accurate-global-weather-ai-model/)** — _Google DeepMind · 9月4日_

**Main takeaway:** Google DeepMind 和 Google Research 一起放出了 WeatherNext 3，按 Brightband 做的独立实时评测，这是目前最准的全球天气模型。它直接从实时观测里学，包括卫星原始数据，每小时出一次预报，分辨率是上一代的 5 倍。

**Main methods:**
- **不走物理模拟，直接从实时观测学。** 模型吃的是卫星原始数据，不再依赖传统数值天气预报那一套，所以能跟上变化很快的局地天气。
- **每小时刷新，分辨率提升 5 倍。** 之前的 AI 天气模型卡在空间分辨率上，实时观测数据也很难喂进去；WeatherNext 3 每小时重算一遍全球高分辨率预报。
- **多了几类预报变量。** 这次把降水（下雨下雪）预报做细了，还加了给可再生能源用的 clean energy 变量。
- **独立第三方评测。** "目前最准"这个说法是 Brightband 的实时评测给的，不是自家 benchmark 自说自话。
- **整套接进 Google 产品线。** Search、Gemini、Maps、Google Maps Platform 和 Cloud 都已经用上，普通用户能直接看，开发者也能走 Cloud 把数据接进自己的项目。
- **一个需要注意的点。** 抓到的正文在讲分辨率那段就断了，模型架构、训练细节，以及跟 WeatherNext 2 正面对比的数字都不在里面。
