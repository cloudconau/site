---
title: "The Service Mesh: Solving Microservice Chaos (And When You Actually Need One)"
description: "Microservices promised speed and independence, but for many SREs and developers, they delivered network complexity. Suddenly, we're all part-time network engineers."
image: "images/speakers/headshots/MofesolaBabalola.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Mofesola Babalola](../../images/speakers/headshots/MofesolaBabalola.png){ .cc-head } ![Hannah Olukoye](../../images/speakers/headshots/HannahOlukoye.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FMofesolaBabalolaHannahOlukoye%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FMofesolaBabalolaHannahOlukoye%2F&amp;text=The%20Service%20Mesh%3A%20Solving%20Microservice%20Chaos%20%28And%20When%20You%20Actually%20Need%20One%29%20%E2%80%94%20Mofesola%20Babalola%20%26%20Hannah%20Olukoye%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FMofesolaBabalolaHannahOlukoye%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# The Service Mesh: Solving Microservice Chaos (And When You Actually Need One)

<p class="cc-byline" markdown>
**Mofesola Babalola** &middot; Staff Site Reliability Engineer, Tempo<br>**Hannah Olukoye** &middot; Google Developer Expert | Engineering Manager, mobile.de
</p>

*Full length talk (20 minutes)*

## Abstract

Microservices promised speed and independence, but for many SREs and developers, they delivered network complexity. Suddenly, we're all part-time network engineers. We have to code retry logic, timeouts, and circuit breakers into every service. We struggle to get uniform "golden signal" metrics. And how do we enforce that all 50 of our polyglot services are communicating securely over mTLS?

This is the "microservice tax," and it's holding us back.

Enter the service mesh. You've heard the buzzwords—Istio, Linkerd—but what is a mesh, and what problems does it actually solve? Is it just hype, or is it the key to taming a complex distributed system?

In this session, we'll cut through the marketing and get to the SRE truth. We'll start with the "why," exploring the common, painful reliability and security challenges that emerge at scale. Then, we'll dive into the "what," demystifying the service mesh architecture (control plane vs. data plane) and explaining how it moves all that complex networking logic out of your application and into a sidecar proxy.

We'll cover the three pillars of a mesh:

- **Reliability:** Automatic retries, timeouts, and circuit breakers.
- **Observability:** Uniform metrics, logging, and tracing for every call.
- **Security:** Automatic mTLS (encryption) and fine-grained authorization policies.

But a mesh isn't a silver bullet. It adds a new layer of complexity and operational overhead. The most important question is: "Do we need one?" We'll finish with a practical, hype-free decision-making framework to help you decide when (or if) the benefits of a mesh outweigh the costs for your team. You'll leave knowing what a mesh is, what it does, and whether you should go home and install one.

## About Mofesola Babalola

Mofesola Babalola is a Site Reliability Engineering leader at Tempo Software, where he manages large-scale observability and service mesh systems powering over 5 million users. With deep experience in Kubernetes, Istio, ArgoCD, and AWS, he specializes in building resilient platforms and automating infrastructure at scale. Mofesola has led the adoption of ambient mesh in production, and actively works on improving GitOps workflows for platform teams. He is passionate about sharing practical insights from the intersection of DevOps, SRE, and developer experience.

## About Hannah Olukoye

Hannah is an Engineering Manager who translates complex software engineering concepts into people-centric strategies. Leveraging her background as a software engineer and Google Developer Expert for Android, she now focuses on building platforms that reduce developer cognitive load and empower teams to move faster and safely.

She remains an active mentor, technical writer, and international speaker dedicated to motivating others, especially women, to pursue careers in tech.

---

[&larr; All speakers](../../speakers.md)
