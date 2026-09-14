---
title: "Who Load-Tests the Load Tester? 25 Million VUs and Everything That Broke"
description: "I am going to talk about the method and lessons learned from pushing Grafana's load testing platform, k6, to its limits."
image: "images/speakers/headshots/AyushGoyal.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Ayush Goyal](../../images/speakers/headshots/AyushGoyal.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAyushGoyal%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAyushGoyal%2F&amp;text=Who%20Load-Tests%20the%20Load%20Tester%3F%2025%20Million%20VUs%20and%20Everything%20That%20Broke%20%E2%80%94%20Ayush%20Goyal%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAyushGoyal%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# Who Load-Tests the Load Tester? 25 Million VUs and Everything That Broke

<p class="cc-byline" markdown>
**Ayush Goyal** &middot; Senior Software Engineer, Grafana Labs
</p>

*Full length talk (20 minutes)*

## Abstract

I am going to talk about the method and lessons learned from pushing Grafana's load testing platform, k6, to its limits. The goal was to sustain 25 million concurrent users hitting a real streaming media API. Scaling from 1.6 million to 25 million virtual users became a tour through every layer of the infrastructure that quietly assumes nobody will ever push it this hard.

Along the way, we ran into several unexpected bottlenecks:

- A single load balancer saturated quite early so we had to use a Network Load Balancer
- Receiving nodes hit kernel-level walls like CPU pinned on softirq, then the connection table filling up, before application code became the bottleneck
- Our mathematical distribution algorithms started taking ~80-90 seconds up from 100-200 ms
- Several control plane issues & timeouts

Every failure whether in networking, the Linux kernel, distributed algorithms, or the control plane exposed a different scalability assumption that only became visible at extreme scale.

This talk is a practical walkthrough of what broke, how we diagnosed each issue, and the engineering changes that ultimately allowed us to reach 25 million concurrent virtual users.

## Speaker Bio

Ayush is a Senior Software Engineer at Grafana Labs. Previously, he was working at Postman and before that, he was the CTO at Anveshan and earlier an SWE at Rippling. He is passionate about building software and also tinkers around with hardware at times. He is also a certified scuba diver and an avid coin collector.

---

[&larr; All speakers](../../speakers.md)
