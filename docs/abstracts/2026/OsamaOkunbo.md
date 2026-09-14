---
title: "The Day I Found Out My Policies Were Off"
description: "The first time I actually checked which of my admission policies were enforcing, the answer was: not all of them. Namespaces had been excluded that I didn't exclude."
image: "images/speakers/headshots/OsamaOkunbo.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Osama Okunbo](../../images/speakers/headshots/OsamaOkunbo.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FOsamaOkunbo%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FOsamaOkunbo%2F&amp;text=The%20Day%20I%20Found%20Out%20My%20Policies%20Were%20Off%20%E2%80%94%20Osama%20Okunbo%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FOsamaOkunbo%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# The Day I Found Out My Policies Were Off

<p class="cc-byline" markdown>
**Osama Okunbo** &middot; Security Engineer, Immibuddy
</p>

*Full length talk (20 minutes)*

## Abstract

The first time I actually checked which of my admission policies were enforcing, the answer was: not all of them. Namespaces had been excluded that I didn't exclude. Policies I'd set to enforce were sitting in warn only. A webhook config had been deleted and nobody had said anything. The dashboards were green the whole time. I'd been reporting "enforced" and enforcing a fraction of it.

This talk is how that happens, and how I rebuilt it so it stuck.

It happens because engineers don't hate security, they hate a denied deploy at 2am with a Rego error they can't read. So they take the one-line exit: failurePolicy: Ignore, a namespace exclusion, or deleting the ValidatingWebhookConfiguration outright. If the bypass is cheaper than complying, they bypass. That's not their failure, it's mine — I priced the control wrong, and then I didn't watch whether it stayed on.

The rebuild had two halves. First, roll out like you mean to keep it: audit mode before anything, so a policy shows me what it would block before it blocks a real deploy; then warn, then enforce, one namespace at a time; exceptions self-service and expiring, because one that never expires is a hole with paperwork on it. Second, and the part I'd missed entirely: instrument the bypasses. A change to a webhook config pages me now. Namespace exclusions get diffed against a baseline. The quiet disable is the one that hurts, so I stopped trusting the dashboard and started watching the exits.

You'll leave able to check whether your own controls are actually on — most people have never looked — and roll them out so they're still enforcing in six months instead of switched off in six weeks.

## Speaker Bio

Osama Okunbo is a Security and Software Engineer who consults with startups and scaleups on cloud-native security, Kubernetes, and compliance. Before working in tech he competed as a professional Judoka and studied Sports Science, eventually transitioning into software engineering through game development before finding his way into cloud security and DevSecOps. He leads security engineering at Immibuddy, a Canadian immigration SaaS platform, and holds consulting clients in fintech and retail. He is the author of Hello Fraud: Why You Feel Like an Impostor in Tech and How to Fix It and holds an MSc in Cybersecurity from the University of Suffolk. He spoke at Manchester Tech Festival 2025 on agentic AI in cybersecurity.

---

[&larr; All speakers](../../speakers.md)
