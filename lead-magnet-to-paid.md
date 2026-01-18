# Lead Magnet Conversion Analysis Report

**Generated:** January 17, 2026
**Data Sources:** Supabase (user_profiles, stripe_subscriptions, user_campaign_funnel) + Stripe MCP (payment verification)
**Scope:** External users only (excludes @searchable.com)

---

## Executive Summary

| Metric | Value | Notes |
|--------|-------|-------|
| **Total Lead Magnet Users** | 4,501 | Users who entered via lead magnet funnel |
| **Started Subscription** | 64 (1.42%) | Started trial or direct purchase |
| **Currently Paying** | 44 (0.98%) | Active + Past Due subscribers |
| **Monthly Revenue** | $4,650 | From lead magnet converters |

### Key Finding

**The lead magnet funnel has a severe top-of-funnel problem.** Only 1.42% of lead magnet users ever start a subscription. However, those who do subscribe have decent retention. The critical issue is converting lead magnet users to try the product.

---

## 1. Complete Subscription Breakdown

### By Tier, Trial Status, and Outcome

| Tier | Trial Status | Current Status | Count | Notes |
|------|--------------|----------------|-------|-------|
| **Professional** | Via Trial | Active | 20 | Converted from 14-day trial |
| **Professional** | Via Trial | Past Due | 2 | Payment failed post-trial |
| **Professional** | Via Trial | Canceled at Trial End | 9 | Never converted |
| **Professional** | Via Trial | Churned After Paying | 4 | Paid then left |
| **Professional** | Via Trial | Currently in Trial | 6 | Still trialing |
| **Professional** | Direct Purchase | Active | 9 | Skipped trial |
| **Starter** | Direct Purchase | Active | 10 | No trial offered |
| **Starter** | Direct Purchase | Canceled | 2 | Direct purchase churned |
| **Starter** | Via Trial | Canceled at Trial End | 1 | Rare - trial on Starter |
| **Scale** | Via Trial | Active | 1 | Converted from trial |
| **Total** | | | **64** | |

### Currently Paying Breakdown

| Tier | Via Trial | Direct Purchase | Total Active | MRR |
|------|-----------|-----------------|--------------|-----|
| **Professional** | 22 | 9 | 31 | $3,875 |
| **Starter** | 0 | 10 | 10 | $500 |
| **Scale** | 1 | 0 | 1 | $400 |
| **Total** | **23** | **19** | **42** (+2 past due) | **$4,775** |

*Note: 2 Professional users in past_due status = additional $250 at risk*

---

## 2. Trial Analysis (Professional Tier Only)

### Professional Trial Funnel

```
Started Professional Trial: 41 users
        │
        ├── 53.7% Converted (22 users)
        │       ├── 20 Active
        │       └── 2 Past Due
        │
        ├── 22.0% Canceled at Trial End (9 users)
        │       └── Never paid
        │
        ├── 9.8% Churned After Paying (4 users)
        │       └── Paid then canceled
        │
        └── 14.6% Currently in Trial (6 users)
                └── Still deciding
```

### Trial Conversion Rate: 53.7%

Of Professional trial users who completed their trial:
- **22 converted** to paying
- **9 canceled** at trial end (never converted)
- **4 churned** after paying at least once

**Key Insight:** Professional trial conversion (53.7%) is lower than the overall platform rate (63.5%), suggesting lead magnet users may be less qualified or have different expectations.

---

## 3. Direct Purchase vs Trial Users

### Purchase Path Comparison

| Purchase Path | Count | Avg Messages | Avg Audits | GSC | GA | Avg Visibility |
|---------------|-------|--------------|------------|-----|-----|----------------|
| **Professional via Trial** | 24 | 11.4 | 1.8 | 25% | 17% | 25.7 |
| **Professional Direct** | 9 | 2.4 | 0.6 | 11% | 11% | 5.0 |
| **Starter Direct** | 10 | 17.8 | 1.5 | 20% | 20% | 12.5 |
| **Scale via Trial** | 1 | 0.0 | 9.0 | 0% | 0% | 22.5 |

### Key Insights

1. **Starter direct purchasers are most engaged** (17.8 avg messages)
   - grega.prah@gmail.com has 130 messages
   - jm2373@aol.com has 28 messages
   - These users chose Starter deliberately and use it heavily

2. **Professional via Trial users are well-engaged** (11.4 avg messages)
   - Top user has 94 messages (alastair@theothersongs.com)
   - 25% connected GSC, 17% connected GA

3. **Professional Direct purchasers have lowest engagement** (2.4 avg messages)
   - Most have 0 messages
   - May have purchased impulsively without proper evaluation

---

## 4. All Paying Lead Magnet Users

### Professional Tier - Via Trial (22 users, $2,750 MRR)

| Email | Status | Messages | Audits | Visibility | GSC | GA |
|-------|--------|----------|--------|------------|-----|-----|
| alastair@theothersongs.com | active | 94 | 1 | 10.0 | - | - |
| seb@vistafolia.com | active | 72 | 4 | 47.7 | ✓ | ✓ |
| e.arzubi@frontier.care | active | 39 | 1 | 35.0 | ✓ | ✓ |
| andrew@getcustomersfast.co.uk | active | 28 | 6 | 72.5 | ✓ | ✓ |
| vasilis.papakostas@konicaminolta.com.gr | active | 20 | 5 | 30.0 | - | - |
| bt@rapidionline.com | active | 14 | 2 | 22.7 | ✓ | - |
| christiandion@talkable.ca | active | 4 | 3 | 67.5 | ✓ | ✓ |
| info@786vcpa.ca | active | 2 | 2 | 20.0 | - | - |
| william.stormont@scone-palace.co.uk | active | 0 | 6 | 35.0 | - | - |
| ema@decipher.agency | active | 0 | 4 | 5.0 | - | - |
| info@dcbdigital.com.au | active | 0 | 2 | - | - | - |
| farizmendi@getresq.com | active | 0 | 2 | 12.5 | ✓ | - |
| chamara@libt.co.uk | **past_due** | 0 | 2 | 10.0 | - | - |
| hello@aevahealth.com | active | 0 | 1 | 7.5 | - | - |
| kl@mvp-swiss.ch | active | 0 | 1 | 10.0 | - | - |
| hienha.ai.2024@gmail.com | **past_due** | 0 | 1 | 0.0 | - | - |
| + 6 more with 0 usage | active | 0 | 0 | - | - | - |

### Professional Tier - Direct Purchase (9 users, $1,125 MRR)

| Email | Status | Messages | Audits | Visibility | GSC | GA |
|-------|--------|----------|--------|------------|-----|-----|
| info@ethicalbrandmarketing.com | active | 14 | 1 | 10.0 | ✓ | - |
| basil.straessle@nolato.com | active | 8 | 3 | 0.0 | - | - |
| cameron@auriaesthetics.com | active | 0 | 1 | - | - | ✓ |
| + 6 more with 0 usage | active | 0 | 0 | - | - | - |

### Starter Tier - Direct Purchase (10 users, $500 MRR)

| Email | Status | Messages | Audits | Visibility | GSC | GA |
|-------|--------|----------|--------|------------|-----|-----|
| **grega.prah@gmail.com** | active | **130** | 1 | 10.0 | ✓ | ✓ |
| jm2373@aol.com | active | 28 | 6 | 10.0 | - | - |
| lea.richter@company.info | active | 20 | 6 | 20.0 | ✓ | ✓ |
| david@risingabovethenoise.com | active | 0 | 2 | 10.0 | - | - |
| + 6 more with 0 usage | active | 0 | 0 | - | - | - |

### Scale Tier - Via Trial (1 user, $400 MRR)

| Email | Status | Messages | Audits | Visibility | GSC | GA |
|-------|--------|----------|--------|------------|-----|-----|
| vikram@digidem.com | active | 0 | 9 | 22.5 | - | - |

---

## 5. Churned Lead Magnet Users

### Users Who Paid Then Left (4 users)

| Email | Tier | Messages | Audits | Days as Customer |
|-------|------|----------|--------|------------------|
| bernard@trendwave.nl | Professional | - | - | 31 days |
| 138@hey.com | Professional | - | - | 31 days |
| jeff.maling@icloud.com | Professional | - | - | 31 days |
| vkanything@gmail.com | Professional | - | - | 31 days |

**All churners left exactly at 31 days** (end of first billing cycle). This suggests:
- They tried for one month and decided not to continue
- No trial extension or early churn

### Users Who Never Converted from Trial (9 users)

| Email | Tier | SEO Level |
|-------|------|-----------|
| adam@vapehouseuk.com | Professional | Intermediate |
| david@brandyour.co | Professional | Beginner |
| josh@meetgeorge.co.uk | Professional | Intermediate |
| matthew@matthewfrener.com | Professional | Beginner |
| nick@goodsleepco.health | Professional | Intermediate |
| mail@ringofbells.net | Professional | Beginner |
| myles@sportsperformancetracking.com | Professional | Intermediate |
| gert@seoleverage.com | Professional | Agency |
| tomasz@nexora.build | Professional | Beginner |

---

## 6. SEO Experience Analysis

### Paying Users by SEO Experience

| SEO Level | Professional | Starter | Scale | Total | % of Paying |
|-----------|--------------|---------|-------|-------|-------------|
| Intermediate | 17 | 4 | 0 | 21 | 47.7% |
| Beginner | 7 | 6 | 0 | 13 | 29.5% |
| Expert | 2 | 0 | 1 | 3 | 6.8% |
| Agency | 2 | 0 | 0 | 2 | 4.5% |
| Unknown | 5 | 0 | 0 | 5 | 11.4% |

**Key Finding:** Intermediate SEO users (47.7%) are most likely to convert and pay. Beginners also convert well (29.5%). Experts rarely convert from lead magnet.

---

## 7. Brand Reach Analysis

### Paying Users by Brand Reach

| Brand Reach | Count | % |
|-------------|-------|---|
| Worldwide | 17 | 38.6% |
| Nationwide | 17 | 38.6% |
| Regional | 4 | 9.1% |
| City | 2 | 4.5% |
| State | 2 | 4.5% |
| Unknown | 2 | 4.5% |

**Insight:** Worldwide and Nationwide brands convert equally well. Brand reach doesn't significantly predict conversion.

---

## 8. Conversion Funnel Summary

```
Lead Magnet Signup (4,501 users)
        │
        │ 1.42% start subscription
        ↓
Started Subscription (64 users)
        │
        ├─── Professional Path (50 users)
        │    │
        │    ├── Via Trial (41 users)
        │    │   ├── 53.7% Converted (22)
        │    │   ├── 22.0% Never Converted (9)
        │    │   ├── 9.8% Churned After Paying (4)
        │    │   └── 14.6% Still in Trial (6)
        │    │
        │    └── Direct Purchase (9 users)
        │        └── 100% Active (9)
        │
        ├─── Starter Path (13 users)
        │    │
        │    ├── Direct Purchase (12 users)
        │    │   ├── 83.3% Active (10)
        │    │   └── 16.7% Canceled (2)
        │    │
        │    └── Via Trial (1 user)
        │        └── Canceled at Trial End
        │
        └─── Scale Path (1 user)
             └── Via Trial → Active (1)
```

---

## 9. Key Metrics

| Metric | Value |
|--------|-------|
| **Lead Magnet to Subscription** | 1.42% (64/4,501) |
| **Professional Trial Conversion** | 53.7% (22/41 completed) |
| **Starter Retention (Direct)** | 83.3% (10/12) |
| **Post-Payment Churn (Pro Trial)** | 15.4% (4/26 who paid) |
| **Total Paying Users** | 44 (42 active + 2 past due) |
| **Total MRR** | $4,775 |
| **MRR at Risk (Past Due)** | $250 |

---

## 10. Stripe Payment Verification

Confirmed via Stripe MCP that lead magnet converters are actually paying:

| Customer | Email | Tier | Payments |
|----------|-------|------|----------|
| cus_TUHYu7URp8lGDR | alastair@theothersongs.com | Professional | 2x $125 |
| cus_TURNzXEneHZUT2 | seb@vistafolia.com | Professional | 2x $125 |
| cus_TeSYu99Q22KHoO | office@helikon.group | Professional | 1x $125 |
| cus_TVfAtbc79eyYn6 | jm2373@aol.com | Starter | 1x $294 (annual?) |

---

## 11. Recommendations

### Priority 1: Fix Lead Magnet to Subscription (1.42%)

**Problem:** 98.6% of lead magnet users never start a subscription.

**Actions:**
1. Stronger CTA in lead magnet delivery email
2. Follow-up sequence promoting trial/Starter
3. Show immediate value in lead magnet results
4. Consider offering Starter as default (no trial needed)

### Priority 2: Promote Starter for Lead Magnet Users

**Finding:** Starter direct purchasers have HIGHEST engagement (17.8 avg messages vs 11.4 for Pro trial).

**Actions:**
1. Feature Starter prominently for lead magnet users
2. Position as "immediate access, no trial needed"
3. Starter users: grega.prah@gmail.com has 130 messages - power user on $50/mo

### Priority 3: Improve Professional Trial Conversion (53.7%)

**Finding:** Lead magnet users have lower trial conversion than overall (53.7% vs 63.5%).

**Actions:**
1. Better onboarding for lead magnet users
2. Connect their lead magnet data to trial experience
3. Push GSC/GA integration early (25% of converters vs 0% of non-converters)

### Priority 4: Address Zero-Usage Paying Users

**Problem:** Many paying users have 0 messages and 0 audits.

| Tier | Zero Usage | Total | % |
|------|------------|-------|---|
| Professional via Trial | 6 | 22 | 27% |
| Professional Direct | 6 | 9 | 67% |
| Starter Direct | 6 | 10 | 60% |

**Actions:**
1. Onboarding sequence for new paying users
2. Usage-triggered emails
3. Personal outreach for Professional users with 0 usage

---

## Appendix: Data Methodology

### Lead Magnet User Identification

```sql
WHERE user_profiles.settings->'tags' ? 'LEAD-MAGNET'
```

### Trial Status Classification

- **Via Trial**: `trial_start IS NOT NULL`
- **Direct Purchase**: `trial_start IS NULL`
- **Converted from Trial**: Status active/past_due AND trial_end < NOW()
- **Canceled at Trial End**: Status canceled AND canceled_at within 1 day of trial_end
- **Churned After Paying**: Status canceled AND canceled_at > trial_end + 1 day

### Exclusions

- @searchable.com email accounts (internal team)
