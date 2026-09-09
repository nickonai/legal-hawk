# US Negative Option & Subscription Enforcement: FTC, ROSCA, Visa/Mastercard

> **Last updated:** 2026-06-18
> **Scope:** Online subscription merchants selling to US consumers via negative option / free-trial funnels
> **Risk level:** CRITICAL — FTC enforcement is at an all-time high; asset freezes and 8-figure judgments are routine

---

## 1. Core Legal Framework

### 1.1 FTC Act Section 5(a) — 15 U.S.C. § 45(a)

Prohibits "unfair or deceptive acts or practices in or affecting commerce."

- **Deceptive:** A representation, omission, or practice that is likely to mislead a consumer acting reasonably under the circumstances
- **Unfair:** Causes or is likely to cause substantial injury to consumers that they cannot reasonably avoid and that is not outweighed by countervailing benefits (15 U.S.C. § 45(n))
- **Penalty:** Civil penalties up to **$53,088 per violation** (2025 amount, adjusted annually for inflation). Each transaction shown to each consumer can be a separate violation.

### 1.2 ROSCA — Restore Online Shoppers' Confidence Act (15 U.S.C. §§ 8401–8405)

Enacted 2010. Applies to **any internet transaction involving a negative option feature.**

**Section 4 of ROSCA (15 U.S.C. § 8403) — Three mandatory requirements:**

| Requirement | Statute | What It Means |
|---|---|---|
| **Clear and Conspicuous Disclosure** | § 8403(1) | All material terms disclosed *before* obtaining billing info |
| **Express Informed Consent** | § 8403(2) | Consumer must affirmatively consent before any charge |
| **Simple Cancellation Mechanism** | § 8403(3) | Must provide a simple mechanism to stop recurring charges |

**Negative Option Feature Definition (TSR 16 C.F.R. § 310.2(w)):**
> "In an offer or agreement to sell or provide any goods or services, a provision under which the consumer's silence or failure to take an affirmative action to reject goods or services or to cancel the agreement is interpreted by the seller as acceptance of the offer."

This covers: free trials converting to paid, subscriptions that auto-renew, any "cancel to avoid charges" structure.

**ROSCA penalty:** Violations are treated as violations of an FTC rule under Section 18 of the FTC Act (15 U.S.C. § 57a(d)(3)), authorizing civil penalties, rescission, monetary relief, and public notification. *Each ROSCA violation is also a Section 5 FTC Act violation.*

**Relief available (Section 19, 15 U.S.C. § 57b):** Monetary relief, rescission or reformation of contracts, refund of money or return of property, and public notification respecting the rule violation.

### 1.3 FTC Negative Option Rule (16 CFR Part 425)

Amended October 2024 ("Click-to-Cancel Rule"). Vacated by federal court July 2025 (National Advertisers v. FTC). However:
- FTC re-proposed similar requirements via ANPRM January 2026
- Vacated rule provisions serve as explicit FTC enforcement priorities under Section 5
- Core principle stands: **cancellation must be at least as easy as enrollment**

---

## 2. The "Clearly and Conspicuously" Standard

This is the critical legal test. Courts and the FTC apply an **8-part test** (established in FTC enforcement and TRO orders):

A disclosure is "clearly and conspicuous" only if it:

1. **Is unavoidable** — consumer cannot proceed without encountering it; not hidden below the fold or behind a link
2. **Is not buried in fine print** — stands out from surrounding text in size, contrast, and placement
3. **Is not contradicted** — not inconsistent with other messages on the page (e.g., "personalized plan" headline contradicts buried "generic content" disclaimer)
4. **Is in the correct medium** — video disclosures for video ads; audio disclosure for audio; text disclosure for text
5. **Is in the target audience's language** — not in English if ad is in Spanish, etc.
6. **Is device-agnostic** — visible and functional on mobile, tablet, and desktop without requiring additional scrolling or interaction
7. **Has adequate type size and contrast** — not gray text on gray background; not smallest text on the page; not obscured by competing visual elements
8. **Is presented before billing information is obtained** — not after the consumer has entered their card number

**Common violations from FTC enforcement:**
- Subscription terms in smallest font on page in gray text on gray background (FTC v. Genesis Tech, 2026)
- Fine print that "might appear below the fold" depending on screen size (same case)
- Terms accessible only via hyperlink in subscription policy user must affirmatively seek (same case)
- Terms contradicted by page heading that implies one-time purchase (same case)
- Payment overlay that shows only transaction amount with no mention of recurring fee (same case)

---

## 3. Five FTC Violation Counts (ROSCA Framework)

Based on FTC v. GM UniverseApps Ltd. (Genesis Tech enterprise), Case No. 4:26-cv-05232-HSG (N.D. Cal. 2026) — the most comprehensive recent ROSCA enforcement action covering 8 subscription products:

| Count | Legal Basis | Conduct |
|---|---|---|
| **Count I** | FTC Act § 5(a), 15 U.S.C. § 45(a) | Failure to disclose material terms of offer (subscription enrollment, recurring charge amount, cancellation terms) |
| **Count II** | FTC Act § 5(a), (n), 15 U.S.C. § 45(a), (n) | Charging consumers without authorization (undisclosed subscriptions, double billing, unauthorized add-on purchases) |
| **Count III** | ROSCA § 4(1), 15 U.S.C. § 8403(1) | Failure to clearly and conspicuously disclose all material terms before obtaining billing information |
| **Count IV** | ROSCA § 4(2), 15 U.S.C. § 8403(2) | Failure to obtain express informed consent before charging |
| **Count V** | ROSCA § 4(3), 15 U.S.C. § 8403(3) | Failure to provide simple mechanisms to stop recurring charges |

---

## 4. The Quiz Funnel Deception Pattern

### 4.1 What It Is

A quiz funnel is a conversion flow that uses interactive questions to create the impression of personalization before presenting a subscription offer. It is widely used in health, wellness, fitness, education, astrology, and productivity apps.

**The FTC has identified this as deceptive when:**
1. Quiz results are predetermined regardless of user answers (Wisey: all users "have ADHD" regardless of symptoms indicated)
2. Personalization is fake — delivered content is generic and does not reflect quiz answers
3. Quiz creates emotional investment ("sunk cost") that overcomes rational evaluation of terms
4. The "personalized plan" frame contradicts buried subscription terms
5. Progress animations and countdown timers create false urgency

### 4.2 The Five-Step Fraudulent Funnel (Genesis Tech / FTC 2026)

| Step | Mechanism | Legal Issue |
|---|---|---|
| **1. Personalized Hook** | Social media ad → quiz promising personalized diagnosis/plan | OK if quiz results actually personalize content |
| **2. Sunk Cost Investment** | Multi-step quiz (10–20 questions) + encouraging messages + "plan loading" animation | Dark pattern — investment creates emotional bias |
| **3. Hidden Subscription Terms** | "Plan" presented with CTA button; subscription terms in smallest text below button, gray-on-gray, below the fold | Violates ROSCA § 8403(1) and FTC Act § 5(a) |
| **4. Double Charging / Upsell Trap** | Post-purchase upsell screen disguised as "confirmation" or "free add-on"; one click = additional subscription charge | Violates FTC Act § 5(a)(n) — unauthorized charge |
| **5. Obstruction of Cancellation** | No cancel button in settings; customer service ignores emails; continues billing after confirmed cancellation | Violates ROSCA § 8403(3) |

### 4.3 Specific Deceptive Mechanics (from Case Evidence)

- **Countdown timer that resets:** 10-minute "offer ends in" timer resets when user interacts with the spin wheel — fake urgency
- **Spin wheel always lands on "biggest discount":** Fabricated scarcity/discount mechanism
- **Pre-selected plan:** 1-month plan pre-selected as "MOST POPULAR" with radio button already filled
- **Payment overlay omits subscription:** PayPal payment form shows only "$19.99" with no mention of $59.99/month recurring charge
- **"Unlock" button charges without confirmation:** Dashboard upsell with "Unlock Training" button initiates charge without a confirmation step
- **Trial period miscalculation:** "28 days" trial in fine print but consumer is charged after 27 days due to 24-hour cancellation requirement
- **Cancellation that doesn't cancel:** Company confirms cancellation by email but continues charging

### 4.4 Quiz Funnel Compliance Requirements

If you run a quiz-based conversion funnel, to comply with ROSCA and FTC Act § 5:

1. **Subscription terms disclosed on quiz landing page** — before user begins quiz (or at minimum, before collecting billing info)
2. **Quiz results must be accurate** — if results are the same regardless of answers, this is deceptive misrepresentation
3. **Delivered content must match promised content** — "personalized plan" must actually be personalized
4. **Terms must appear before the payment CTA** — not hidden below it; not only in linked Policy
5. **Payment form must disclose recurring nature** — the checkout modal/page must include subscription terms
6. **No countdown timers that reset or are fake** — FTC Act § 5(a) prohibits false urgency
7. **Upsell screens must have confirmation step** — no single-click charges on post-purchase screens
8. **Cancellation mechanism must exist and work** — online, self-service, same channel as signup

---

## 5. Common Enterprise Doctrine

When a group of companies operates as a **single enterprise** to defraud consumers, the FTC can:
- Sue all entities as a joint enterprise
- Hold all individual defendants jointly and severally liable
- Seek disgorgement of total enterprise revenue

**Triggers for common enterprise finding:**
- Shared officers, directors, or employees across entities
- Same operational address or infrastructure
- Commingled funds or cross-entity transfers
- Entities operate different "products" but use same funnel mechanics, same payment processors, same customer service
- One entity appears to be "parent" with control over all

**Genesis Tech example:** 15 corporate defendants (Cyprus + Delaware entities) all operating under common control of 2 founders (Vladimir Mnogoletny and Vasili Ulianov), through intermediary Stamatis Skianis. All entities subject to joint and several liability.

**Practical risk:** If you run multiple subscription products through shell companies to dilute liability, the FTC will pierce the corporate structure and aggregate all revenue for calculating penalties and disgorgement.

---

## 6. Asset Freeze and TRO Risk

### 6.1 When the FTC Seeks an Asset Freeze

The FTC routinely obtains **ex parte Temporary Restraining Orders (TROs) with asset freezes** in subscription fraud cases. An asset freeze is sought when:
- Defendants are likely to dissipate or transfer assets before trial
- Offshore or foreign corporate structure creates risk of asset flight
- Revenue is being rapidly transferred abroad
- Evidence of ongoing fraud with current victims

### 6.2 What an Asset Freeze Does

- **Blocks all transfers, sales, or disposal** of defendant assets (bank accounts, cryptocurrency, real estate, business assets)
- **Applies to third parties** (banks, payment processors) who must hold all funds and report to the court
- **Foreign asset repatriation:** Defendants must return all assets held abroad to US jurisdiction within 5 days (Genesis Tech TRO)
- **Preservation of records:** All business records, electronic data, communications must be preserved immediately
- **Reporting obligation:** Defendants must file a complete accounting of all assets within 3 days

### 6.3 Practical Trigger Thresholds

An ex parte TRO is available (no prior notice to defendant required) when:
- Advance notice would enable defendants to dissipate assets
- There is a risk of immediate irreparable harm
- Evidence of ongoing deceptive practices is strong

**In Genesis Tech:** TRO signed June 4, 2026, the same day the complaint was filed. Defendants had no warning.

### 6.4 Individual Liability for Officers and Directors

The FTC can hold individual founders, CEOs, and officers personally liable when they:
- Participated in or had authority to control the deceptive practices
- Had actual or constructive knowledge of the deception
- Benefited financially from the scheme

This means the asset freeze can cover **personal bank accounts and personal assets** of founders and executives.

---

## 7. Key FTC Enforcement Cases and Penalty Amounts

| Case | Year | Amount | Core Issue |
|---|---|---|---|
| **FTC v. Amazon (Prime)** | 2023-2025 | **$2.5B** (estimated) | Iliad flow for enrollment; Odysseus flow for cancellation — deliberate multi-step obstruction |
| **FTC v. Epic Games** | 2022-2023 | **$520M** ($275M refund + $245M privacy) | Unintended purchases; children's data dark patterns |
| **FTC v. Vonage** | 2022 | **$100M** | Required phone call to cancel; intentional hold times |
| **FTC v. Publishers Clearing House** | 2023 | **$18.5M** | Deceptive design → recurring charges without disclosure |
| **FTC v. JustAnswer** | 2024 | **$7.7M** | Buried subscription terms; trial-to-paid with inadequate disclosure |
| **FTC v. Uber One** | 2024 | Consent order | Deceptive pre-selection; confusing cancellation |
| **FTC v. ABCmouse (Age of Learning)** | 2020 | **$10M** | Hard cancellation process; auto-renewal not clearly disclosed |
| **FTC v. MOBE Ltd.** | 2018 | **$900M** | Deceptive income claims in online education |
| **FTC v. GM UniverseApps / Genesis Tech** | 2026 | Pending | Quiz funnel deception; ROSCA violations; ~$106M US consumer harm across 8 products |

---

## 8. Visa/Mastercard Scheme Requirements for Subscription Merchants

These are card network rules — not laws — but non-compliance triggers **scheme fines that are passed through to the merchant via the acquirer.** They apply to any merchant accepting card payments for subscriptions.

### 8.1 Legal Basis

| Card Network | Rule Reference | Rule Title |
|---|---|---|
| **Mastercard** | Rule 5.4.2 | Negative Option Billing Merchants |
| **Visa** | Rule 5.8.16.2 | Negative Option Transaction Requirements |

### 8.2 Website Requirements

Before a consumer can be charged, the merchant website must display:
- **Physical/mailing address** of the merchant
- **Support email address OR support phone number**
- **Merchant location:** city and country (minimum)

### 8.3 Pre-Payment Disclosure Requirements

Must be displayed **before** the consumer enters payment information:

- **Subscription price** (recurring amount)
- **Billing frequency** (monthly, weekly, etc.)
- **Last 4 digits of the card** to be charged (on recurring charge screen)
- **How to cancel** (specific instructions or link)

**Required disclaimer template** (must appear directly under the payment/CTA button):

> "By clicking [button name], you agree that [MERCHANT NAME] will charge your [card type] ending in [XXXX] [amount] per [period] starting [date] until you cancel. Cancel anytime through [cancellation method/link]."

### 8.4 Transaction Receipt Requirements

After every charge — **including failed/declined attempts** — a receipt must be sent immediately. The receipt must include:
- Trial terms (if in trial period)
- Auto-renewal disclosure
- Next charge amount and date
- Cancellation link or instructions

### 8.5 Cancellation Mechanism Requirements

- **Easy online cancellation** must be available (link or button in account)
- Cancellation via email is acceptable **only if** cancellation instructions are clearly visible before enrollment
- No requirement for phone call to cancel
- Cancellation must be processed without undue delay

### 8.6 Negative Option Specific Requirements

For trial-to-paid conversions:
- **Full disclosure at signup:** Complete trial terms before enrollment
- **Click-to-accept:** Consumer must actively accept negative option terms (no pre-checked boxes)
- **Reminder notification:** Consumer must receive a reminder **3–7 days before trial period ends**, informing them of upcoming charge amount and how to cancel

### 8.7 Non-Compliance Fines

| Card Network | Initial Fine | Escalation |
|---|---|---|
| **Visa** | **$1,000 per month** | Escalates to **$50,000+ per month** for repeat violations |
| **Mastercard** | **$20,000** per violation | Escalates to **$100,000+** for continued non-compliance |

Fines are assessed by the card network against the **acquirer (acquiring bank)**, who passes them to the merchant. Acquirers may terminate the merchant relationship rather than absorb repeated fines.

---

## 9. ROSCA Compliance Checklist for Subscription Products

### 9.1 Pre-Enrollment

- [ ] Subscription terms disclosed BEFORE collecting billing information
- [ ] Disclosure is "clearly and conspicuous" (8-part test — see Section 2)
- [ ] Terms not contradicted by other page content (no "personalized plan" framing if plan is generic)
- [ ] Trial period, conversion date, and recurring price explicitly stated
- [ ] Terms displayed on every device/screen size (not hidden below fold)

### 9.2 At Enrollment

- [ ] Express affirmative consent to subscription terms (checkbox not pre-selected)
- [ ] Consent separate from general T&C acceptance
- [ ] Payment form includes subscription disclosure (not just total amount)
- [ ] Confirmation email/receipt includes trial terms + cancellation instructions

### 9.3 Quiz Funnels Specifically

- [ ] Quiz results are accurate and not predetermined
- [ ] Delivered content actually matches quiz answers
- [ ] No fake countdown timers (timer resets = FTC violation)
- [ ] No spin wheels that consistently land on "biggest discount"
- [ ] Upsell screens have explicit confirmation step before charging
- [ ] Post-purchase "add to program" buttons do not charge without separate consent

### 9.4 Recurring Billing

- [ ] Consumer receives receipt for EVERY charge (including failed attempts)
- [ ] Receipt includes next charge date and amount
- [ ] Reminder sent 3–7 days before trial ends (Visa/Mastercard requirement)
- [ ] Billing descriptor on card statement is recognizable (brand name, not corporate entity)
- [ ] Double-billing prevention: system cannot bill same consumer twice in same period

### 9.5 Cancellation

- [ ] Self-service online cancellation available (no phone call required)
- [ ] Cancellation accessible from same channel used to enroll
- [ ] Cancellation completes within same session (no 5+ step processes)
- [ ] Cancellation actually stops billing (billing does not continue after confirmed cancellation)
- [ ] No ignoring cancellation requests or requiring justification to cancel

### 9.6 Corporate Structure

- [ ] Each subscription product legally compliant on its own merits
- [ ] Multiple products under related entities → FTC can use common enterprise doctrine for joint liability
- [ ] Shell companies do not isolate liability if same operators control all entities
- [ ] Individual founders/executives personally liable for their involvement in deceptive practices

---

## 10. Penalties Summary

| Violation | Penalty |
|---|---|
| FTC Act § 5(a) — deceptive practice | Up to $53,088 per violation (2025) |
| ROSCA violation (= FTC Act rule violation) | Up to $53,088 per violation + monetary relief/disgorgement |
| Visa non-compliance (subscription rules) | $1,000/month → $50,000+/month |
| Mastercard non-compliance (Rule 5.4.2) | $20,000 → $100,000+ |
| Asset freeze (TRO) | All assets frozen pending litigation |
| Individual liability for founders/CEOs | Personal assets included in freeze and judgment |

---

## Related References

- `references/international/dark-patterns.md` — general dark pattern framework across all jurisdictions; FTC enforcement cases summary
- `references/international/non-obvious-traps.md` — Section 1 (Free Trial to Paid Conversion); Section 4 (Testimonials and Income Claims)
- `references/international/platform-compliance.md` — Stripe, Google Ads, paid social requirements
