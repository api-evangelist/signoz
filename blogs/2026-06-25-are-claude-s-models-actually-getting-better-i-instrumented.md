---
title: "Are Claude’s Models Actually Getting Better? I Instrumented Claude Code to Find Out"
url: "https://signoz.io/blog/claude-code-model-comparison"
date: "2026-06-25"
author: "hello@signoz.io (SigNoz Inc)"
feed_url: "https://signoz.io/rss/"
---
Benchmark scores tell you whether a model solved a task, not what it cost to get there. I instrumented Claude Code with OpenTelemetry and SigNoz to compare Claude Sonnet 4.6, Opus 4.7, and Opus 4.8 across accuracy, cost per solved task, tokens, cache utilization, error rate, and active time, on a fixed Terminal-Bench task suite.
