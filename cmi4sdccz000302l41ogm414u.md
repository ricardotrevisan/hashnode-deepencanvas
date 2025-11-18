---
title: "Chaos Engineering: prepare for the worst-case scenario"
datePublished: Tue Nov 18 2025 16:26:48 GMT+0000 (Coordinated Universal Time)
cuid: cmi4sdccz000302l41ogm414u
slug: chaos-engineering-prepare-for-the-worst-case-scenario
cover: https://raw.githubusercontent.com/ricardotrevisan/ricardotrevisan.github.io/master/images/image_20251118.png
tags: sre, cloudcomputing, redundancy, edgecomputing, digitaleconomy, sitereliabilityengineering, chaosengineering, multiprovider

---

Can your business withstand a full day offline?
If the answer is “yes,” you’re not operating in true digital.  
If it’s “no,” you live the dilemma we all face: balancing effort, cost, and risk all the time.

In the Digital Economy, unstable service isn’t a nuisance — it’s **loss, friction, and churn**.

Cloudflare’s outage today wasn’t an “incident.”  
It was a **systemic event**, with a cascading effect: sales stalled, APIs failing, internal access blocked, operations paralyzed.

Why?

Because we concentrated too much on a single edge provider.

Just yesterday we talked about this in the context of AI: **centralization brings short-term efficiency and long-term fragility**.

Cloudflare became “infrastructure of the infrastructure.”  
When it fails, the impact echoes across the Internet. Those who’ve lived through it know: when the edge gives way, the rest collapses too.

And the uncomfortable truth remains: **this shouldn’t knock anyone offline. But it did.**

---

# **Concentration = Fragility**

The adoption of Cloudflare as an all-in-one solution exploded:

* DNS
* CDN
* Reverse Proxy
* WAF
* Zero Trust
* Tunnels / VPNs
* Workers / KV / Durable Objects

Yes, it’s convenient.  
Yes, it reduces complexity.  
But convenience comes with a price — and it’s always paid at the worst moment.

When 60% of your operations depend on a single provider, you create **correlated risk**.  
A partial incident becomes a total collapse.

Today it became evident: companies without alternate DNS, without fallback, and without a secondary edge **disappeared from the Internet**.

It’s not Cloudflare’s fault. It’s an architectural fault.

---

# **Redundancy isn’t a luxury — it’s survival**

Resilience isn’t something a vendor delivers. It’s a design consequence.

And that’s exactly what separates resilient companies from vulnerable ones.

---

## **1. Multi-Provider DNS (mandatory)**

If DNS goes down, nothing else comes up. Plain and simple.

Robust model:

* Cloudflare + Route53, NS1, or Akamai
* 60–300s TTL
* External health checks

That alone would have prevented half of today’s collapses.

---

## **2. Redundant CDN (Fastly / Akamai / Edgio)**

Hardly anyone does it — until the day you need it.

Ideal architecture:

* Cloudflare as primary
* Fastly or Akamai as secondary
* Routing via weighted DNS, GTM, or NS1 Pulsar

If the primary edge drops, traffic flows to the other. No pain, no panic.

---

## **3. Real Fallback Reverse Proxy**

One entry gate invites trouble.

* Cloudflare as primary proxy
* AWS Global Accelerator or distributed NGINX as the alternate route
* Cross-checked health checks

When one goes down, the other takes over. Simple. Effective.

---

## **4. WAF in Two Layers**

Relying on a single WAF left companies blind today.

The right approach:

* Cloudflare WAF as Layer A
* AWS WAF or Fastly Next-Gen as Layer B
* Replicated core rules

Critical security demands critical redundancy.

---

## **5. Zero Trust: don’t put everything in Cloudflare**

Whole teams were cut off from their own infra because they only had one tunnel.

There are several coexistence options (Zscaler, for example.)

* Tailscale
* Zscaler
* Perimeter81
* OpenZiti

A secondary route — even if limited — saves the day.

---

## **6. Multi-Edge and Multi-Cloud: true architecture**

This isn’t a trend, it isn’t hype. It’s the only way to reduce simultaneous failure.

A mature design includes:

* Distributed edge (Cloudflare + Fastly/Akamai)
* Replicated backends (even when cold)
* Cross-region replicated databases
* Independent queues (Kafka + SQS/Kinesis)
* Logs and monitoring outside the primary provider

That’s engineering. That’s maturity.

---

# **Chaos Engineering: test or pretend?**

Having redundancy and not testing is theater. And theater doesn’t protect anyone.

Practices that keep operations alive:

* Simulate Cloudflare outages monthly
* Measure real failover, not imagined
* Automate DNS/CDN switchover
* Maintain tested and versioned runbooks
* Monitor via independent providers

Waiting for “everything to work” isn’t SRE. It’s faith — and faith doesn’t secure any system.

---

# **The naked truth**

Cloudflare isn’t the problem.  
Any provider can fail — and will fail.

The mistake is relying on just one.

Mature companies distribute risk. Naive ones centralize.

Today it’s clear who’s in which group.

---

# **Conclusion: turn outage into a turning point**

Today’s incident exposed a comforting illusion: that centralized simplicity is sufficient.

If your company went down today, it wasn’t Cloudflare who failed. It was your design.

And there are now only two routes:

1. Stay vulnerable and hope for luck.
2. Restructure the architecture and stop being hostage to a single provider.

The second option requires investment, effort, and maturity. But it buys something non-negotiable:

**business continuity.**

In the digital world, continuity isn’t a detail. It’s power.

#ChaosEngineering #SiteReliabilityEngineering #SRE #Redundancy #EdgeComputing #MultiProvider #CloudComputing #ChaosEngineering #DigitalEconomy