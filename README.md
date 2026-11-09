# Awesome-Automated-Threat-Anomaly-Detection

# Awesome-Automated-Threat-Anomaly-Detection

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **Druva's threat detection is a managed service (MDDR) bundled with the platform, not a standalone product**, and **several entries have pricing that requires careful caveats**.

## The data problems

**Druva's threat detection is MDDR, bundled into the platform.** The comparison PDF describes **Managed Data Detection & Response (MDDR)** as included, with "proactive threat hunting that integrates with XDR, SIEM, and Microsoft Sentinel" and "single price, all-in-one solution, no hidden costs" . **No standalone threat detection price surfaced**—Druva uses all-inclusive SaaS pricing with no egress fees .

**CrowdStrike publishes per-device pricing.** Falcon Go **$7.99/device/month**, Falcon Pro **$14.99/device/month**, Falcon Enterprise **$19.99/device/month** or **$184.99/device/year** .

**SentinelOne publishes per-endpoint pricing.** Singularity Complete **$179.99/endpoint/year**, Commercial **$229.99/endpoint/year**, Enterprise quote-only. Prices displayed for **5–100 workstations** and final pricing goes through an authorized partner .

**Microsoft Defender for Endpoint Plan 2 is included in E5 or the E5 Security add-on.** The add-on lists at **$12/user/month** on an E3 base, with median negotiated rates **$8–$10** and top quartile **$6–$8** . **CDW-G lists Plan 2 at $23.93 per user** , which is a different SKU/pricing context—do not present it as the standard rate.

**Trend Micro Vision One has both CDW and Vendr data.** CDW-G lists Endpoint Security Essentials renewal at **$39.89–$42.65/device** for 251–500 licenses . Vendr benchmarks show mid-market (500–2,000 endpoints) at **$50K–$175K/year**, per-endpoint **$25–$45**; enterprise (2,500–10,000+) at **$200K–$1M+**, per-endpoint **$18–$35** .

**Sophos Intercept X has no published price.** Software Advice reviews describe it as higher cost than competitors .

**Carbon Black Cloud has VendorBenchmark estimates.** Endpoint Standard **$30–$45/endpoint/year**, Advanced **$45–$58**, Enterprise EDR **$58–$72**; post-Broadcom discounts compressed to **15–30%** .

**Palo Alto Cortex XDR Pro is $688.26 for 1 endpoint** per CDW-G . That is an extreme outlier—likely a multi-year or specialized SKU—and should not be presented as a standard rate.

**FortiEndpoint EDR Essentials is $491.99–$549.62 for 1 endpoint for 3 years** per CDW.ca . That works out to **~$164–$183/endpoint/year**.

**Check Point Harmony Endpoint pricing is published per license.** Prevent **$20.99/year**, Advanced **$43.99/year**, Complete **$66.99/year** (1-year) or **$183.99** (5-year) .

## Open-source: what actually exists

The Springer chapter describes an integrated open-source endpoint security framework combining **OSquery, OpenEDR, Bluespawn, Whids** (EDR tools), **Open XDR**, and **TheHive, Cortex, Google GRR** (incident response). In controlled tests simulating **100 targeted attacks on 50 assets**, it achieved **91.4% detection rate**, **14.2s mean time to detect**, **26.7s mean time to respond**, and **under 8% CPU / 10% memory** usage .

**OSquery delivered the best detection efficiency; Open XDR enhanced cross-platform visibility; TheHive streamlined incident workflows** . This is a research-validated open-source stack, not a single product.

**No star counts were surfaced** for OSquery, OpenEDR, Bluespawn, Whids, Open XDR, TheHive, Cortex, or GRR. Do not invent them.

## What I recommend

**Split into two honest categories:**

**1. Commercial EDR / Threat Detection Platforms** (proprietary):
- **CrowdStrike** — $7.99–$19.99/device/mo 
- **SentinelOne** — $179.99–$229.99/endpoint/yr 
- **Microsoft Defender** — E5 add-on $12/user/mo list, $8–$10 negotiated 
- **Trend Micro** — ~$40/device renewal (CDW) ; Vendr $18–$45/endpoint 
- **Carbon Black** — $30–$72/endpoint/yr (VendorBenchmark) 
- **FortiEDR** — ~$164–$183/endpoint/yr (3-year, CDW) 
- **Check Point Harmony** — $20.99–$66.99/year per license 
- **Sophos Intercept X** — pricing not surfaced 
- **Druva** — MDDR bundled, all-inclusive platform pricing 

**2. Open-Source EDR Stack** (research-validated combination):
- **OSquery** — best detection efficiency in the study 
- **OpenEDR, Bluespawn, Whids** — EDR components 
- **Open XDR** — cross-platform visibility 
- **TheHive, Cortex, GRR** — incident response 

**Flag the pricing outliers explicitly:** Cortex XDR's $688.26 for 1 endpoint  and Microsoft's CDW listing at $23.93/user  are not standard per-endpoint rates comparable to CrowdStrike's $19.99/device/month.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not present Druva MDDR as a standalone SKU, cite Cortex XDR's outlier as a standard rate, or fabricate star counts for the open-source stack.
