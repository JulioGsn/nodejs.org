---
title: Poor Performance - Diagnostics
layout: docs.hbs
---

# Poor Performance

In this document you can learn about how to profile a Node.js process.

- [Poor Performance](#poor-performance)
  - [My application has a poor performance](#my-application-has-a-poor-performance)
    - [Symptoms](#symptoms)
    - [Debugging](#debugging)

## My application has a poor performance

### Symptoms

My applications latency is high and I have already confirmed that the bottleneck
is not my dependencies like databases and downstream services. So I suspect that
my application spends significant time to run code or process information.

You are satisfied with your application performance in general but would like to
understand which part of our application can be improved to run faster or more
efficient. It can be useful when we want to improve the user experience or save
computation cost.

### Debugging

In this use-case, we are interested in code pieces that use more CPU cycles than
the others. When we do this locally, we usually try to optimize our code.

This document provides two simple ways to profile a Node.js application:

- [Using V8 Sampling Profiler](/docs/guides/simple-profiling/)
- [Using Linux Perf](/docs/guides/diagnostics/poor-performance/using-linux-perf)
