---
title: "Who's Stealing My CPU? Catching Noisy Neighbours with eBPF on Kubernetes"
description: "Your pod's CPU usage looks green. Requests and limits are set correctly, and kubectl top shows nothing alarming. Yet application latency is spiking. The hidden cause?"
image: "images/speakers/headshots/OlgaMirensky.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Olga Mirensky](../../images/speakers/headshots/OlgaMirensky.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FOlgaMirensky%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FOlgaMirensky%2F&amp;text=Who%27s%20Stealing%20My%20CPU%3F%20Catching%20Noisy%20Neighbours%20with%20eBPF%20on%20Kubernetes%20%E2%80%94%20Olga%20Mirensky%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FOlgaMirensky%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# Who's Stealing My CPU? Catching Noisy Neighbours with eBPF on Kubernetes

<p class="cc-byline" markdown>
**Olga Mirensky** &middot; Senior Staff Site Reliability Engineer, Ping Identity
</p>

*Full length talk (20 minutes)*

## Abstract

Your pod's CPU usage looks green. Requests and limits are set correctly, and kubectl top shows nothing alarming. Yet application latency is spiking. The hidden cause? A noisy neighbour sharing the same node is winning scheduling, and standard Kubernetes metrics are completely blind to it.

Standard metrics track CPU utilisation and throttling, but they cannot measure CPU contention - the delay an application experiences waiting in the kernel run-queue to get CPU time. Building on Netflix's eBPF research into measuring kernel run-queue latency, this talk bridges the gap between raw eBPF code and a practical Kubernetes pattern, complete with monitoring dashboards.

I'll walk through deploying an eBPF collector via a Kubernetes DaemonSet that aggregates scheduling latency directly inside the kernel with minimal overhead, then export these metrics into Prometheus and explore them on live dashboards.

You'll leave with an open-source end-to-end pattern you can deploy in your own clusters, along with an understanding of how eBPF opens up visibility into other invisible node-level bottlenecks - from disk I/O queuing to memory contention.

## Speaker Bio

Olga is a Senior Staff SRE at Ping Identity with deep roots in Kubernetes, GitOps, FinOps, performance and cloud-native systems. She has spent her career building platforms and developer tooling across large enterprises in tech and financial services industries. When she's not working on side projects or tinkering on her never-ending side projects, or playing with new DGX Spark, she is either running half marathons with friends or camping in the woods.

---

[&larr; All speakers](../../speakers.md)
