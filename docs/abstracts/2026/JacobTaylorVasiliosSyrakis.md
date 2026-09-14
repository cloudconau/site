---
title: "I'm Behind Seven Proxies: Demystifying Envoy on Kubernetes"
description: "Envoy has become one of the most important building blocks in the cloud-native ecosystem."
image: "images/speakers/headshots/JacobTaylor.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Jacob Taylor](../../images/speakers/headshots/JacobTaylor.png){ .cc-head } ![Vasilios Syrakis](../../images/speakers/headshots/VasiliosSyrakis.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FJacobTaylorVasiliosSyrakis%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FJacobTaylorVasiliosSyrakis%2F&amp;text=I%27m%20Behind%20Seven%20Proxies%3A%20Demystifying%20Envoy%20on%20Kubernetes%20%E2%80%94%20Jacob%20Taylor%20%26%20Vasilios%20Syrakis%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FJacobTaylorVasiliosSyrakis%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# I'm Behind Seven Proxies: Demystifying Envoy on Kubernetes

<p class="cc-byline" markdown>
**Jacob Taylor** &middot; Staff Engineer, Canva<br>**Vasilios Syrakis** &middot; Senior Systems Engineer
</p>

*Full length talk (20 minutes)*

## Abstract

Envoy has become one of the most important building blocks in the cloud-native ecosystem. It powers service meshes, API gateways, ingress controllers and countless bespoke networking platforms through the combination of it's rich feature set paired with runtime reconfiguration through xDS. Yet for many engineers, Envoy remains a black box hidden behind projects like Istio or Envoy Gateway.

This session is designed for Kubernetes practitioners who want to understand Envoy itself. We'll start by building a mental model of Envoy's architecture, explaining the core configuration resources—listeners, filter chains, routes and clusters—and how requests flow through them. From there we'll explore practical features including HTTP connection management, TLS, extension points and the xDS APIs that enable dynamic configuration.

Armed with those fundamentals, we'll examine how Kubernetes projects such as Istio and Envoy Gateway assemble these primitives into higher-level platforms, before showing how you can build your own Envoy-powered solutions using native Kubernetes concepts.

We'll finish with two production case studies that demonstrate how these patterns can be applied to solve real networking problems at scale.

## About Jacob Taylor

Jake is a senior network engineer at Canva with over 9 years of experience in the field. He currently yells at Bazel a lot and occasionally builds network infrastructure. Previously, having worked at organisations such as NTT, AWS, and Atlassian, he has been exposed to a variety of different networks and codebases. When he's not looking at a computer, you can find him cooking, walking, playing video games, and shooting arrows at targets with his bow.

## About Vasilios Syrakis

You may remember Vasilios from his viral layoff video where he reflected on the edge infrastructure that he built over 8 years at Atlassian. He's worked extensively with Envoy Proxy, built an xDS control-plane from scratch, open-sourced it, and used it to power complex requirements across teams. In recent years he joined the cult of Rust. Outside the 9-5, he occasionally does live-streams and produces tech content. Soon to be a Dad, and uses Neovim BTW.

---

[&larr; All speakers](../../speakers.md)
