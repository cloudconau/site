---
title: "Building Hybrid AI Systems: Edge Inferencing Meets Cloud Reasoning"
description: "Modern AI applications increasingly need to run closer to where data is generated and decisions are made."
image: "images/speakers/headshots/ShengChen.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Sheng Chen](../../images/speakers/headshots/ShengChen.png){ .cc-head } ![Frank Fan](../../images/speakers/headshots/FrankFan.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FShengChenFrankFan%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FShengChenFrankFan%2F&amp;text=Building%20Hybrid%20AI%20Systems%3A%20Edge%20Inferencing%20Meets%20Cloud%20Reasoning%20%E2%80%94%20Sheng%20Chen%20%26%20Frank%20Fan%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FShengChenFrankFan%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# Building Hybrid AI Systems: Edge Inferencing Meets Cloud Reasoning

<p class="cc-byline" markdown>
**Sheng Chen** &middot; Sr. Solutions Architect, AWS<br>**Frank Fan** &middot; Principal Container Solution Architect, AWS
</p>

*Full length talk (20 minutes)*

## Abstract

Modern AI applications increasingly need to run closer to where data is generated and decisions are made. This session presents an architectural pattern for hybrid AI systems that split latency-sensitive inference at the edge from cloud-native reasoning, connected through a shared memory layer.

Using a real-world warehouse safety monitoring system as the case study, we examine the trade-offs for placing a Vision Language Model (VLM) on edge GPUs using a hybrid Kubernetes architecture, while delegating summarisation and conversational retrieval to a cloud-based agent runtime.

We cover the decision framework for what runs where, agentic memory strategies, and cross-environment observability.

Key takeaways:

- A decision framework for what belongs at the edge vs. the cloud
- Choosing the right models for your edge applications
- Squeezing performance with quantisation, decoding and cold-start optimisation
- Observing GPU and model health across hybrid environments
- Using a shared memory layer to turn edge inference into business insight

Attendees will leave with practical patterns for building their own hybrid AI systems - from the edge/cloud decision boundary through to agentic memory and cross-environment observability.

## About Sheng Chen

Sheng Chen is a Sr. Solutions Architect at AWS Australia, bringing over 20 years of experience in IT infrastructure and cloud architecture. In his current role, Sheng helps customers accelerate cloud migrations and infrastructure modernisation by leveraging cloud-native technologies. He specialises in Amazon EKS, AWS hybrid cloud services, platform engineering, HPC and AI infrastructure.

## About Frank Fan

Frank Fan, an AWS Principal Container Solution Architect in Australia, has 20+ years of experience in designing and implementing large-scale technology transformations. He specializes in containerization and driving migration initiatives. He has presented at significant IT events like AWS reInvent, AWS Summit and API days. Frank's youtue channel https://www.youtube.com/@gettocloud5719

---

[&larr; All speakers](../../speakers.md)
