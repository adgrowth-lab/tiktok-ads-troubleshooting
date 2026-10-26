# TikTok Ads Troubleshooting & Optimization Guide (2026 Edition): Fix TikTok Ads Not Spending, Audit Pangle Bot Traffic & Claim $6,000 TikTok Ad Credit 🛡️

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)](audit.py)
[![Test Suite: 100% Passed](https://img.shields.io/badge/Tests-31%2F31_Passing-brightgreen?style=for-the-badge)](test_audit.py)
[![TikTok Ads Credit: Up to $6,000 Match](https://img.shields.io/badge/TikTok_Ads_Credit-Up_To_$6,000_Match-25f4ee?style=for-the-badge&logo=tiktok&logoColor=black)](https://adgrowth-lab.github.io/)
[![Official Partner Gateway](https://img.shields.io/badge/Official_Route-Direct_TikTok_Partner-fe2c55?style=for-the-badge&logo=tiktok&logoColor=white)](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng)
[![Reddit 30-Day Research](https://img.shields.io/badge/Data-64_Reddit_Cases-orange?style=for-the-badge&logo=reddit&logoColor=white)](research-tiktok-ads-reddit-30days.md)

> **The empirical, battle-tested TikTok Ads troubleshooting handbook and diagnostic CLI suite for DTC brands, e-commerce stores, Shopify dropshippers, and media buyers.**  
> Solve **TikTok ads not spending**, audit **Pangle bot traffic leaks**, navigate the **TikTok ads learning phase**, and claim up to **$6,000 in official TikTok ads credit**. Derived from a 30-day investigation of **64 live advertiser cases** across `r/TikTokAds`, `r/PPC`, `r/dropship`, and `r/shopify`.

> 🎁 **OFFICIAL TIKTOK ADS CREDIT & PARTNER INCENTIVE GATEWAY (CLAIM UP TO $6,000 MATCH)**:  
> High-velocity media buyers can bypass personal ad account probation sandboxes ($50/day spend caps) and claim **up to $6,000 in official matching TikTok ad credits** plus a stackable 50% discount voucher directly through the verified partner gateway:  
> 👉 **[Direct TikTok Ads Manager Partner Registration (partnerlinks.io)](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng)**  
> 🧮 **Interactive Modeling Simulator**: **[Launch Web Match Calculator (adgrowth-lab.github.io)](https://adgrowth-lab.github.io/)**  
> *(Official ByteDance enterprise partnership route via Impact.com · Automatic 100%–60% spend matching on new TikTok Ads accounts)*

---

## ⚡ Quick Navigation: The 4 Defense Pillars & Utilities

| Pillar / Module | Primary File / Command | Standalone Repository | Core Function & Scope |
| :--- | :--- | :--- | :--- |
| 🎁 **Official Partner Gateway** | [Claim Up To $6,000 Credits](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng) | [partnerlinks.io Gateway](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng) | **Direct verified registration**: Unlocks spend match vouchers ($200–$6,000) & whitelisted billing |
| 🌐 **All-in-One Defense Suite** | [`COMPREHENSIVE-DEFENSE-SUITE.md`](COMPREHENSIVE-DEFENSE-SUITE.md)<br>`python3 audit.py full-audit` | [tiktok-ads-troubleshooting](https://github.com/adgrowth-lab/tiktok-ads-troubleshooting) | **Integrated master scan**: Evaluates creative, campaign, payment, and traffic in one command |
| 🛡️ **Scheme A: Compliance Linter** | [`CREATIVE-COMPLIANCE-GUIDE.md`](CREATIVE-COMPLIANCE-GUIDE.md)<br>`python3 audit.py compliance` | [tiktok-creative-compliance-linter](https://github.com/adgrowth-lab/tiktok-creative-compliance-linter) | **Pre-flight copy & script auditor**: Catches absolute claims, body shaming, and IP risks |
| 💳 **Scheme B: VCC BIN Database** | [`vcc-bin-database.md`](vcc-bin-database.md)<br>`python3 audit.py bin` | [tiktok-vcc-bin-database](https://github.com/adgrowth-lab/tiktok-vcc-bin-database) | **2026 payment survival table**: 16 verified BINs (Mercury, Stripe, Relay, Airwallex, etc.) |
| 📨 **Scheme C: Appeal Field Kit** | [`appeal-templates/`](appeal-templates/)<br>`python3 audit.py appeal` | [tiktok-ads-appeal-kit](https://github.com/adgrowth-lab/tiktok-ads-appeal-kit) | **5 battle-tested legal templates**: Unusual Activity, Payment Discrepancy, Policy Reversals |
| 🚨 **Pangle Bot Leak Detector** | `python3 audit.py pangle` | Included in Master CLI | **Traffic auditor**: Detects budget drain from 3rd-party gaming apps (Shopify/GA4 CSV support) |
| 🎯 **Cold-Start Campaign Linter** | `python3 audit.py cold-start` | Included in Master CLI | **Algorithmic setup auditor**: Scores your setup (0–100) before spending |
| 💰 **Spend Match Estimator** | `python3 audit.py spend-match` | Included in Master CLI | **Official incentive simulator**: Promotional credits ($200–$6,000) calculator |
| 📊 **30-Day Empirical Dossier** | [`research-tiktok-ads-reddit-30days.md`](research-tiktok-ads-reddit-30days.md) | Included in Master Repo | **Reddit intelligence**: Analysis of 64 live media buyer threads and case studies |
| 🧮 **Interactive Web Simulator** | [adgrowth-lab.github.io](https://adgrowth-lab.github.io/) | [adgrowth-lab.github.io](https://github.com/adgrowth-lab/adgrowth-lab.github.io) | **Clean browser calculator**: Media-buying purchasing power and spend-match estimator |

---

## 📊 1. Executive Summary: The State of TikTok Ads in 2026

Across Reddit ad communities over the past 30 days, one sentiment dominates media buyer discussions: **"Meta CPMs are too expensive to survive, but TikTok is a financial meat grinder if you don't know the landmines."**

Analysis of 64 high-intent discussion threads revealed that **over 80% of advertiser budget waste** stems from six predictable, systemic failure modes:
1. **The Meta-to-TikTok Chasm**: Taking winning Meta static UGC or muted videos to TikTok results in instant sub-0.8s swipe-aways.
2. **Pangle Bot Traffic Hijacking**: Automatic placements quietly routes 80–90% of budget into non-TikTok mobile game rewarded ads.
3. **The External Store Penalty**: TikTok's algorithm heavily favors TikTok Shop GMV Max, while external Shopify checkouts suffer massive bounce rates.
4. **48–72h Creative Burnout**: Winning hooks burn out within 3 days, causing runaway CPAs ($30 CPA ➔ $180+ CPA).
5. **The $50 Spend Limit & VCC Ban Sandboxes**: Personal ad accounts get trapped in probation sandboxes, while whitelisted agency lines scale unhindered.
6. **Predatory Official Rep Advice**: TikTok phone reps consistently advise widening targeting and raising budgets, burning client cash without accountability.

---

## 🔍 2. The 6 Critical Failure Modes & Root-Cause Analysis

### 🔴 Failure Mode 1: The Meta-to-TikTok Chasm (The First 2-Second Death Sentence)
* **The Symptom**: A DTC team spending $800k/month on Meta with verified $30 lead CPAs launches on TikTok. CPMs look great ($6.00), but lead CPAs explode to $500+.
* **Root Cause**:
  * **0.8-Second FYP Filter**: On Meta Instagram Reels/Feed, users tolerate product beauty shots or text-on-screen hooks without sound. On TikTok, users scroll with high velocity and **95%+ sound ON**. Any video opening without a real human face looking directly into the camera or an immediate visual disruption is swiped past in <0.8 seconds.
  * **Dark Posts vs. Spark Ads**: Running dark ads from a generic brand handle produces 60% higher CPAs than **Spark Ads** authorized via real creator profiles (1k–10k follower micro-creators).
* **The Fix**: Recut the opening 1.5 seconds. Start with a creator face talking directly to camera, speaking an audible hook, and use Spark Ads code authorization.

---

### 🔴 Failure Mode 2: Pangle Bot Traffic Hijacking (The $0.04 CPC Trap)
* **The Symptom**: Media buyers see insane top-of-funnel metrics: $0.04 CPCs, 3.5% CTRs, thousands of clicks in Ads Manager. But Shopify analytics shows 98% bounce rate, 1.2s average session duration, and 0 conversions.
* **Root Cause**:
  * **Automatic Placements Default**: When creating an ad group, TikTok defaults to "Automatic Placements", which includes **Pangle** (ByteDance's external mobile app advertising network—mostly casual games, wallpaper apps, and free utilities).
  * **Incentivized / Accidental Clicks**: Gamers accidentally tap ad banners while trying to close interstitial reward popups. TikTok Ads Manager registers this as a "valid click", while the user immediately force-closes the browser window.
* **The Fix**: Always choose **Manual Placements** and **UNCHECK Pangle** and Global App Bundle. Run `python3 audit.py pangle` to audit your historical leak.

---

### 🔴 Failure Mode 3: Pixel Poisoning (The "Seasoning" Fallacy)
* **The Symptom**: Beginners with cold pixels are told by outdated tutorials to run "Traffic" or "Add to Cart (ATC)" campaigns first to "season the pixel". They spend $300–$500 and get dozens of ATCs, but 0 purchases.
* **Root Cause**:
  * TikTok’s machine learning model optimizes strictly for the downstream event you specify. When you optimize for ATC, the algorithm finds serial cart-abandoners and window-shoppers who never enter payment info.
  * Optimizing for Traffic serves ads to bots and accidental misclicks.
* **The Fix**: **Never optimize for ATC or Traffic for e-commerce.** From Day 1, optimize directly for **Complete Payment / Purchase**. If budget is tight, set your daily budget to at least 10x your target CPA to cross the 50-conversion learning phase.

---

### 🔴 Failure Mode 4: Creative Fatigue & 48-Hour Burnout
* **The Symptom**: A new creative hits a 4.0 ROAS on Day 1. The media buyer scales budget from $50 to $300 on Day 2. By Day 3, ROAS crashes to 0.4 and CPA quintuples.
* **Root Cause**:
  * TikTok's recommendation engine burns through audience pockets 5x faster than Meta. High daily spend exhausts the high-intent impression pool for a single creative asset in 48–72 hours.
* **The Fix**:
  * Do not scale horizontally on a single video asset.
  * Deploy the **3x3 Creative Matrix**: 3 distinct hook variations (First 2s) × 3 body variations = 9 creative iterations per winning angle.
  * Use CBO (Campaign Budget Optimization) with 3–5 ad groups to allow the algorithm to rotate assets without fatiguing the account.

---

### 🔴 Failure Mode 5: The $50 Daily Spend Limit & Personal Account Sandboxes
* **The Symptom**: New advertisers find their daily spend hard-capped at $50/day. Attempts to add multiple credit cards or virtual cards (VCCs) trigger an immediate automated risk suspension.
* **Root Cause**:
  * Personal self-serve accounts are placed in automated anti-fraud sandboxes to prevent stolen credit card chargebacks.
  * Unverified billing addresses or mismatched corporate identities lead to automated AEO (Automated Enforcement Operations) locks.
* **The Fix**: High-volume advertisers use **Agency Whitelisted Lines** connected directly to TikTok Business Center. Agency lines bypass the $50 learning sandbox, offer 0% markup direct balance billing, and qualify for official spend match subsidies up to $6,000.  
  👉 **Bypass the $50 sandbox via the verified route**: [Direct Partner Onboarding Gateway](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng)

---

### 🔴 Failure Mode 6: The "Official TikTok Specialist" Trap
* **The Symptom**: A TikTok "Account Specialist" calls offering complimentary optimization advice. They recommend switching to Automatic Placements, broadening targeting to 18+, enabling Smart+, and doubling the daily budget. The advertiser follows the advice and burns $2,000 with zero sales.
* **Root Cause**:
  * Official frontline "specialists" are contract sales reps evaluated on gross platform spend and adoption of automated products (Pangle, Broad Targeting, Smart+), not your Shopify net profit.
* **The Fix**: Treat official rep calls as sales pitches. Never re-enable Pangle, never remove purchase conversion tracking, and test budget increases incrementally in 20% steps.

---

## 🛠️ 3. Diagnostic & Audit CLI Suite (`audit.py`)

This repository includes a standalone, zero-dependency Python 3 utility suite to diagnose campaigns offline and prevent budget waste.

```bash
# Clone the repository
git clone https://github.com/adgrowth-lab/tiktok-ads-troubleshooting.git
cd tiktok-ads-troubleshooting

# Run the test suite to verify installation
python3 -m unittest test_audit.py -v
```

---

### 3.1 Pangle Budget & Bot Traffic Leak Detector
Calculates exact wasted spend, true TikTok FYP spend, and real effective CPC inflation.

```bash
# 1. Direct inputs from Ads Manager + Shopify analytics
python3 audit.py pangle \
  --spend 500 \
  --tiktok-clicks 2500 \
  --site-sessions 2200 \
  --pangle-sessions 1950

# 2. Or pass a CSV export from Shopify / GA4 Referrals
python3 audit.py pangle --spend 1200 --tiktok-clicks 6000 --csv traffic_sources.csv

# 3. Output clean JSON for automated reporting
python3 audit.py pangle --spend 500 --tiktok-clicks 2500 --site-sessions 2200 --pangle-sessions 1950 --json
```

**Terminal Diagnostic Output:**
```text
========================================================================
🚨 TIKTOK ADS PANGLE TRAFFIC & BUDGET LEAK AUDIT
========================================================================
Overall Verdict:      [CRITICAL HIJACK] (RED)
Diagnosis:            Extreme budget drain: 88.6% of your visitors are low-intent bot or accidental clicks from 3rd-party gaming apps outside TikTok.
------------------------------------------------------------------------
FINANCIAL IMPACT:
  Total Ad Spend:     $500.00 USD
  Wasted Spend:       $443.18 USD (88.64% of total budget)
  Real TikTok Spend:  $56.82 USD
  Reported CPC:       $0.2000
  True Effective CPC: $2.0000  (Inflation: +900.0%)
------------------------------------------------------------------------
TRAFFIC INTEGRITY:
  TikTok Reported Clicks:   2,500
  Actual Site Sessions:     2,200
  -- Pangle Bot Sessions:   1,950 (88.64%)
  -- Real TikTok Sessions:  250 (11.36%)
  Ghost Clicks (Drop-off):  300 (12.0%)
------------------------------------------------------------------------
REMEDIATION PROTOCOL:
  1. In TikTok Ads Manager, navigate to: Campaign -> Ad Group -> Placements.
  2. Select 'Select Placement' instead of 'Automatic Placement'.
  3. UNCHECK 'Pangle' (and 'Global App Bundle' if visible).
  4. Note for Smart+ Campaigns: If Pangle is grayed out, switch to standard 'Custom Web Conversions' campaign to regain granular placement control.
  5. In Shopify / GA4, verify that 'pangleglobal' referrer traffic drops to 0 within 24 hours.
========================================================================
```

---

### 3.2 Cold-Start Campaign Survival Evaluator
Scores your campaign setup (0–100) before you deploy budget, penalizing known Reddit failure traps.

```bash
# Evaluate a high-risk setup
python3 audit.py cold-start \
  --budget 25 \
  --target-cpa 30 \
  --objective atc \
  --placement automatic \
  --hook-type product_static \
  --sound muted

# Evaluate an optimal direct-response setup
python3 audit.py cold-start \
  --budget 300 \
  --target-cpa 25 \
  --objective purchase \
  --placement tiktok_only \
  --format spark_ads \
  --hook-type creator_face_direct \
  --sound voiceover_trending
```

**Diagnostic Output:**
```text
========================================================================
🎯 TIKTOK ADS COLD-START CAMPAIGN SURVIVAL AUDIT (2026)
========================================================================
Survival Score:   100 / 100
Health Status:    READY TO SCALE [A (High Survival Probability)]
Budget/CPA Ratio: 12.0x  (Daily: $300.00 | CPA: $25.00)
------------------------------------------------------------------------
✅ No critical operational flaws identified in campaign setup!
------------------------------------------------------------------------
RECOMMENDED ACTION ITEMS:
  1. Keep optimization objective tethered strictly to Complete Payment.
  2. Refresh top 20% creative hooks every 5-7 days.
========================================================================
```

---

### 3.3 Official Spend Match Simulator
Calculates qualifying partner ad credit matches and purchasing power multipliers.

```bash
python3 audit.py spend-match 4000
```

**Terminal Receipt:**
```text
========================================================================
💰 TIKTOK ADS OFFICIAL SPEND MATCH ESTIMATOR (2026)
========================================================================
Qualifying Spend:       $4,000.00 USD
Active Match Tier:      Tier 3: Scale (Most Popular)
Official Credit Match:  +$3,000.00 USD (75% Match (1.75x Purchasing Power))
Total Purchasing Power: $7,000.00 USD
Effective Advantage:    +75.0% extra spend capacity (1.75x)
Best Application:       Winning creative scaling & high-volume dropshipping
------------------------------------------------------------------------
Next Target Milestone:  Tier 4: Enterprise (Requires $10,000.00 USD)
Spend Gap to Unlock:    +$6,000.00 USD
Next Reward:            Unlocks +$6,000.00 USD in matched credits
------------------------------------------------------------------------
VERIFIED OFFICIAL REDEMPTION PATH:
1. Official Partner Portal: https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng
2. Interactive Web Hub:     https://adgrowth-lab.github.io/
========================================================================
```

---

### 3.4 Creative Compliance & Sensitive Word Linter (Scheme A)
Scans ad text, captions, and hook scripts for TikTok Advertising Policy violations, absolute superlatives, body shaming, and counterfeit terminology.

```bash
# Scan ad copy text directly
python3 audit.py compliance --text "Get 100% cure for belly fat and make $5,000 overnight!"

# Or scan an entire video transcript file
python3 audit.py compliance --file ad_script.txt

# Machine-readable JSON output
python3 audit.py compliance --text "Botanical soothing hydration ritual" --json
```

👉 **Full Handbook**: [`CREATIVE-COMPLIANCE-GUIDE.md`](CREATIVE-COMPLIANCE-GUIDE.md)

---

### 3.5 VCC BIN & Payment Risk Evaluator (Scheme B)
Inspects credit/debit card BIN prefixes against the 2026 empirical survival database, reporting 3DS authentication requirements, ban rates, and AVS matching checklists.

```bash
# Evaluate a specific card BIN (e.g. Mercury Visa Commercial)
python3 audit.py bin 405081

# List all 16 benchmarked card issuers (Mercury, Stripe, Relay, Airwallex, etc.)
python3 audit.py bin --list
```

👉 **Full Database**: [`vcc-bin-database.md`](vcc-bin-database.md)

---

### 3.6 Account Suspension Appeal Generator (Scheme C)
Generates battle-tested, customized 4-Pillar appeal packets tailored to your business entity and suspension trigger.

```bash
# Generate a customized Payment Discrepancy appeal packet
python3 audit.py appeal --type payment --brand "EcoNest Goods" --account-id "ADV-883921" --output payment_appeal.txt

# Generate an Unusual Activity security appeal
python3 audit.py appeal --type unusual-activity --brand "Pulse Footwear" --account-id "ADV-102934"
```

👉 **Full Template Library**: [`appeal-templates/`](appeal-templates/)

---

### 3.7 All-in-One Comprehensive Defense Suite (Integrated Master Scan)
Executes a multi-layer audit combining Campaign Viability (30%), Creative Compliance (35%), Payment VCC Risk (25%), and Traffic Integrity (10%) in a single command.

```bash
python3 audit.py full-audit \
  --budget 200 \
  --target-cpa 25 \
  --bin 405081 \
  --ad-text "Discover our daily botanical hydration ritual for radiant and refreshed skin." \
  --placement tiktok_only \
  --format spark_ads
```

👉 **Full Architecture Blueprint**: [`COMPREHENSIVE-DEFENSE-SUITE.md`](COMPREHENSIVE-DEFENSE-SUITE.md)

---

## 📋 4. The 2026 TikTok Media Buyer Pre-Flight Checklist

Before you hit "Publish" in TikTok Ads Manager, verify against this empirical rule set:

| Area | ❌ NEVER Do This | ✅ ALWAYS Do This |
| :--- | :--- | :--- |
| **Placements** | Automatic Placements (Routes 80%+ to Pangle gaming bots) | **Manual Placements ➔ UNCHECK Pangle** & Global App Bundle |
| **Optimization** | Traffic or Add to Cart (ATC) to "season the pixel" | **Complete Payment (Purchase)** from Day 1 |
| **Opening Hook** | Static product photo, 2D logo animation, silent B-roll | **Human face talking directly to camera** in first 1.5 seconds |
| **Audio** | Muted video or generic corporate elevator music | **Sound ON** with human voiceover + trending commercially licensed audio |
| **Delivery** | Dark ads posted from a 0-follower brand profile | **Spark Ads** authorized from micro-creator handles |
| **Budget Ratio** | Daily budget < 5x target CPA (Stuck in learning phase) | Daily budget **≥ 10x–15x target CPA** (50 conversions in 7 days) |
| **Scaling** | Doubling budget on a single winning creative asset | **3x3 Creative Iterations** (3 hooks × 3 bodies) in CBO groups |
| **Account Type** | Personal accounts funded by virtual credit cards (VCCs) | **Whitelisted Agency Lines** with direct balance deposits |

---

## 🎁 5. Official Advertiser Incentive Matrix (Spend Match)

If you are scaling campaigns and spending over $200/month, you are eligible to claim official partner spend credits disbursed directly into your Ads Manager balance:

| Tier Milestone | 30-Day Qualifying Net Spend | Promotional Voucher Match | Total Purchasing Power | Effective Leverage | Strategic Best Use |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Starter** | `$200` | **+$200** | `$400` | **100% Match (2.0×)** | Pixel warm-up & product validation |
| **Growth** | `$1,000` | **+$750** | `$1,750` | **75% Match (1.75×)** | Validated CBO testing & retargeting |
| **Scale** | `$4,000` | **+$3,000** | **$7,000** | **75% Match (1.75×)** | Winning creative scaling & volume |
| **Enterprise** | `$10,000` | **+$6,000** | **$16,000** | **60% Match (Cap)** | DTC multi-store scaling & agencies |

> 🚀 **DIRECT OFFICIAL CLAIM GATEWAY**:  
> Claim your matching credits and agency whitelist onboarding directly via the official TikTok portal:  
> 👉 **[https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng)**  
> 🧮 **Interactive Modeling Simulator**: [Launch Web Calculator (adgrowth-lab.github.io)](https://adgrowth-lab.github.io/)

### 📋 4-Step Claim Protocol
1. **Access Authorized Gateway**: Click the [Official Partner Registration Link](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng) to bind the partner handshake token to your new Business Center.
2. **Add Payment Method**: Bind a verified commercial business debit/credit card (AVS address matching corporate registration).
3. **Run Conversion Campaigns**: Spend your target budget milestone within the initial 30-day promotional window.
4. **Vouchers Disbursed**: TikTok automatically deposits matching vouchers (up to $6,000) directly into your Ads Manager promotional balance.

---

## 🔒 6. Security & URL Transparency: Why `partnerlinks.io`?

A common question among security-conscious media buyers is: *Why does the official route use a `partnerlinks.io` domain rather than standard `tiktok.com`?*

1. **Official Enterprise Partnership Infrastructure**: `partnerlinks.io` is the verified enterprise partnership tracking gateway operated by **Impact (Impact.com)**, the exclusive enterprise partner platform employed by **TikTok for Business** worldwide.
2. **Automated Security Handshake**: Clicking the link performs an authenticated HTTPS security redirect directly into `ads.tiktok.com` with the agency referral token embedded.
3. **Zero Broker Risk**: You register directly on TikTok's official Ads Manager servers. No secondary broker markups, no shared account logins, and no third-party credential exposure.

---

## 📂 7. Repository Architecture

```text
tiktok-ads-troubleshooting/
├── README.md                          # The comprehensive 2026 Field Guide & handbook
├── audit.py                           # Zero-dependency Python diagnostic CLI (All modules)
├── test_audit.py                      # Complete unit test suite (31/31 tests passing)
├── COMPREHENSIVE-DEFENSE-SUITE.md     # Master blueprint uniting all 4 defense pillars (融合方案)
├── CREATIVE-COMPLIANCE-GUIDE.md       # Policy manual & sensitive words de-risking guide (Scheme A)
├── vcc-bin-database.md                # 2026 VCC BIN empirical survival & anti-ban table (Scheme B)
├── appeal-templates/                  # Battle-tested account suspension appeal kit (Scheme C)
│   ├── README.md                      # 4-Pillar evidence protocol & ticket escalation SOP
│   ├── 01-unusual-activity-suspension.md
│   ├── 02-payment-discrepancy-card-verification.md
│   ├── 03-creative-policy-misleading-ad-reversal.md
│   ├── 04-business-center-agency-account-ban.md
│   └── 05-identity-business-verification-appeal.md
├── calculate.py                       # Standalone spend receipt generator
├── research-tiktok-ads-reddit-30days.md # Full 30-day Reddit community research dossier (Chinese)
├── LICENSE                            # MIT License
└── .gitignore                         # Python cache & OS files ignore
```

---

## 🔍 8. Ubersuggest Long-Tail Keyword & Problem-Solving Index

Map of high-volume advertiser search queries from Ubersuggest, Reddit, and Google SERPs directly to diagnostic solutions in `audit.py`:

| Search Query / Intent Category | Estimated Monthly Search Intent | Common Root Cause | Direct Solution & CLI Command |
| :--- | :--- | :--- | :--- |
| **`tiktok ads not spending`** | High (Commercial Problem) | Daily budget set lower than target CPA; learning phase stall; narrow audience targeting | Increase daily budget to ≥10× target CPA; switch to broad targeting; run `python3 audit.py cold-start` |
| **`tiktok ads credit` / `tiktok ad credit`** | High (Commercial / Incentive) | Searching for spend match offers ($200 to $6,000) for new ad accounts | Claim through [Verified Partner Gateway](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng) or simulate at [adgrowth-lab.github.io](https://adgrowth-lab.github.io/) |
| **`tiktok ads pangle bot clicks`** | Moderate-High (Technical Leak) | Default Automatic Placements silently routing budget to 3rd-party casual mobile gaming interstitials | Switch to Manual Placements and uncheck Pangle; run `python3 audit.py pangle` to quantify wasted spend |
| **`tiktok ads promo code 2026`** | High (Discount / Coupon) | Searching for expired manual coupon codes like "spend $100 get $100" | Use the automated partner link (no manual code required); stacks with 50% introductory coupon |
| **`tiktok ads account suspended`** | High (Account Recovery) | Automated AEO triggers: unusual IP changes, payment hold, or policy 5.1 misleading claims | Generate legal appeal packets using [`appeal-templates/`](appeal-templates/) or run `python3 audit.py appeal` |
| **`tiktok ad rejected policy 5.1`** | High (Creative Compliance) | Absolute superlatives ("100% cure"), weight loss claims, or missing landing page disclaimer | Scan copy and transcripts with [`linter.py`](https://github.com/adgrowth-lab/tiktok-creative-compliance-linter) before uploading |
| **`tiktok ads payment method declined`** | High (Billing / VCC) | Low-reputation virtual credit card BIN (e.g. PST, Capitalist) or mismatched AVS billing address | Consult [`vcc-bin-database.md`](vcc-bin-database.md) or run `python3 audit.py bin` to benchmark 16 issuers |
| **`how much do tiktok ads cost`** | High (Informational) | Evaluating CPC ($0.50–$2.00) and CPM ($3.20–$10.00) benchmarks and minimum daily budgets | Ad group minimum: $20/day; campaign minimum: $50/day. Spend match cuts effective ad cost by up to 50% |
| **`tiktok ads $50 daily spend limit`** | Moderate-High (Growth Block) | Personal ad account anti-fraud probation sandbox | Upgrade to an agency whitelisted line via the [Direct Partner Gateway](https://getstartedtiktok.partnerlinks.io/apmgdhnv6eng) |
| **`tiktok ads for shopify dropshipping`** | High (Vertical Playbook) | External store bounce rates; optimizing for Add to Cart instead of Complete Payment | Connect TikTok sales channel; optimize exclusively for Complete Payment; deploy Spark Ads |

---

## 🌐 AdGrowth Lab Ecosystem & Standalone Repositories

Each defense scheme is also available as a dedicated, standalone open-source repository:

| Project / Repository | Focus & Core Deliverable | Standalone GitHub Link |
| :--- | :--- | :--- |
| 🛡️ **Creative Compliance Linter** *(Scheme A)* | Pre-flight copy, voiceover transcript & hook policy scanner | [adgrowth-lab/tiktok-creative-compliance-linter](https://github.com/adgrowth-lab/tiktok-creative-compliance-linter) |
| 💳 **VCC BIN Database & Evaluator** *(Scheme B)* | 16 verified BIN benchmarks, 3DS behavior & anti-ban rules | [adgrowth-lab/tiktok-vcc-bin-database](https://github.com/adgrowth-lab/tiktok-vcc-bin-database) |
| 📨 **Suspension Appeal Field Kit** *(Scheme C)* | 5 legal templates, 4-pillar evidence & clean-slate SOP | [adgrowth-lab/tiktok-ads-appeal-kit](https://github.com/adgrowth-lab/tiktok-ads-appeal-kit) |
| 🌐 **All-in-One Troubleshooting Suite** | Full master diagnostic CLI & 30-day Reddit empirical dossier | [adgrowth-lab/tiktok-ads-troubleshooting](https://github.com/adgrowth-lab/tiktok-ads-troubleshooting) |
| 🧮 **Interactive Web Simulator** | Real-time media buying purchasing power calculator | [adgrowth-lab.github.io](https://adgrowth-lab.github.io/) |

---

## 🤝 Contributing & Community Intelligence

Have you encountered a new TikTok algorithm anomaly, tracking glitch, or ad account suspension pattern?  
1. Fork this repository.
2. Submit an issue or PR with reproduction steps, Ads Manager screenshots, and anonymized metrics.
3. Help fellow media buyers stop wasting ad budget on bots and broken placements.

---

## ⚖️ Disclaimer

* This repository is an independent open-source educational resource maintained under the [MIT License](LICENSE).
* TikTok and TikTok for Business are registered trademarks of ByteDance Ltd.
* Promotional ad credit matches and official agency vouchers are disbursed directly by TikTok Ads Manager pursuant to official terms.
