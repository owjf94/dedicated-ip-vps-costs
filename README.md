# buy vps with dedicated ip: Real Costs, What's Included by Default, and When Residential IP Actually Matters

Most VPS providers advertise dedicated IP addresses, but the actual bundling varies: some include it free, some charge $2–5/month extra, and the phrase "dedicated IP" itself can mean two completely different things depending on whether you're getting a standard datacenter address or a residential one.

If you're shopping for a VPS specifically because you need a dedicated IP—whether that's for running your own mail server, setting up SSL, accessing geo-restricted services, or avoiding the reputation issues that come with shared addresses—the actual decision comes down to three questions: Does the plan include it at no extra cost? Is it the type of IP you actually need? And what's the real monthly spend once you factor in bandwidth, renewal pricing, and whether you'll need to scale up later?

> **Quick decision guide:**
> - **Standard hosting, email, SSL, or server management** → ZoroCloud US-9929-Plus at ¥49/month includes dedicated IPv4, 1TB bandwidth, 24-hour refund protection; or RackNerd 1GB Special at $21.99/year for lowest annual cost
> - **Account management, streaming unlock, platform verification** → ZoroCloud Hong Kong residential at ¥88/month (~$12) provides genuine ISP-grade static residential IPv4
>
> 👉 [View ZoroCloud's datacenter and residential VPS plans](https://bit.ly/zorocloud)

## What "Dedicated IP" Actually Includes (and What It Doesn't)

A dedicated IP means you get a unique IPv4 address assigned only to your VPS—not shared with other users, not behind NAT. You control the rDNS record, you can bind services directly to it, and outgoing connections show your IP instead of a shared pool address.

The variation across providers:

- **Number included:** Most budget VPS plans include exactly one IPv4. If you need more, expect $2–5/month per additional address, and some providers cap how many you can add.
- **Type of IP:** Standard VPS comes with datacenter IPs. These work fine for hosting, APIs, and most server tasks, but platforms that care about IP reputation (streaming services, social networks, payment gateways) often flag or throttle datacenter ranges. Residential IPs cost more but appear as regular home internet connections.
- **IPv6 availability:** Many providers hand out IPv6 addresses freely—RackNerd gives up to 100 free IPv6 in some locations. If your application supports IPv6, you can save the IPv4 for legacy services.

ZoroCloud's entire VPS lineup includes one dedicated IPv4 by default across all tiers, from the ¥39/month US-9929-Mini to the ¥669/month Elite plans. That's standard for most serious providers now—RackNerd does the same, and even their cheapest $21.99/year plan ships with a dedicated address and full rDNS control.

The real question isn't whether you get an IP; it's whether the IP you get will work for your actual use case.

## Datacenter IP vs. Residential IP: When the Difference Actually Matters

Not all dedicated IPs behave the same way once you start using them.

**Datacenter IPs** come from IP blocks registered to hosting companies. They're what you get with standard VPS plans. Use them for:

- Web hosting and application servers
- API endpoints and backend services
- Email servers (though you'll need to work on sender reputation)
- Development and testing environments
- VPN endpoints for basic privacy

They're cheap, plentiful, and totally fine for most server workloads.

**Residential IPs** are registered to actual ISPs—the same pools that home internet connections come from. They cost significantly more but solve specific problems:

- Running accounts on platforms with aggressive datacenter blocking (TikTok, Instagram business accounts, ad verification tools)
- Bypassing geo-restrictions that specifically filter datacenter ranges
- Web scraping without instant rate limiting
- Streaming service access where datacenter IPs get blocked
- AI service access (ChatGPT, Claude, Gemini) in regions with restrictive policies

ZoroCloud splits their lineup accordingly. Their US-9929, US-CNC, and US-CERA series use standard datacenter IPs optimized for China-to-US connectivity (CN2 GIA, AS9929 routing). Their separate residential dual-ISP plans in Hong Kong, Japan, and Singapore provide genuine ISP-grade static residential addresses that stay assigned to your VPS for the service duration.

If you're just hosting a website or running a backend service, paying 3–4x more for a residential IP makes no sense. But if you've been burned by platforms detecting and blocking your datacenter VPS within hours, the residential option isn't a luxury—it's the baseline that actually works.

## ZoroCloud Datacenter VPS Plans (Standard Dedicated IPv4)

All plans include 1 dedicated IPv4, KVM virtualization, and 24-hour refund policy. Refund conditions: traffic used < 20GB, no IP abuse/blocking, no malicious activity. Limit: 2 refund requests per user account per day.

### US-9929 Series (AS9929 routing, both directions)

Test IP: 38.34.13.1

| Plan | CPU | RAM | Storage | Bandwidth | Monthly Traffic | Price | Order |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Mini | 1×E5v4 | 1GB | 20GB SSD | 100Mbps | 500GB | ¥39/month | [Order US-9929-Mini](https://bit.ly/zorocloud) |
| Plus | 1×E5v4 | 1GB | 20GB SSD | 100Mbps | 1TB | ¥49/month | [Order US-9929-Plus](https://bit.ly/zorocloud) |
| Pro | 2×E5v4 | 2GB | 40GB SSD | 100Mbps | 2TB | ¥79/month | [Order US-9929-Pro](https://bit.ly/zorocloud) |
| Max | 4×E5v4 | 4GB | 80GB SSD | 100Mbps | 4TB | ¥169/month | [Order US-9929-Max](https://bit.ly/zorocloud) |
| Ultra | 4×E5v4 | 8GB | 120GB SSD | 200Mbps | 6TB | ¥358/month | [Order US-9929-Ultra](https://bit.ly/zorocloud) |
| Elite | 8×E5v4 | 16GB | 160GB SSD | 200Mbps | 12TB | ¥638/month | [Order US-9929-Elite](https://bit.ly/zorocloud) |

### US-CNC Series (CN2/9929/CMIN2 optimized routing)

| Plan | CPU | RAM | Storage | Bandwidth | Monthly Traffic | Price | Order |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Plus | 1×EPYC | 1GB | 20GB NVMe | 100Mbps | 1TB | ¥59/month | [Order US-CNC-Plus](https://bit.ly/zorocloud) |
| Pro | 2×EPYC | 4GB | 40GB NVMe | 100Mbps | 2TB | ¥99/month | [Order US-CNC-Pro](https://bit.ly/zorocloud) |
| Max | 4×EPYC | 4GB | 80GB NVMe | 100Mbps | 3TB | ¥189/month | [Order US-CNC-Max](https://bit.ly/zorocloud) |
| Ultra | 4×E5v4 | 8GB | 120GB NVMe | 100Mbps | 4TB | ¥368/month | [Order US-CNC-Ultra](https://bit.ly/zorocloud) |
| Elite | 8×EPYC | 16GB | 160GB NVMe | 100Mbps | 6TB | ¥669/month | [Order US-CNC-Elite](https://bit.ly/zorocloud) |

### US-CERA Series (Cera DDoS protection + CN2 GIA return path)

| Plan | CPU | RAM | Storage | Bandwidth | Monthly Traffic | DDoS Protection | Price | Order |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Plus | 1×EPYC | 1GB | 20GB NVMe | 100Mbps | 1TB | 50Gbps | ¥59/month | [Order US-CERA-Plus](https://bit.ly/zorocloud) |
| Pro | 2×EPYC | 4GB | 40GB NVMe | 100Mbps | 2TB | 50Gbps | ¥104/month | [Order US-CERA-Pro](https://bit.ly/zorocloud) |
| Max | 4×EPYC | 4GB | 80GB NVMe | 100Mbps | 3TB | 50Gbps | ¥194/month | [Order US-CERA-Max](https://bit.ly/zorocloud) |
| Ultra | 4×E5v4 | 8GB | 120GB NVMe | 100Mbps | 4TB | 50Gbps | ¥373/month | [Order US-CERA-Ultra](https://bit.ly/zorocloud) |
| Elite | 8×E5v4 | 16GB | 160GB NVMe | 200Mbps | 6TB | 50Gbps | ¥673/month | [Order US-CERA-Elite](https://bit.ly/zorocloud) |

### Other Regional Series (Europe & UK)

ZoroCloud also operates UK-9929 (starting ¥129/month, test IP 85.189.123.1) and DE-9929 (starting ¥129/month, test IP 189.24.110.1) series with similar AS9929 routing for European users. Full specifications available on the official store.

The three US series target slightly different priorities. US-9929 focuses on raw connectivity quality for users routing through China Unicom's AS9929 network. US-CNC adds multi-carrier optimization across China Telecom, Unicom, and Mobile. US-CERA trades a bit of routing optimization for built-in 50Gbps DDoS protection—useful if you're running public-facing services that occasionally attract attack traffic.

For basic VPS hosting with a dedicated IP where you just need the server to be reachable and reasonably fast, the ¥49/month US-9929-Plus gives you 1TB monthly transfer and a 24-hour refund window to test whether the routing works for your location. 👉 [Check US-9929 series pricing](https://bit.ly/zorocloud)

## ZoroCloud Residential IP Plans (Static ISP-Grade Addresses)

These plans use genuine residential ISP connections, not datacenter IP blocks rebranded as "residential." The IP stays static and dedicated to your VPS; it doesn't rotate or pull from a shared pool. Third-party sources estimate pricing in USD equivalents, but official billing uses CNY.

| Location | CPU | RAM | Storage | Bandwidth | Monthly Traffic | Test IP | Estimated Price |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Hong Kong | 1 core | 1GB | 20GB | 100Mbps | 1TB | 61.10.4.1 | ¥88/month (~$12) |
| Hong Kong | 2 cores | 4GB | 40GB | 100Mbps | 2TB | 61.10.4.1 | ¥115/month (~$16) |
| Hong Kong | 4 cores | 4GB | 80GB | 100Mbps | 4TB | 61.10.4.1 | ¥230/month (~$32) |
| Japan | 1 core | 1GB | 10GB | 200Mbps | 1TB | — | ¥100/month (~$14) |
| Japan | 2 cores | 2GB | 20GB | 300Mbps | 2TB | — | ¥155/month (~$22) |
| Japan | 4 cores | 4GB | 40GB | 500Mbps | 4TB | — | ¥300/month (~$42) |
| Singapore | 1 core | 1GB | 20GB | 200Mbps | 1TB | 203.116.0.1 | ¥185/month (~$26) |
| Singapore | 2 cores | 2GB | 40GB | 300Mbps | 2TB | 203.116.0.1 | ¥280/month (~$39) |
| Singapore | 4 cores | 4GB | 80GB | 500Mbps | 4TB | 203.116.0.1 | ¥570/month (~$80) |

*USD estimates based on third-party reporting at approximate 7.0 CNY/USD exchange rate; verify current pricing on official site.*

These work well for account operations, streaming unlock, AI service access, and any scenario where platforms actively filter datacenter IPs. The Hong Kong plans offer the lowest entry cost for residential IP in Asia; Japan provides higher bandwidth at similar pricing; Singapore costs more but gives dual-ISP routing with higher IP purity for stricter platform verification.

Annual payment discount available with promo code **Zoroyear** (applies to yearly billing cycles only).

## How RackNerd's Pricing Compares (Datacenter IP Only)

RackNerd runs on similar economics—every plan includes one dedicated IPv4 by default—but structures pricing differently.

**Annual Specials** (best per-month cost):

- 1GB RAM / 1 core / 20GB SSD / 3TB bandwidth: **$21.99/year** (~$1.83/month)
- 2GB RAM / 2 cores / 35GB SSD / 5TB bandwidth: **$35.99/year** (~$3/month)
- 4GB RAM / 3 cores / 60GB SSD / 7TB bandwidth: **$59.99/year** (~$5/month)
- 6GB RAM / 6 cores / 100GB SSD / 12TB bandwidth: **$89.99/year** (~$7.50/month)
- 8GB RAM / 7 cores / 150GB SSD / 20TB bandwidth: **$119.99/year** (~$10/month)

**Monthly Standard Plans**:

- 512MB RAM / 1 vCore / 30GB SSD / 500GB bandwidth: **$26.99/year**
- 1GB RAM / 2 vCores / 50GB SSD / 1TB bandwidth: **$17.99/month**
- 4GB RAM / 4 vCores / 130GB SSD / 3TB bandwidth: **$24.59/month**
- 8GB RAM / 6 vCores / 220GB SSD / 5TB bandwidth: **$36.59/month**

The annual pricing beats almost everything else at the entry level. The catch: you pay upfront, and if you outgrow the plan mid-contract, upgrading cleanly usually means opening a new order rather than seamlessly moving to the next tier.

RackNerd doesn't offer residential IP options. Their entire lineup focuses on datacenter-grade infrastructure with strong annual pricing but no ISP-grade residential addressing.

## Real Total Cost: What You Actually Pay Over 12 Months

Monthly advertised pricing hides the real cost comparison. Looking at 12-month totals:

**Entry-level dedicated IP hosting:**

- RackNerd 1GB Special: $21.99 total (prepaid annual)
- ZoroCloud US-9929-Mini: ¥39 × 12 = ¥468 (~$67/year at 7.0 rate)
- ZoroCloud US-9929-Plus: ¥49 × 12 = ¥588 (~$84/year at 7.0 rate)

RackNerd wins on absolute cost, but the ¥10/month difference between ZoroCloud Mini and Plus matters: you're paying ¥120/year extra to double your bandwidth from 500GB to 1TB. If you routinely hit 500GB/month, that's worth it. If you stay under 300GB, the Mini saves you money without losing functionality.

**Mid-tier with better specs:**

- RackNerd 4GB Special: $59.99/year (3 cores, 60GB SSD, 7TB bandwidth)
- ZoroCloud US-9929-Max: ¥169 × 12 = ¥2,028 (~$290/year, 4 cores, 80GB SSD, 4TB bandwidth)

At this tier, RackNerd's annual special costs less than 5 months of ZoroCloud's equivalent. You'd choose ZoroCloud Max only if AS9929 routing demonstrably improves your user experience enough to justify the 5x cost difference—which it might if your traffic is primarily China-based and latency-sensitive.

**Residential IP (no RackNerd equivalent):**

- ZoroCloud Hong Kong residential: ¥88 × 12 = ¥1,056 (~$151/year)
- ZoroCloud Japan residential: ¥100 × 12 = ¥1,200 (~$171/year)

These have no direct comparison because the IP type is fundamentally different. If platforms block datacenter IPs for your use case, the question isn't whether residential IP costs more—it's whether you can operate at all without it.

## Three Scenarios and What You'd Actually Pay

**Scenario 1: Basic web hosting + email with dedicated IP**

You need a clean dedicated IP for SSL and to avoid shared-IP email reputation issues. Traffic is light; you're just running a WordPress site and a small mail server.

- **RackNerd 1GB Special** at $21.99/year works if you're comfortable with annual prepay and minimal RAM. Includes dedicated IPv4, 20GB storage, 3TB bandwidth.
- **ZoroCloud US-9929-Plus** at ¥49/month costs ¥588/year (~$84) but gives monthly flexibility and CN2-optimized routing if your users are in Asia. Also includes 1TB bandwidth and 24-hour refund window.

Both include the dedicated IP; neither charges extra for it. The question is whether you value lower total cost (RackNerd) or flexible billing + better Asia routing (ZoroCloud).

**Scenario 2: Running social media accounts or scraping without getting instantly blocked**

Standard datacenter IPs get flagged within hours. You need a residential IP that platforms treat as a real user connection.

- **ZoroCloud Hong Kong residential** at ¥88/month is the cheapest residential option. 1GB RAM, 100Mbps, 1TB monthly transfer, static residential IPv4.
- **ZoroCloud Japan residential** at ¥100/month provides better bandwidth (200Mbps) and slightly more storage for ¥12 extra per month.

There's no datacenter-IP equivalent that solves this problem. You either pay for residential or deal with constant blocks and CAPTCHA loops.

**Scenario 3: Mid-sized app or API service with moderate traffic**

You need more than 1GB RAM, predictable performance, and enough bandwidth to handle a few hundred concurrent users without throttling.

- **RackNerd 4GB Special** at $59.99/year gives 3 vCores, 60GB SSD, 7TB bandwidth. Dedicated IPv4 included. Strong value if you don't need residential.
- **ZoroCloud US-9929-Max** at ¥169/month costs ¥2,028/year but provides 4 vCores, 4GB RAM, 4TB bandwidth, and AS9929 premium routing. Also includes 24-hour refund if the routing doesn't meet expectations.

At this tier, RackNerd wins on raw cost. ZoroCloud makes sense if your user base is primarily in China and routing quality directly affects perceived app performance. 👉 [Compare ZoroCloud datacenter plans](https://bit.ly/zorocloud)

## When You Don't Need a Dedicated IP (and Can Save Money)

NAT VPS plans exist—they give you a VPS with shared IPv4 and a block of forwarded ports (usually 20+ ports in the higher range). Monthly cost drops to $1–3 for similar specs, and IPv6 is usually included directly.

You can use NAT VPS if:

- Your app only needs outbound connections (web scraping, API clients, automation scripts)
- You're okay binding services to non-standard ports
- You don't need to run a mail server or anything that requires port 25/465/587
- SSL works fine with IPv6 or an external reverse proxy

You can't use NAT VPS if:

- You need inbound access on standard ports (80, 443, 22, etc.)
- You're running email, game servers, or anything that requires predictable inbound addressing
- The service you're connecting to blocks IPv6 or shared IP ranges

Most people searching for "buy VPS with dedicated IP" already know they need the dedicated address. But if your use case is flexible, confirming whether you actually need dedicated IP or just need *any* public-facing address can cut your monthly cost in half.

## What to Check Before You Buy

**Bandwidth limits and overage costs:** 1TB sounds like a lot until you're streaming video, running backups, or handling image-heavy traffic. Check whether the provider throttles after the cap or charges overages. ZoroCloud's plans state the monthly transfer cap clearly; RackNerd provides generous bandwidth but doesn't specify throttling vs. billing behavior in standard documentation.

**Refund and testing windows:** ZoroCloud offers 24-hour refunds if usage is under 20GB and there's no IP abuse, with a limit of 2 refund requests per user account per day. RackNerd mentions 72-hour free IPv4 replacement but doesn't prominently advertise a refund policy. If routing quality matters to your workload, having a way to test and exit within the first day removes a lot of risk.

**IP replacement policy:** If your dedicated IP gets blacklisted or shows up on spam databases due to previous user behavior, can you get a new one? RackNerd allows free IPv4 swaps within 72 hours. ZoroCloud's replacement policy wasn't explicitly detailed in available documentation, but the 24-hour refund window at least gives you a clean exit if the IP is already problematic.

**Storage type:** NVMe (ZoroCloud US-CNC/CERA series) boots faster and handles random I/O better than standard SSD (ZoroCloud US-9929 series, RackNerd RAID-10 SSD). For databases and high-traffic apps, this matters. For static sites and light workloads, the difference is mostly academic.

**Location and latency:** A 1-core VPS in the right datacenter will outperform a 4-core VPS in a distant location for user-facing apps. RackNerd operates 20+ global locations; ZoroCloud focuses on US, UK, Germany, Hong Kong, Singapore, and Japan. Test IP addresses are listed for most ZoroCloud plans—ping them from your actual user locations before buying.

## Making the Call

Standard hosting, development, or backend services where datacenter IP works fine: RackNerd's annual specials at $21.99–$119.99/year offer the lowest per-month cost. ZoroCloud's US-9929 series at ¥39–¥638/month provides monthly flexibility and Asia-optimized routing at roughly 3–5x the annual cost.

Residential IP for account management, streaming unlock, or platform verification: ZoroCloud's Hong Kong residential plans at ¥88/month provide genuine ISP-grade static addresses. This is a different product category with no direct RackNerd equivalent. 👉 [View ZoroCloud's full VPS lineup](https://bit.ly/zorocloud)

The one thing you shouldn't do: assume every "dedicated IP included" VPS will work the same way for your workload. A free datacenter IP is standard now, but whether it's the *type* of IP you need—and whether the provider's routing, bandwidth, refund policy, and actual 12-month cost fit your use case—only becomes clear once you look past the headline price.
