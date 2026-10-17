---
title: "Feature Flags interactive tutorial"
excerpt: "An interactive, browser-based tutorial on feature flags using OpenFeature and flagd to separate deployment from release.<br/><img src='/images/feature_flags_tutorial.png'>"
collection: portfolio
date: 2025-03-01
---

This interactive tutorial teaches feature flags, a technique that lets teams deploy new code without immediately releasing it to users. It runs on the Killercoda learning platform, where each learner gets a ready-made environment with a working application, and the tutorial guides them through changing its behaviour.

The tutorial explains how feature flags separate the deployment of code from its release to users, which is useful among other situations for dogfooding, A/B testing and gradual rollout. The exercises use OpenFeature, the vendor-neutral standard, together with the open-source flagd evaluation engine. Learners perform exercises such as switching a hidden feature on while the application is running, creating flags of their own, writing targeting rules that show a feature only to selected users based on evaluation context, and configuring multiple variants with a percentage-based rollout. The tutorial provides detailed explanations as well as solution files for anyone who gets stuck.

Designing the tutorial required looking at DevOps knowledge from a new perspective and creating scenarios that build upon each other to communicate their ideas effectively to an unfamiliar audience.

View the [interactive tutorial](https://killercoda.com/eryngia/scenario/feature-flags) or [source code](https://github.com/eryngia/dd2482-tutorial).

![Feature flags](/images/feature_flags_tutorial.png)