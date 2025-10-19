# High-Performance Scalable Go Applications on Linux

**A Practical Guide to Building, Profiling, and Troubleshooting**

> Build, profile, and harden production-grade Go services on Linux—by actually shipping one: a cost-saving, S3-compatible hot cache proxy with full observability.

---

## Why this book?

This is a **one-stop handbook** for starting complex Go projects the right way: **observability first**. From commit #1 you’ll wire **Linux system metrics, tracing, and dashboards** so bottlenecks surface immediately—on **bare servers, inside VMs, in Docker/Podman containers, and in layered combos** (e.g., **KVM host → guest VM → container**). No hand-wavy theory: you get **copy-paste commands**, **Grafana panels to watch**, and **what “healthy” looks like**—so when performance dips, you know exactly where to look (host vs. guest vs. cgroup vs. app).

---

## What you’ll learn

* **Day-1 production skeleton:** repo layout, Makefile/CI, config, health checks, `/debug/pprof`, structured logs, metrics, and traces—ready to run anywhere.
* **Host/VM/container visibility without guesswork:** concrete checks for **CPU run queues and steal time**, **cgroup throttling**, **GC/alloc pressure**, **disk queue depth & I/O latency**, **TCP retransmits/drops**, **softirq saturation**, and **file-descriptor/backlog limits**—plus the exact **Grafana dashboards** to confirm each.
* **Runtime control with guardrails:** budgets for latency/CPU/memory, safe tuning of `GOMAXPROCS` and GC pacing, backpressure/timeouts/retries, and flame-graph/trace workflows to prove wins.
* **Repeatable perf loop:** baseline → load → profile/trace → change → verify → enforce with CI perf budgets and alerts.
* **Deploy anywhere, see everything:** consistent dashboards and alerts for **bare metal**, **VMs**, **containers**, and **mixed stacks**, so signals stay comparable across environments.
* **All of this while building a real service** you can run in production.

**Target audience:** Intermediate-to-advanced Go engineers who want **practical commands and dashboards—not lectures—**to keep complex services fast and stable across host/VM/container boundaries.

---

## The capstone project: an S3 hot cache proxy

You’ll build an **S3-compatible local proxy** that serves hot objects from **memory + disk**, streams large payloads, supports range requests, and exposes first-class signals (hit/miss, byte-savings, tail latency, saturation). Why this example?

* **It saves real money:** By serving repeat reads locally, you **cut AWS S3 egress** and reduce upstream `GET` volume—material savings for teams with **big data** in S3 (analytics/ML pipelines, media, logs).
* **It forces real trade-offs:** eviction policy (e.g., TinyLFU/LRU), consistency semantics, error/backoff behavior, and concurrency patterns—all measurable via the dashboards you install on day one.
* **It proves portability:** the same binary, metrics, and Grafana views work **on bare Linux**, **inside a VM**, or **in Docker/Podman on that VM**, so you can pinpoint whether a slowdown is the **host**, the **hypervisor**, the **container**, or the **app**.

By the end, you won’t just “know” what to do—you’ll have **a running, observable service** and a **playbook of commands and dashboards** you can reuse on every Go system you touch.
