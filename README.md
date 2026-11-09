# Awesome-Automated-Threat-Anomaly-Detection

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **pricing is fragmented across marketplace listings**, and the open-source side is a commercial product's free core.

## The data problems

**Druva's threat detection is a managed service (MDDR), not a standalone product.** The PDF describes AI-driven threat detection, automated recovery, and a $10M Data Resiliency Guarantee, with **Managed Data Detection & Response (MDDR)** provided by Druva's SOC 24/7 . **Threat Hunting is a Premium SKU** . No specific price for threat detection surfaced—Druva uses consumption-based pricing with no egress fees .

**CrowdStrike publishes per-device pricing.** Falcon Go **$7.99/device/month**, Falcon Pro **$14.99/device/month**, Falcon Enterprise **$19.99/device/month** or **$184.99/device/year** .

**SentinelOne publishes per-endpoint pricing.** Singularity Complete **$179.99/endpoint/year**, Commercial **$229.99/endpoint/year**, Enterprise contact sales . Prices are for 5–100 workstations and final pricing goes through an authorized partner .

**Microsoft Defender for Endpoint Plan 2 is $32.91/user** per CDW listing . The E5 Security add-on lists at **$12/user/month** on an E3 base, with median negotiated rates **$8–$10** .

**Trend Micro Vision One Endpoint Security Essentials renewal is $39.89–$42.65/device** for 251–500 licenses .

**Sophos Intercept X has no published price**—Software Advice reviews describe it as higher cost than competitors .

**Carbon Black Cloud entry-level starts around $5/endpoint/month** per SelectHub .

**Palo Alto Cortex XDR ProEP is $747.11 for 1 endpoint for 1 month** per CDW . That is an extreme outlier—likely a renewal or specialized SKU—and should not be presented as a standard rate.

**FortiEDR is $27,813.28 for 500 endpoints for 1 year** per CDW . That works out to **~$55.63/endpoint/year**.

**Check Point Harmony Endpoint Complete renewal is $131,482.46 for 1 license** per CDW . That figure is almost certainly a multi-year or multi-seat bundle mislabeled as 1 license—do not present it as a per-endpoint rate.

## Open-source: what actually exists

**Kizashi** is the only open-source EDR surfaced: **AGPL-3.0, self-hostable, Windows endpoints only** . It captures ETW telemetry for process, network, registry, DNS, auth, WMI, named pipes, and PowerShell. It supports network isolation and rule-driven auto-remediation.

**Kizashi is the free core of a commercial product.** Curated rule packs, stateful behavioral detectors (port-scan, DNS tunneling, C2 correlation, ransomware burst, kill-chain scoring), YARA scanning, and SigmaHQ sync are **commercial edition only** . Linux/macOS agents, threat intel feeds, UEBA, and AI-assisted triage are also commercial .

**Do not present Kizashi as a full EDR replacement**—it is a telemetry and isolation core without the detection content that makes EDR useful.

## What I recommend

**Split into two honest categories:**

**1. Commercial EDR Platforms** (proprietary):
- **CrowdStrike** — $7.99–$19.99/device/mo 
- **SentinelOne** — $179.99–$229.99/endpoint/yr 
- **Microsoft Defender** — $32.91/user (CDW) ; E5 add-on $12/user/mo 
- **Trend Micro** — ~$40/device renewal 
- **FortiEDR** — ~$55.63/endpoint/yr 
- **Carbon Black** — from ~$5/endpoint/mo 
- **Druva** — MDDR managed service, Premium SKU 
- **Sophos, Palo Alto, Check Point** — pricing fragmented or outliers 

**2. Open-Source (free core only):**
- **Kizashi** — AGPL-3.0, Windows ETW telemetry + isolation, detection content is commercial 

**Flag the pricing outliers explicitly:** Cortex XDR's $747.11/month for 1 endpoint  and Check Point's $131,482.46 for "1 license"  are not standard per-endpoint rates. Do not present them as comparable to CrowdStrike's $19.99/device/month.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not present Druva MDDR as a standalone SKU, cite Cortex XDR's outlier as a standard rate, or claim Kizashi replaces commercial EDR detection.
