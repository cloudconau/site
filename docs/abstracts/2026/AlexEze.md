---
title: "Operators as Data: Why Lifecycle is Not a Separate Problem"
description: "The Operator Lifecycle Manager (OLM) exists because operators were binaries. When the unit of distribution is a binary, lifecycle management—versioning, upgrade, deprecation,…"
image: "images/speakers/headshots/AlexEze.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Alex Eze](../../images/speakers/headshots/AlexEze.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAlexEze%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAlexEze%2F&amp;text=Operators%20as%20Data%3A%20Why%20Lifecycle%20is%20Not%20a%20Separate%20Problem%20%E2%80%94%20Alex%20Eze%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAlexEze%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# Operators as Data: Why Lifecycle is Not a Separate Problem

<p class="cc-byline" markdown>
**Alex Eze** &middot; Infrastructure Developer, NHS
</p>

*Lightning Talk (5 mins)*

## Abstract

The Operator Lifecycle Manager (OLM) exists because operators were binaries. When the unit of distribution is a binary, lifecycle management—versioning, upgrade, deprecation, deletion—becomes a separate problem that requires a separate system. OLM is that system, but it adds its own controllers, its own CRDs, its own installation lifecycle. The overhead is the necessary cost of the binary constraint.

This lightning talk introduces a different model: operators as declarative patterns—data. When the operator is data, lifecycle is not an external concern to manage; it is a built-in property of the artifact. The same model that bakes test results into the artifact at publish time (simulation gates + e2e gates, proof in OCI annotations) governs upgrade, deprecation, and deletion. The proof of correctness travels with the artifact. There is no separate lifecycle system to install. You write patterns, and the lifecycle comes with them.

We'll walk through the full lifecycle: creation (ork validate), testing (ork simulate and ork e2e), distribution (ork push with gated proof), consumption (ork inspect and ork pull), upgrade (versioned imports), deprecation (metadata with migration target), and deletion (declarative deletion protection). The lifecycle is not a process running somewhere; it is a record traveling with the artifact.

Attendees will leave with a new mental model: when the operator is data, lifecycle is not a separate problem. The same artifact that carries your operator carries its own proof, its own version, and its own deprecation notice. The lifecycle is expressed in the same language as the operator itself.

This talk will be demonstrated with Orkestra, an open-source declarative runtime for Kubernetes behaviour (Apache 2.0), built on a single idea: operator behaviour is different from operator infrastructure. You declare the behaviour; the runtime provides the infrastructure. All examples and code are from https://github.com/orkspace/orkestra.

## Speaker Bio

Alex Eze is the creator of Orkestra, a declarative runtime for Kubernetes operators. A former clinical pharmacist, currently an Infrastructure Engineer with the NHS. He taught himself to code after a job interview revealed a gap in his Kubernetes operator knowledge — and spent the following years closing that gap, not just for himself but for every engineer who has looked at operator boilerplate and walked away. Orkestra is the result: a runtime built on the idea that your CRD is enough.

---

[&larr; All speakers](../../speakers.md)
