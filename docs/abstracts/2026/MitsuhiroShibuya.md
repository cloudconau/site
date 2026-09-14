---
title: "When your circuit breaker backfires — outlier detection in Istio and Envoy"
description: "We turned on a circuit breaker to make one of our services more reliable. Minutes later it was making things worse, and not only there: errors spread to services that had nothing…"
image: "images/speakers/headshots/MitsuhiroShibuya.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Mitsuhiro Shibuya](../../images/speakers/headshots/MitsuhiroShibuya.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FMitsuhiroShibuya%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FMitsuhiroShibuya%2F&amp;text=When%20your%20circuit%20breaker%20backfires%20%E2%80%94%20outlier%20detection%20in%20Istio%20and%20Envoy%20%E2%80%94%20Mitsuhiro%20Shibuya%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FMitsuhiroShibuya%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# When your circuit breaker backfires — outlier detection in Istio and Envoy

<p class="cc-byline" markdown>
**Mitsuhiro Shibuya** &middot; Site Reliability Engineer, Mercari
</p>

*Full length talk (20 minutes)*

## Abstract

We turned on a circuit breaker to make one of our services more reliable. Minutes later it was making things worse, and not only there: errors spread to services that had nothing to do with the change, and traffic kept concentrating onto fewer and fewer pods until they were overwhelmed and crashed. The safety net we had just added had become the problem. Yet nothing was really misconfigured: the setting looked reasonable and passed every automated policy check. What caused the incident was how three things interacted: how the mesh ejects unhealthy pods, how traffic then shifts onto the pods that remain, and what clients do when requests start to fail. Each piece was doing its job; together, they caused a cascade. And the one signal that would have made it obvious was not being collected.

This talk uses that real incident to show how those pieces interact, and then turns to the practical side: how Istio's outlier detection actually behaves, and why Envoy calls it passive health checking rather than circuit breaking. We will look at the settings that make it dangerous, how to combine it with the right load balancing and a retry budget so it contains a failure instead of spreading it, and how to make it observable. You will leave knowing how to use outlier detection safely, without it causing the very failures it is meant to prevent. For anyone running Istio and Envoy on Kubernetes, with no deep service-mesh knowledge required.

## Speaker Bio

Mitsuhiro Shibuya is a Tokyo-based Site Reliability Engineer with nearly a decade of experience dedicated to the art of keeping complex systems running. He began his career as a Backend Engineer with a lasting love for Ruby, and keeps that passion alive through modest contributions to open-source projects. Cat enthusiast.

---

[&larr; All speakers](../../speakers.md)
