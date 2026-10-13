# DMIT Premium: How to Pick a CN2 GIA Plan for a China-Facing Site Without Overpaying

People searching "DMIT Premium" usually want one of two answers: is the Premium line worth the markup over DMIT's cheaper options, or which Premium plan should I actually buy. Both questions run into the same problem — the product page tells you the specs but not whether you're paying for something you'll never use.

What follows is what the Premium profile actually is, what it costs across DMIT's three locations, and where the money is genuinely well spent.

## What "Premium" actually means at DMIT

DMIT sorts its VPS catalog by network profile first, size second. Three profiles exist: Tier 1, Eyeball, and Premium — the last one abbreviated as `.Pro` in every plan name, which is why you'll see things like `LAX.AS3.Pro.TINY`.

DMIT's own wording for the Premium profile is uncharacteristically plain:

> "This profile includes Tier 1 + all Premium Transit providers, such as DMIT's backbone, and China Telecom CN2 GIA."

So Premium isn't a mystery tier — it's the Tier 1 backbone *plus* DMIT's own network *plus* premium transit partners, with China Telecom's CN2 GIA on top. DMIT lists the recommended workloads as corporate and e-commerce sites targeting China and APAC visitors, live streaming and media delivery, low-latency game servers for Asian players, and cross-border applications that need stable routing into mainland China.

If your users aren't in mainland China or Asia-Pacific, that list is a polite way of telling you to buy something cheaper.

## Premium vs Eyeball vs Tier 1

Before you look at prices, get the three profiles straight. They differ entirely in routing, not in CPU or RAM — the same plan size exists in each.

| Profile | Routing | Roughly who it's for |
| --- | --- | --- |
| **Tier 1** (`.T1`) | Clean international transit, no China-specific optimisation | Overseas audiences, bandwidth-heavy work, cheap annual entry |
| **Eyeball** (`.EB`) | China Mobile CMIN2 plus China-optimised peering | Mobile-first China audiences, more traffic per dollar than Premium |
| **Premium** (`.Pro`) | Tier 1 + DMIT backbone + premium transit + China Telecom CN2 GIA | Sites and services where mainland China latency is the product |

The practical rule: Premium costs more per gigabyte of traffic than Eyeball, and both cost more than Tier 1. What you buy with the difference is routing that doesn't fall apart during Chinese peak hours. DMIT's Cloud Instance page frames it as "lower latency, fewer hops, and significantly reduced packet loss" versus a typical Tier 1 path — which is marketing, but it's marketing that matches the AS-path data third-party reviewers keep publishing.

## Los Angeles Premium plans and pricing

LAX is where most people start, and it's also where the entry price is lowest. The current-generation AS3 platform uses AMD EPYC 7003 series CPUs.

| Plan | CPU | RAM | SSD | Monthly traffic | Port | After quota | Price | Order |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LAX.AS3.Pro.TINY | 1 core | 2 GB | 20 GB | 1,000 GB | 1 Gbps | 4 Mbps unmetered | $10.90/mo | [ Start with the entry Premium plan](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.Pocket | 2 cores | 2 GB | 40 GB | 1,500 GB | 4 Gbps | 4 Mbps unmetered | $16.90/mo | [ See the Pocket configuration](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.STARTER | 2 cores | 2 GB | 80 GB | 3,000 GB | 10 Gbps | 4 Mbps unmetered | $34.90/mo | [ Check STARTER availability](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.MINI | 4 cores | 4 GB | 80 GB | 5,000 GB | 10 Gbps | 8 Mbps unmetered | $62.90/mo | [ Compare the MINI plan](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.MICRO | 4 cores | 4 GB | 160 GB | 7,000 GB | 10 Gbps | 8 Mbps unmetered | $87.90/mo | [ View MICRO specs and stock](https://www.dmit.io/aff.php?aff=12046) |
| LAX.AS3.Pro.MEDIUM | 6 cores | 8 GB | 160 GB | 14,000 GB | 10 Gbps | 10 Mbps unmetered | $199.90/mo | [ Check the MEDIUM plan](https://www.dmit.io/aff.php?aff=12046) |

Two things stand out. First, the jump from TINY to Pocket buys 2 cores, double the disk, 500 GB more traffic, and a 4 Gbps port for $6. Second, RAM flatlines at 2 GB all the way to STARTER, which is $34.90 for the same memory as the $10.90 plan. If memory is your constraint, STARTER is a bad deal and MINI is where things actually change.

The AS3 platform also carries a warning DMIT publishes itself: it's still described as being in a continuous optimisation stage, with disk performance and SLA potentially below a mature platform. Don't put a revenue-critical site on an unproven generation if you can wait.

## Hong Kong Premium: two hardware generations, two price lists

Hong Kong is the latency play. The physical distance from Hong Kong to mainland China is why Premium routing here gets you the lowest round-trip times in DMIT's catalog, and also why the prices start roughly four times higher than LAX.

**HKG Premium on AS3 (AMD EPYC 7003):**

| Plan | CPU | RAM | SSD | Monthly traffic | Price | Order |
| --- | --- | --- | --- | --- | --- | --- |
| TINY | 1 core | 1 GB | 20 GB | 500 GB | $39.90/mo | [ See Hong Kong Premium TINY](https://www.dmit.io/aff.php?aff=12046) |
| STARTER | 1 core | 2 GB | 40 GB | 1,000 GB | $79.90/mo | [ Compare HKG STARTER](https://www.dmit.io/aff.php?aff=12046) |
| MINI | 2 cores | 2 GB | 60 GB | 1,500 GB | $126.90/mo | [ Check HKG MINI stock](https://www.dmit.io/aff.php?aff=12046) |
| MICRO | 2 cores | 4 GB | 80 GB | 2,000 GB | $179.90/mo | [ View the MICRO plan](https://www.dmit.io/aff.php?aff=12046) |
| MEDIUM | 4 cores | 4 GB | 160 GB | 2,500 GB | $239.90/mo | [ See the MEDIUM configuration](https://www.dmit.io/aff.php?aff=12046) |

**HKG Premium on AN5 (AMD EPYC 9005):** the same Premium routing on newer silicon, with larger disks:

| Plan | CPU | RAM | SSD | Monthly traffic | Price | Order |
| --- | --- | --- | --- | --- | --- | --- |
| MINI | 2 cores | 2 GB | 80 GB | 1,500 GB | $149.90/mo | [ See AN5 MINI pricing](https://www.dmit.io/aff.php?aff=12046) |
| MICRO | 2 cores | 4 GB | 160 GB | 2,000 GB | $159.90/mo | [ Compare AN5 MICRO](https://www.dmit.io/aff.php?aff=12046) |
| MEDIUM | 4 cores | 4 GB | 160 GB | 2,500 GB | $180.00/mo | [ Check AN5 MEDIUM](https://www.dmit.io/aff.php?aff=12046) |
| LARGE | 4 cores | 8 GB | 320 GB | 3,000 GB | $240.00/mo | [ View AN5 LARGE](https://www.dmit.io/aff.php?aff=12046) |
| GIANT | 8 cores | 16 GB | 640 GB | 6,000 GB | $500.00/mo | [ See AN5 GIANT specs](https://www.dmit.io/aff.php?aff=12046) |

Read that pair of tables carefully, because there's a real arbitrage in it. The AN5 MICRO at $159.90 gives you 160 GB of disk and 4 GB of RAM, while the AS3 MICRO at $179.90 gives you 80 GB and the same 4 GB. If you need storage and don't need the newest CPU, the older-generation AS3 line isn't automatically the cheaper one — the AN5 lineup starts at MINI and skips the small tiers entirely.

Hong Kong stock moves in bursts and frequently sells out. Anything you read about availability, including here, has a shelf life of days.

## Tokyo Premium plans

Tokyo sits between the two on latency — worse than Hong Kong, noticeably better than Los Angeles for mainland users. Premium pricing starts lower than Hong Kong but the traffic allowances are smaller.

| Plan | CPU | RAM | SSD | Monthly traffic | Price | Order |
| --- | --- | --- | --- | --- | --- | --- |
| TYO.Pro.TINY | 1 core | 1 GB | 20 GB | 300 GB | $21.90/mo | [ See Tokyo Premium TINY](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.STARTER | 1 core | 2 GB | 30 GB | 500 GB | $32.90/mo | [ Compare TYO STARTER](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MINI | 2 cores | 2 GB | 50 GB | 1,000 GB | $54.90/mo | [ Check TYO MINI availability](https://www.dmit.io/aff.php?aff=12046) |
| TYO.Pro.MICRO | 2 cores | 4 GB | 80 GB | 2,000 GB | $74.90/mo | [ View TYO MICRO](https://www.dmit.io/aff.php?aff=12046) |

Larger Tokyo Premium tiers exist above MICRO and are priced well into the hundreds per month. Tokyo is DMIT's most frequently sold-out region, so treat the table as a target list rather than a menu.

## Premium Secure and Premium Unmetered

Two Premium variants on the Los Angeles side sit outside the standard table, and they solve specific problems rather than offering better value.

**Premium Secure** (`.sPro`) takes the CN2 GIA return path and puts Cloudflare Magic Transit in front of the inbound direction. Inbound traffic gets scrubbed at Cloudflare's edge; outbound traffic still returns over GIA. That asymmetry is deliberate, since most attacks hit inbound connections. If you're running the kind of site that attracts DDoS traffic, this is the version of Premium you want rather than bolting on third-party protection.

**Premium Unmetered** trades bandwidth for a traffic cap that doesn't exist. Instead of metered gigabytes with a throttle at the limit, you get a fixed unmetered port speed. The catch is the port is slower than what metered Premium plans offer. It makes sense for steady, predictable throughput; it's a bad fit if you occasionally need to move hundreds of gigabytes in an afternoon.

Both are LAX-only offerings as far as DMIT's current product listing goes.

## AS3 vs AN4 vs AN5: paying for hardware you probably don't need

DMIT runs Premium across multiple hardware generations on the same routes. The naming follows the platform: AS3 is AMD EPYC 7003, AN4 is EPYC 9004, AN5 is EPYC 9005.

Same plan, same route, different generation means different prices. The `LAX.Pro.TINY` tier, for instance, has been listed around $10.90/month on AS3, roughly $12.90 on AN4, and again higher on AN5 — a spread of a few dollars a month for identical network behaviour and identical specs.

For a VPN endpoint, a small website, or a proxy, that spread buys you nothing you'll notice. CPU generation matters when you're running something that actually consumes CPU — databases, encryption-heavy services, build agents, game servers. If your workload is network-bound rather than compute-bound, buy the oldest generation that's in stock and put the difference into more traffic.

## The throttle is the real pricing mechanism

Here's the part worth understanding before you compare DMIT to anyone else: Premium plans don't shut off when you exhaust your monthly traffic. They drop to a low unmetered speed — 4 Mbps on the small LAX tiers, 8 Mbps on MINI and MICRO, 10 Mbps on MEDIUM.

4 Mbps is roughly enough for one 1080p stream. It is not enough for a busy website. But it is enough to keep a light SSH-accessed box alive, and it means a traffic spike won't hard-kill your service at 3 a.m.

That matters when you're sizing a plan. Paying for 3,000 GB you'll never touch is worse value than buying 1,000 GB and accepting throttle in the last week of the month — unless a week at 4 Mbps would visibly break your product.

Some Tokyo Premium listings, by contrast, describe the service pausing until the next billing cycle rather than throttling. Sources disagree on this and DMIT revises plan terms between restocks, so read the specific product page before you commit.

## Discounts: recurring codes, not sales

DMIT doesn't run broad seasonal sales the way budget hosts do. What it issues are recurring discount codes scoped to a product line and a billing cycle, so the discount applies to every renewal, not just the first invoice.

The naming convention gives away what each code does. `202510_HKG_TYO_PRO_20OFF_RECURRING` is a 20% recurring discount on Hong Kong and Tokyo Premium on quarterly-or-longer terms. Codes circulating for the LAX Pro and Eyeball lines have included 10% and 15% recurring variants, typically restricted to STARTER-and-up or to non-monthly billing.

Two honest caveats. Codes are rebuilt each promo cycle, so anything you find in a blog post or aggregator — including the strings above — may already be dead; the cart has a validation step and will simply refuse it. And the recurring structure means the discount is worth far more on an annual plan than a monthly one, which is exactly the trade DMIT is nudging you toward.

Billing cycles themselves carry a discount: annual and semi-annual terms are priced below twelve and six monthly payments respectively. Combine that with a valid recurring code and the effective monthly cost of Premium comes down meaningfully. Verify the final number in the cart rather than trusting arithmetic done from a third-party table.

## Refunds, IP swaps, and other fine print

A few policies matter enough to check before paying, particularly if you're buying an annual Premium plan at Hong Kong prices.

The refund window is short and conditional. As documented, you get a full refund within three days of purchase as long as you've used no more than 30 GB of traffic — minus the payment gateway fee. After that, partial refunds are calculated on remaining service time within a 30-day window. Renewal orders, balance-funded purchases, repeat refunds on the same product line, and IPs blocked by the GFW are excluded. Policies like these get revised, so confirm against DMIT's current terms.

IP replacement costs $5 in normal circumstances. If the IP is blocked, replacement is free, but limited to once every 15 days. Given that a blocked IP is the single most common reason people abandon a China-facing VPS, that distinction is worth knowing before you file a ticket.

Payment methods include PayPal, Alipay, and major credit cards. Support is handled over tickets.

## Who should skip Premium

Three cases where Premium is the wrong purchase:

**Your audience is entirely outside China and APAC.** The entire value of the `.Pro` profile is the CN2 GIA path and the China peering. Remove that requirement and you're paying a large premium for routing that delivers nothing your users can perceive. Tier 1 exists for exactly this.

**You're bandwidth-hungry but latency-tolerant.** Bulk file serving, backup targets, media archives — Eyeball gives you far more traffic per dollar with routing that's still China-optimised, just weighted toward China Mobile rather than China Telecom.

**You need a written SLA.** DMIT doesn't publish one, and third-party write-ups flag that host-node maintenance happens without advance email notice. If your business depends on contractual uptime guarantees, this isn't the vendor for it.

Where Premium does earn its price: websites and applications whose users are in mainland China, latency-sensitive services like real-time communication or game servers, cross-border apps that need consistent routing rather than peak-hour collapse, and anyone running the kind of target that needs the Secure variant. Those are the scenarios DMIT built the profile for, and the price reflects the transit contracts behind it.

Start with the smallest tier that covers your traffic, run a month, and check the routing yourself before committing to an annual term. DMIT publishes a looking glass for each location if you want to trace the path from your own connection first.

👉 [Browse current DMIT Premium plans and pricing](https://www.dmit.io/aff.php?aff=12046)
