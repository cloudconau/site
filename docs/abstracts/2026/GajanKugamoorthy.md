---
title: "Provenance for AI Agent Skills"
description: "We have spent a decade learning to secure the software supply chain: signed images, SBOMs, provenance attestations."
image: "images/speakers/headshots/GajanKugamoorthy.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Gajan Kugamoorthy](../../images/speakers/headshots/GajanKugamoorthy.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FGajanKugamoorthy%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FGajanKugamoorthy%2F&amp;text=Provenance%20for%20AI%20Agent%20Skills%20%E2%80%94%20Gajan%20Kugamoorthy%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FGajanKugamoorthy%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# Provenance for AI Agent Skills

<p class="cc-byline" markdown>
**Gajan Kugamoorthy** &middot; Senior Consultant, Vivanti
</p>

*Full length talk (20 minutes)*

## Abstract

We have spent a decade learning to secure the software supply chain: signed images, SBOMs, provenance attestations. AI Agents quietly reopened the hole. The SKILL.md, CLAUDE.md, and tool-definition files that drive agent behaviour are just text, they're pulled from public registries, and almost nobody verifies them. Early 2026 made the consequences concrete: Snyk's first audit of the agent-skills ecosystem scanned roughly 4,000 skills and found over a third carried a security flaw, 534 critical, with 76 confirmed-malicious payloads - on a marketplace with no signing, no review, and no sandbox by default.

In this proposed talk, I will show how to sign agent instructions and reject anything that has been tampered with, before the agent reads a single line. Specifically,  I will walk through treating an agent skill the way we already treat a container image: sign it with Sigstore, and verify provenance at load time so an unsigned or modified skill never executes. Then I will show the defence-in-depth layer - even a correctly signed skill is contained, because signing proves where a skill came from, not that it's safe. To make it concrete I plan to  use nono (open source too from Sigstore's creator, https://github.com/always-further/nono), which already signs CLAUDE.md/SKILL.md with keyless Sigstore and blocks unsigned or tampered instructions at the kernel level.

As an audience, you will leave knowing how to sign your agents' instruction files and block any tampered or unverified skill before it ever runs - bringing the same supply chain rigour you already apply to container images to the prompts and skills that control your agents.

## Speaker Bio

As a Senior Consultant at Vivanti, Gajan specialises in cloud infrastructure, security, and cloud data platforms. Most of his recent hands-on work is building enterprise-grade agentic AI platforms and securing them (e.g. AWS Bedrock AgentCore), which is exactly where this talk's threat model lives. He has extensive experience leading large-scale Kubernetes platform modernisation programs for major Australian banks and architecting secure cloud data platforms for health device manufacturers, and is one of only a handful of CNCF Kubestronauts in Australia, as well as a KCD Melbourne organiser.

His deep technical expertise is built on a foundation of over 7 years at IBM, where he developed cloud native security solutions and contributed to more than 15 patents. Recognised by IBM as an award-winning open-source contributor, Gajan is a key contributor to a diverse range of projects, including OpenSSF's Minder, Red Hat's open-cluster-management.io, and Integrity Shield. This hands-on, real-world experience gives him a practical perspective on building the secure platforms he will discuss in his talk.

---

[&larr; All speakers](../../speakers.md)
