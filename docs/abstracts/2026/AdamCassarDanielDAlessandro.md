---
title: "The Bot Might Be Your Customer - Rethinking Traffic Management"
description: "Automated traffic used to be easy to reason about. A person was a customer; a bot was something to block. That model no longer works. A search crawler may bring you business."
image: "images/speakers/headshots/AdamCassar.png"
card: "summary"
---

<div class="cc-header-row" markdown>
<div class="cc-heads" markdown>
![Adam Cassar](../../images/speakers/headshots/AdamCassar.png){ .cc-head } ![Daniel D'Alessandro](../../images/speakers/headshots/DanielDAlessandro.png){ .cc-head }
</div>
<div class="cc-share-row"><span class="cc-share-label">Share</span><a class="cc-share cc-share--li" href="https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAdamCassarDanielDAlessandro%2F" target="_blank" rel="noopener" aria-label="Share on LinkedIn">in</a><a class="cc-share cc-share--x" href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAdamCassarDanielDAlessandro%2F&amp;text=The%20Bot%20Might%20Be%20Your%20Customer%20-%20Rethinking%20Traffic%20Management%20%E2%80%94%20Adam%20Cassar%20%26%20Daniel%20D%27Alessandro%20at%20CloudCon%20Sydney%202026" target="_blank" rel="noopener" aria-label="Share on X">X</a><a class="cc-share cc-share--fb" href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fcloudcon.au%2Fabstracts%2F2026%2FAdamCassarDanielDAlessandro%2F" target="_blank" rel="noopener" aria-label="Share on Facebook">f</a></div>
</div>

# The Bot Might Be Your Customer - Rethinking Traffic Management

<p class="cc-byline" markdown>
**Adam Cassar** &middot; Co-Founder & Head of Security Engineering, Peakhour.io<br>**Daniel D'Alessandro** &middot; Co-Founder & Head of Performance and Delivery, Peakhour.io
</p>

*Full length talk (20 minutes)*

## Abstract

Automated traffic used to be easy to reason about. A person was a customer; a bot was something to block. That model no longer works.

A search crawler may bring you business. An AI shopping agent may be acting for a real customer. A partner might call your API thousands of times a day. The same application is also dealing with scrapers, credential stuffing, residential proxy networks and bots running full browsers. They can look similar at the edge, but they should not receive the same response.

This talk is about making that decision. I'll show how route, account outcomes, network fingerprints, bot signals, cache state and recent behaviour can be used to group traffic without pretending they prove identity. We will then decide what to do with it: let it through, slow it down, serve it from cache, move it to an API, challenge it or block it.

The examples come from operating these controls in production: IP-based limits defeated by address rotation, useful crawlers overwhelming origins, full-page caching absorbing Layer 7 attacks, and policies that reduced cost without treating every unusual client as an attacker.

Traffic management is no longer a human-versus-bot filter. It is a way to decide what work a request may do and how much of your application it may consume.

## About Adam Cassar

Adam Cassar is Co-Founder and Head of Security Engineering at Peakhour. He has spent more than 20 years working in large-scale infrastructure and software development.

His work focuses on traffic that is difficult to classify and expensive to get wrong: automated clients, residential proxies, abusive APIs, aggressive crawlers and Layer 7 attacks. He builds and operates controls spanning bot management, network fingerprinting, rate limiting, application security, caching and origin protection.

Adam speaks and writes about the practical trade-offs in these systems, particularly how to control automation without mistaking a technical signal for identity or blocking useful traffic.

## About Daniel D'Alessandro

Daniel is co-founder of Peakhour.io, an Australian CDN and web application security platform. He has more than 25 years' experience across software development, web performance, cloud infrastructure and application security.

His current focus is bot and traffic management, including browser and network fingerprinting, residential proxy detection, rate limiting and techniques for identifying abusive automated traffic at the edge. He works closely with organisations dealing with the practical impact of bots, from infrastructure cost and performance problems through to credential stuffing, scraping and application abuse.

---

[&larr; All speakers](../../speakers.md)
