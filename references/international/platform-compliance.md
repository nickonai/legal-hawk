# Platform Compliance: Stripe, Paid Social Ads, Google Ads

## Overview

SaaS businesses depend on payment processors and advertising platforms. Account suspensions from Stripe, social ad platforms, or Google can be existential threats. This reference covers the specific policies, thresholds, and triggers that lead to enforcement actions, with practical prevention strategies.

---

## STRIPE

### Prohibited Businesses

Stripe maintains a prohibited and restricted businesses list. Accounts in prohibited categories will be terminated. Key prohibited categories:

- **Illegal products or services**: Anything illegal in the jurisdiction of operation
- **Certain financial products**: Unregistered securities, binary options, forex (without proper licensing), cryptocurrency (varies by jurisdiction -- some permitted with approval)
- **Adult content and services**: Sexually explicit content (Stripe is stricter than many processors)
- **Gambling**: Online gambling without proper licensing in all relevant jurisdictions
- **Get-rich-quick schemes**: Products or services promising unrealistic income or returns. This includes:
  - "Make $10K/month with no work" type offers
  - Systems or courses promising guaranteed financial outcomes
  - Programs that primarily recruit others for income (see MLM below)
- **Multi-level marketing (MLM)**: MLM and network marketing businesses are restricted or prohibited
- **Counterfeit goods**: Any products infringing on trademarks or intellectual property
- **Weapons and ammunition**: Firearms, ammunition, and certain weapons accessories
- **Drugs and drug paraphernalia**: Including certain supplements making drug-like claims
- **Pseudo-pharmaceuticals**: Products with unsubstantiated health claims

### High-Risk Categories (Not Prohibited But Flagged)

These categories are allowed but face enhanced scrutiny:

- **Education and coaching**: Permitted, but flagged if perceived as "predatory." Triggers include:
  - High-ticket programs ($1,000+) with aggressive refund-averse policies
  - Income or outcome guarantees ("You WILL make $X")
  - Upsell funnels where the primary product is access to more upsells
  - High chargeback rates (see below)
  - Coaching programs that resemble get-rich-quick schemes
- **Subscription services**: Acceptable, but Stripe monitors for dark patterns in billing
- **Digital downloads and software**: Generally fine, but higher chargeback risk
- **Travel**: Advance bookings create chargeback risk due to delivery timing

### Chargeback (Dispute) Thresholds

Chargeback rates are the percentage of transactions that result in a customer dispute. Stripe and the card networks (Visa, Mastercard) enforce escalating thresholds:

| Level | Chargeback Rate | Consequence |
|-------|----------------|-------------|
| **Normal** | < 0.75% | No action |
| **High-Risk** | 0.75% - 0.89% | Warning from Stripe. Enhanced monitoring. You may be asked to provide a remediation plan. |
| **Excessive** | 0.90% - 0.99% | Formal escalation. Stripe may require immediate remediation, hold reserves, or restrict payouts. Visa/Mastercard monitoring programs may activate. |
| **Penalty Zone** | 1.0%+ | Card network fines begin ($50-$100 per chargeback for Visa VDMP, escalating monthly). Stripe may terminate the account. Mastercard's Excessive Chargeback Merchant (ECM) program activates at 1.5%. |

**How chargeback rate is calculated**: Total disputes in a month divided by total transactions in that month. Visa uses the prior month's transactions as the denominator. Even a small number of disputes can push a low-volume merchant over the threshold.

### Required Website Pages for Stripe

Stripe reviews merchant websites during onboarding and periodically. Missing or inadequate pages can trigger account holds or termination:

1. **Refund Policy**: Must be clearly stated and easy to find. Must include:
   - Whether refunds are offered
   - Time window for refund requests
   - Process for requesting a refund
   - Any conditions or exceptions
   - How refunds are processed (original payment method, credit, etc.)
   - Timeline for receiving the refund

2. **Terms of Service / Terms and Conditions**: Must cover:
   - What the customer is purchasing
   - Subscription terms (billing frequency, renewal, cancellation)
   - Limitation of liability
   - Governing law and dispute resolution
   - Acceptable use policy

3. **Contact Information**: Must include at minimum:
   - Email address (a real, monitored email)
   - Ideally also: phone number, physical address, contact form
   - Must be easy to find (footer link on every page, or dedicated contact page)

4. **Clear Pricing**: Before the customer enters payment information, they must see:
   - Exact amount they will be charged
   - Currency
   - Billing frequency (monthly, annual, one-time)
   - Any trial periods and what happens when the trial ends
   - Any setup fees or additional charges

5. **Privacy Policy**: Required by Stripe and by law in most jurisdictions. Must cover:
   - What data is collected
   - How data is used
   - Third-party sharing (including Stripe as payment processor)
   - Data retention
   - User rights (GDPR, CCPA as applicable)

### Subscription-Specific Requirements

Stripe has specific requirements for subscription businesses:

- **Transparent billing**: Customers must know exactly what they will be charged, when, and how often. No hidden fees.
- **Easy cancellation**: Cancellation must be at least as easy as signup. Stripe explicitly monitors for dark patterns:
  - Burying cancellation options deep in settings
  - Requiring phone calls to cancel
  - Making customers jump through multiple confirmation screens designed to prevent cancellation
  - Charging after cancellation request
- **Pre-renewal notifications**: Best practice (and legally required in many jurisdictions) to notify customers before subscription renewal, especially for annual plans.
- **Clear trial-to-paid transitions**: If offering free trials, clearly communicate when the trial ends and what the first charge will be. Send a reminder before the trial converts to paid.

### Dispute Prevention Strategies

1. **Keep dispute rate below 0.75%** at all times. Target < 0.5% for comfort.
2. **Use Ethoca and Verifi alerts**: These are early warning systems from Mastercard (Ethoca) and Visa (Verifi/CDRN) that notify you of disputes before they become formal chargebacks. You can issue a refund proactively to prevent the chargeback from counting against your rate. Stripe integrates with both.
3. **Clear billing descriptors**: Ensure your Stripe billing descriptor (the name that appears on the customer's credit card statement) is recognizable. Use your brand name, not a corporate entity name the customer would not recognize.
4. **Send receipts**: Stripe sends receipts automatically, but ensure they are enabled and include clear descriptions of what was purchased.
5. **Respond to disputes promptly**: Stripe gives you a window to respond to disputes with evidence. Always respond -- even if you expect to lose, responding reduces the impact.
6. **Implement a generous refund policy**: It is far cheaper to issue a refund than to fight a chargeback. A chargeback costs you the transaction amount + a $15 Stripe dispute fee + damage to your chargeback rate.
7. **Monitor your dispute rate weekly**: Use Stripe's Radar and dispute analytics dashboard.

---

## VISA / MASTERCARD SCHEME REQUIREMENTS FOR SUBSCRIPTION MERCHANTS

Card network rules impose specific requirements on merchants using **negative option / subscription billing.** Non-compliance triggers scheme fines passed through by the acquirer.

### Rule References

| Network | Rule | Title |
|---|---|---|
| Mastercard | Rule 5.4.2 | Negative Option Billing Merchants |
| Visa | Rule 5.8.16.2 | Negative Option Transaction Requirements |

### Website Requirements

The merchant website must clearly display (before checkout):
- Physical or mailing address
- Support email address or phone number
- Merchant location (city + country minimum)

### Pre-Payment Disclosure (Required Under Pay Button)

Before the consumer enters payment information, show:
- Subscription price and billing frequency
- How to cancel (specific link or instructions)

**Required disclaimer template directly under the "Pay/Subscribe" button:**
> "By clicking [button], you agree that [MERCHANT NAME] will charge your [card type] ending in [XXXX] [amount] per [period] starting [date] until you cancel. Cancel anytime via [link/method]."

### Transaction Receipt Requirements

After **every charge** — including failed/declined transactions — send a receipt immediately. Receipt must include:
- Trial terms (if applicable)
- Auto-renewal disclosure
- Next charge amount and date
- Cancellation link or instructions

### Cancellation Requirements

- Easy **online** cancellation mechanism required
- Email cancellation acceptable only if cancellation instructions were clearly displayed before enrollment
- No phone-call-only cancellation allowed

### Negative Option / Trial Requirements

For trial-to-paid conversions specifically:
- Full trial terms at point of enrollment (before billing info collected)
- Consumer must **click to accept** negative option terms — no pre-checked boxes
- Send a **reminder notification 3–7 days before the trial period ends** with charge amount and cancellation instructions

### Non-Compliance Fines

| Network | Initial Fine | Escalation |
|---|---|---|
| **Visa** | **$1,000/month** | **$50,000+/month** for continued non-compliance |
| **Mastercard** | **$20,000** per violation | **$100,000+** for repeated violations |

Fines are assessed against the **acquirer** who passes them to the merchant. Acquirers may terminate the merchant relationship rather than absorb escalating fines. See also: `references/us/negative-option-ftc.md` for FTC/ROSCA legal requirements (separate from scheme rules).

---

## PAID SOCIAL ADS (social media advertising platforms)

### Common Account Ban Triggers

Social ad platform account bans are notoriously opaque. The most common triggers:

1. **Repeated policy violations**: Multiple rejected ads accumulate strikes. Platforms use escalating enforcement systems.
2. **Misleading content**: Ads that promise outcomes the product cannot deliver. Common in education/coaching:
   - "Guaranteed results"
   - Unrealistic income claims
   - Before/after claims that are unsubstantiated
3. **Low-quality landing pages**: Landing pages that:
   - Do not match the ad's promises
   - Have excessive pop-ups or redirect chains
   - Lack required disclosures (privacy policy, terms)
   - Have broken functionality or slow load times
   - Use clickbait tactics
4. **Cloaking**: Showing different content to platform reviewers than to actual users. This is one of the most severe violations and results in permanent bans. Platforms use automated and manual detection.
5. **Circumvention**: Creating new ad accounts after a ban, using other people's accounts, or using technical methods to evade enforcement. This escalates to a **business-level ban** affecting all associated accounts.
6. **Engagement bait**: "Tag a friend," "Share to win," etc.
7. **Excessive negative feedback**: When users hide, report, or negatively respond to your ads at high rates.

### Landing Page Requirements

Every ad links to a landing page. The platform reviews landing pages as part of ad approval:

- **Content must match ad promises**: If the ad says "free guide," the landing page must deliver a free guide without requiring payment first.
- **Privacy policy link**: Must be present and accessible on the landing page (especially if collecting email addresses or any personal data).
- **Mobile optimized**: Landing page must function properly on mobile devices. Broken mobile experiences trigger disapproval.
- **No auto-playing audio or video**: Distracting auto-play elements can trigger disapproval.
- **No deceptive design**: Fake countdown timers (that reset), fake "limited availability" claims, fake chat notifications, misleading buttons.
- **Functional**: No 404 errors, no redirect chains, no broken forms.
- **Clear identification**: The business behind the landing page must be identifiable (company name, contact info).

### Prohibited Claims

- **Unrealistic income claims**: "Make $10K in your first month" -- prohibited even as a testimonial unless it represents typical results (which it almost never does).
- **Health cures**: "This supplement cures cancer" -- absolutely prohibited. Even softer health claims face heavy scrutiny.
- **Misleading before/after**: Images or claims showing transformation results that are not representative, unsubstantiated, or manipulated.
- **Personal attributes**: Ads cannot assert or imply things about the user's personal attributes (race, ethnicity, religion, sexual orientation, disability, financial status, criminal record, etc.). Example: "Struggling with debt?" is prohibited. "Debt consolidation services" is permitted.
- **Clickbait and sensationalism**: Withholding information to create curiosity ("You won't believe what happened...").

### Special Ad Categories

**Education** is a Special Ad Category in the US (along with credit, employment, housing, and social issues/politics):

- **Limited targeting**: Cannot target by age, gender, zip code (only 15-mile radius minimum), or detailed demographics.
- **No lookalike audiences**: Must use "Special Ad Audiences" instead of standard lookalike audiences.
- **Must declare the category**: When creating the ad, you must select the Special Ad Category. Failure to do so when required results in ad disapproval or account penalties.
- **Note**: The education special category specifically applies to ads promoting educational programs, institutions, or opportunities. General SaaS products that happen to be used in education may not need the special category designation -- but education-focused marketing (e.g., "Enroll in our course") does.

### Testimonial and Disclaimer Requirements

- **"Results not typical" disclaimers**: Required when featuring customer testimonials that show above-average results. The disclaimer must be clearly visible (not buried in fine print).
- **Income disclaimers**: If showing income results, you must include: "Results not typical. Individual results will vary." Many advertisers add: "See income disclosure at [link]."
- **Endorsement disclosures**: If the person in the testimonial was compensated (even with free product access), this must be disclosed.
- **Substantiation**: You must be able to substantiate any claims in testimonials with documentation.

### Prevention Strategies

1. **Monitor Account Health regularly**: Major social ad platforms provide an account quality dashboard. Check it weekly.
2. **Honest creatives**: Do not exaggerate. If your course helps people get jobs, do not claim it guarantees employment. Show typical outcomes, not best-case scenarios.
3. **Never circumvent**: If an account is banned, appeal through proper channels. Do not create new accounts or use others' accounts. Platforms link accounts through payment methods, IP addresses, device fingerprints, and browser cookies.
4. **Warm up new accounts**: New ad accounts should start with small budgets and non-controversial campaigns. Gradually increase spend.
5. **Appeal promptly**: When ads are disapproved, request a review if you believe the disapproval is incorrect. Be specific about why the ad complies.
6. **Maintain a backup**: Have a secondary verified Business Manager (legitimate, not for circumvention) so one account issue does not eliminate all advertising capability.
7. **Test creatives in small batches**: Before scaling, test new ad creative with small budgets to catch policy issues early.

---

## GOOGLE ADS

### Three-Strikes System

Google Ads uses a three-strikes enforcement system (introduced 2021, refined 2023):

| Strike | Consequence |
|--------|-------------|
| **First strike** | Warning + temporary account hold (ad serving paused). Must acknowledge the policy and fix the violation. |
| **Second strike** | Within 90 days of the first. Account hold for 3 days. All ads paused. |
| **Third strike** | Within 90 days of the first. **Account suspension**. Permanent for the specific violation type. Appeal possible but difficult. |

**Important**: The 90-day window resets after 90 days without a new strike. Strikes are per violation type -- you could have strikes across multiple categories simultaneously.

### Top Suspension Triggers

Based on Google's enforcement data:

1. **Circumventing systems policy (~38% of suspensions)**: This includes:
   - Cloaking (showing different content to Google than to users)
   - Redirecting through multiple domains
   - Attempting to evade review by manipulating ad content
   - Using bridging pages designed primarily to pass review
   - Creating new accounts after suspension

2. **Unacceptable business practices (~38% of suspensions)**: This includes:
   - Misleading users about the nature of the business
   - Collecting user information under false pretenses
   - Coordinated deceptive practices
   - Impersonating other businesses or products

3. **Misrepresentation (significant percentage)**: Ads or landing pages that:
   - Omit relevant information
   - Provide misleading information about products, services, or businesses
   - Use false claims about affiliation with other companies
   - Create false urgency or scarcity

4. **Trademark violations**: Using competitor trademarks in ad text (not keywords -- keyword use is generally permitted, but ad text use is restricted).

### Advertiser Identity Verification (AIV)

- **Mandatory** for all advertisers. Google requires identity verification to run ads.
- **Process**:
  1. Google sends a notification requesting verification
  2. Submit legal business name, government ID or business registration documents, and other identifying information
  3. Google verifies within 30 days (sometimes faster)
  4. Until verified, ads may be limited or paused
- **"About this advertiser" disclosure**: After verification, Google shows a disclosure on your ads (accessible via the three-dot menu) showing your verified name and location. Users can see who is behind any ad.
- **Failure to complete AIV**: Account suspension after the deadline (typically 30 days from notification).

### Education as High-Risk Industry

Google classifies education (especially online education and coaching) as a high-risk industry:

- **Enhanced review**: Education ads face more frequent manual reviews.
- **Legitimacy documentation**: Google may request proof of legitimacy:
  - Business registration
  - Educational accreditation (if applicable)
  - Student outcome data
  - Proof that marketed services actually exist
- **Restricted claims**: Cannot guarantee degrees, certifications, or employment outcomes unless you are an accredited institution.
- **Country-specific restrictions**: Some countries restrict education advertising more heavily (e.g., certain education ads in India require additional verification).

### Misrepresentation Policy

Google's misrepresentation policy is one of the most commonly enforced:

- **Ads must match landing pages exactly**: If the ad promotes "Free CRM Software," the landing page must offer free CRM software -- not a free trial, not a free demo of paid software.
- **No omission of material information**: Prices, fees, subscription terms, and limitations must be clearly stated.
- **Business identity must be accurate**: The business name in the ad must match the business operating the landing page.
- **No impersonation**: Cannot imply affiliation with, or endorsement by, other companies or organizations.
- **No false claims of authority**: Cannot claim certifications, awards, or endorsements that do not exist.
- **Landing page functionality**: Landing page must be functional, load properly, and not use deceptive navigation (e.g., fake back buttons, redirect loops).

### Prevention Strategies

1. **Complete Advertiser Identity Verification immediately** when prompted. Do not delay -- delays risk account limitations.
2. **Audit campaigns monthly**: Review all active ads and landing pages for policy compliance. Check that:
   - All landing pages are functional and load correctly
   - Ad claims match landing page content exactly
   - Pricing is accurate and complete
   - Testimonials include required disclaimers
   - No expired promotions or outdated claims
3. **Use Google's Policy Manager**: Available in the Google Ads interface, it shows current policy issues and violation history.
4. **Avoid automated bulk changes**: Automated tools that change ad text or URLs in bulk can inadvertently create policy violations. Review changes before publishing.
5. **Maintain consistent branding**: Use the same business name across your Google Ads account, landing pages, and verification documents.
6. **Do not create multiple accounts**: Google links accounts and treats multiple accounts from the same business as potential circumvention.
7. **Respond to policy warnings quickly**: When Google flags an issue, fix it within 7 days. Do not wait for the strike.
8. **Keep records**: Document your compliance efforts. If you need to appeal, having records of proactive compliance steps strengthens your case.
9. **Use Performance Max and Smart campaigns carefully**: Automated campaign types may generate ad variations that inadvertently violate policies. Monitor auto-generated assets.

---

## Cross-Platform Compliance Checklist

### Website Requirements (Satisfies All Three Platforms)

- [ ] **Refund policy**: Clear, accessible, fair (Stripe requirement; also helps reduce ad disputes)
- [ ] **Terms of Service**: Comprehensive, covering subscription terms (Stripe requirement)
- [ ] **Privacy policy**: GDPR/CCPA compliant, linked from all pages (all three platforms require)
- [ ] **Contact information**: Email + phone/address visible on every page (Stripe and Google requirement)
- [ ] **Clear pricing**: No hidden fees, transparent billing terms (Stripe and Google requirement)
- [ ] **Mobile optimization**: All pages function on mobile (social platforms and Google requirement)
- [ ] **Consistent branding**: Business name matches across ads, landing pages, payment (Google AIV requirement)

### Advertising Content

- [ ] **No unrealistic claims**: Income claims, health claims, or guaranteed outcomes (all platforms prohibit)
- [ ] **Testimonials have disclaimers**: "Results not typical" clearly visible (ad platforms and FTC requirement)
- [ ] **Ads match landing pages**: 1:1 correspondence between ad promises and landing page content (Google requirement)
- [ ] **Special categories declared**: Education ads declared in the correct special ad category
- [ ] **No cloaking or circumvention**: Same content shown to reviewers and users (all platforms; this is the single most dangerous violation)

### Payment and Billing

- [ ] **Chargeback rate monitored**: Weekly monitoring, target < 0.5%, action plan if approaching 0.75%
- [ ] **Ethoca/Verifi alerts active**: Early dispute detection (Stripe integration)
- [ ] **Clear billing descriptors**: Recognizable business name on statements
- [ ] **Easy cancellation**: One-click or minimal-step cancellation process
- [ ] **Pre-renewal reminders**: Sent before subscription renewals, especially annual

### Account Health Monitoring

- [ ] **Stripe**: Monitor dispute rate in Dashboard > Payments > Disputes weekly
- [ ] **Social ad platforms**: Check the account quality dashboard weekly
- [ ] **Google**: Review Policy Manager in Google Ads interface monthly
- [ ] **Document everything**: Keep records of compliance reviews, remediation actions, and policy acknowledgments
