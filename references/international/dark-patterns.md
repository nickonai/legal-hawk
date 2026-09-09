# Dark Patterns: Legal Framework Across Jurisdictions

> **Last updated:** 2026-03-30
> **Scope:** SaaS products operating internationally
> **Risk level:** HIGH -- enforcement is accelerating globally; fines are substantial

---

## 1. Definition and Classification

### 1.1 What Constitutes a Dark Pattern

A "dark pattern" (also called a "deceptive design pattern") is a user interface design choice that manipulates users into taking actions they did not intend, or that are against their interests. The term was coined by UX researcher Harry Brignull in 2010. Regulators worldwide now treat dark patterns as a form of unfair or deceptive commercial practice.

**Core characteristic:** The interface exploits cognitive biases, creates friction asymmetry, or obscures material information to steer user behavior toward outcomes that benefit the business at the user's expense.

### 1.2 Taxonomy of Dark Patterns

| Pattern | Description | Typical SaaS Implementation |
|---|---|---|
| **Forced Continuity** | Free trial converts to paid subscription with no clear warning or easy opt-out. | Trial asks for credit card upfront; charge begins silently after trial expires with no reminder email. |
| **Roach Motel** | Easy to sign up, extremely difficult to cancel. | One-click signup but cancellation requires calling a phone line, navigating 8+ screens, or sending a physical letter. |
| **Hidden Costs** | Charges not disclosed until the final step of checkout. | Service fees, taxes, or mandatory add-ons revealed only at payment confirmation. |
| **Confirmshaming** | Uses emotionally manipulative language to guilt users into accepting. | "No thanks, I don't want to save money" or "I prefer to stay uninformed" as the decline option. |
| **Trick Questions** | Confusing phrasing designed to make users select unintended options. | Double negatives in opt-out checkboxes: "Uncheck this box if you prefer not to not receive emails." |
| **Disguised Ads** | Advertisements styled to look like native content or navigation elements. | "Download" buttons that are actually ads; sponsored results without clear labeling. |
| **Bait and Switch** | User intends one action but a different, undesirable action occurs. | Clicking "Close" on a popup actually subscribes the user to a mailing list. |
| **Sneak into Basket** | Additional items or services added to the cart without explicit user action. | Pre-selected add-on insurance, premium support, or extended warranty at checkout. |
| **Privacy Zuckering** | Default settings maximize data sharing; privacy-protective options are buried or confusing. | All data-sharing toggles default to ON; the "Accept All" cookies button is prominent while "Manage Preferences" is a small text link. |
| **False Urgency** | Countdown timers, limited-stock warnings, or other artificial scarcity cues. | "Only 2 seats left at this price!" when inventory is not actually limited. |
| **Obstruction** | Making a desired action (unsubscribe, delete account, downgrade) unreasonably difficult. | Requiring users to navigate through retention offers, wait on hold, or complete surveys before cancellation is processed. |
| **Nagging** | Repeated interruptions pushing the user toward a specific action. | Persistent upgrade modals, repeated permission requests, or dismiss-and-reappear banners. |

### 1.3 Legal vs. Illegal Aggressive Marketing -- Where Is the Line?

The line between aggressive-but-legal marketing and an illegal dark pattern depends on jurisdiction, but common principles apply:

**Generally legal (with caveats):**
- Prominent upsell offers during checkout that are clearly labeled and not pre-selected
- Retention flows that present a counter-offer before confirming cancellation (if cancellation remains easily reachable)
- Email reminders about expiring trials (provided the original consent was valid)
- A/B testing of button colors, copy, and layouts for conversion optimization

**Generally illegal across most jurisdictions:**
- Pre-checked boxes that add paid services without explicit consent
- Cancellation processes that are materially harder than the signup process
- Hiding mandatory fees until after the user has committed to purchase
- Using interface design to make the privacy-invasive option visually dominant while obscuring the protective option
- Failing to send pre-renewal notices for auto-renewing subscriptions
- Countdown timers tied to no real deadline

**Gray zone (varies by jurisdiction):**
- Confirmshaming language (explicitly banned in some EU guidance; not directly addressed in US federal law)
- Default opt-in for marketing emails (illegal in EU/UK under GDPR/PECR; legal in US under CAN-SPAM if unsubscribe is provided)
- Retention flows with multiple steps (legal if cancellation is ultimately simple; illegal if designed to exhaust the user into abandoning)

---

## 2. European Union -- Digital Services Act (DSA) Article 25

### 2.1 Legal Basis

**Regulation (EU) 2022/2065** -- the Digital Services Act -- entered into force on 16 November 2022. Article 25 applies to all "providers of online platforms" and has been fully applicable since **17 February 2024**.

### 2.2 Article 25 -- Prohibition of Dark Patterns

Article 25(1) provides:

> Online platforms shall not design, organise or operate their online interfaces in a way that deceives or manipulates the recipients of their service or in a way that otherwise materially distorts or impairs the ability of the recipients of their service to make free and informed decisions.

Article 25(2) clarifies that the prohibition does not apply to practices already covered by the Unfair Commercial Practices Directive (2005/29/EC) or the GDPR.

Article 25(3) mandates that the European Commission may issue guidelines on the application of Article 25.

### 2.3 What Is Prohibited

The DSA, together with European Data Protection Board (EDPB) Guidelines 3/2022 on Dark Patterns in Social Media Platform Interfaces (adopted 14 February 2023), identifies these prohibited categories:

1. **Overloading** -- Presenting too many choices, requests, or options to nudge users toward sharing more data
2. **Skipping** -- Defaulting to the least privacy-friendly settings; pre-selecting consent
3. **Stirring** -- Emotional manipulation (confirmshaming) or visual nudging (bright accept button vs. gray reject)
4. **Hindering** -- Making it difficult to find information or controls (e.g., privacy settings buried 5+ clicks deep)
5. **Fickle** -- Inconsistent or unstable interface design that confuses users about the effect of their actions
6. **Left in the Dark** -- Hiding information, using ambiguous language, or providing incomplete disclosures

### 2.4 Enforcement and Penalties

- **Fines:** Up to **6% of the provider's global annual turnover** for systematic violations of Article 25 (DSA Article 52(3))
- **Periodic penalty payments:** Up to 5% of average daily global turnover per day for continued non-compliance (Article 52(4))
- **Digital Services Coordinators (DSCs):** Each EU Member State designates a DSC responsible for supervising compliance and issuing orders
- **European Commission:** Has direct enforcement power over Very Large Online Platforms (VLOPs, 45M+ monthly active users in the EU) and Very Large Online Search Engines (VLOSEs)

### 2.5 Enforcement Actions (as of March 2026)

- The Commission opened formal proceedings against several VLOPs in 2024-2025 for suspected Article 25 violations related to subscription cancellation flows and cookie consent banners
- Multiple national DSCs have issued compliance orders requiring redesign of checkout flows with pre-selected add-ons

### 2.6 EU Unfair Commercial Practices Directive (UCPD) 2005/29/EC

The UCPD already prohibits "aggressive commercial practices" (Articles 8-9) and "misleading actions" (Articles 6-7). Dark patterns frequently violate:

- **Article 6(1)(d):** Misleading information about price or manner in which price is calculated
- **Article 7(1):** Omission of material information (hidden costs)
- **Article 7(4):** Failure to identify commercial intent
- **Article 9:** Use of harassment, coercion, or undue influence

The UCPD Guidance (updated 2021) explicitly addresses dark patterns, including fake countdown timers, hidden charges, and obstacles to cancellation.

### 2.7 EU Digital Fairness Act (Proposed)

The European Commission announced a proposed Digital Fairness Act as part of its 2024 work programme. Key anticipated provisions:

- Extended dark pattern prohibitions beyond platforms to all online traders
- Specific rules on addictive design patterns
- Strengthened right to cancel digital subscriptions
- Harmonized cancellation button requirements across Member States
- Enhanced enforcement powers for consumer authorities

As of March 2026, the proposal is in the legislative process. SaaS operators should monitor this closely as it would significantly broaden the scope of dark pattern regulation.

### 2.8 GDPR Intersection

Under GDPR Article 7(4) and Recital 42-43, consent obtained through dark patterns is **not valid consent**. The EDPB has confirmed that:

- Pre-ticked boxes do not constitute valid consent (also confirmed by CJEU in *Planet49*, Case C-673/17)
- Cookie walls that force acceptance of all cookies without a genuine alternative are generally non-compliant
- Consent must be as easy to withdraw as to give (Article 7(3))
- Asymmetric design (prominent "Accept All" vs. hidden "Reject All") undermines freely given consent

**Fine exposure:** Up to 4% of global annual turnover or EUR 20 million (whichever is greater) under GDPR Article 83(5).

---

## 3. United States -- FTC Enforcement and State Laws

### 3.1 Federal Framework

The US has no single comprehensive dark patterns statute. Instead, enforcement relies on:

1. **FTC Act, Section 5** -- Prohibition on "unfair or deceptive acts or practices"
2. **Restore Online Shoppers' Confidence Act (ROSCA)** -- 15 U.S.C. Sec. 8401-8405
3. **FTC Negative Option Rule** -- 16 CFR Part 425 (amended)
4. **State laws** (California, Colorado, Connecticut, and others)

### 3.2 FTC Click-to-Cancel Rule -- Timeline and Current Status

| Date | Event |
|---|---|
| **October 2024** | FTC finalizes the Click-to-Cancel Rule amending the Negative Option Rule (16 CFR Part 425) |
| **January 2025** | Most provisions take effect |
| **April 2025** | Click-to-cancel mechanism provisions take effect |
| **July 2025** | Rule **vacated** by federal court (National Advertisers v. FTC); court found FTC exceeded authority under current commission structure |
| **January 2026** | FTC issues Advanced Notice of Proposed Rulemaking (ANPRM) signaling intent to re-propose similar requirements through a revised process |

**Key provisions of the (vacated) rule that signal FTC enforcement priorities:**
- Sellers must make cancellation at least as easy as enrollment ("click-to-cancel")
- Annual reminders required before each renewal for plans with automatic renewal
- Clear and conspicuous disclosure of all material terms before charging
- Express informed consent required, documented by the seller
- Prohibition on requiring consumers to listen to save offers before cancelling (unless the consumer affirmatively opts in)

**Current practical impact:** Despite the vacature, the FTC continues enforcing dark pattern prohibitions under Section 5 of the FTC Act and ROSCA. The vacated rule serves as a strong signal of enforcement expectations.

### 3.3 ROSCA Requirements (15 U.S.C. Sec. 8401-8405)

ROSCA applies to any internet-based negative option marketing (including free-to-paid trials and auto-renewals). Requirements:

1. **Clear and conspicuous disclosure** of all material terms of the transaction before obtaining billing information
2. **Express informed consent** -- affirmative action by the consumer (not pre-checked boxes)
3. **Simple cancellation mechanism** -- the mechanism must be at least as easy to use as the signup mechanism

**Penalties:** Violations treated as unfair or deceptive acts under the FTC Act. Civil penalties up to **$53,088 per violation** (adjusted annually for inflation; 2025 figure).

### 3.4 Key FTC Enforcement Cases

| Case | Year | Amount | Dark Pattern at Issue |
|---|---|---|---|
| **FTC v. Amazon.com (Prime)** | 2023-2025 | **$2.5 billion** (estimated total including restitution and penalties) | Enrollment in Prime through manipulative UI ("Iliad" flow); cancellation process designed to be confusing and multi-step ("Odysseus" flow) |
| **FTC v. Epic Games (Fortnite)** | 2022-2023 | **$520 million** ($275M refund + $245M privacy penalty) | Tricking players (including children) into unintended purchases through confusing button placement and lack of purchase confirmation |
| **FTC v. ABCmouse (Age of Learning)** | 2020 | **$10 million** | Difficult cancellation process; failure to clearly disclose auto-renewal |
| **FTC v. Uber** | 2024 | Consent order + restitution | Subscription (Uber One) enrollment through deceptive pre-selection and confusing cancellation |
| **FTC v. JustAnswer** | 2024 | **$7.7 million** | Buried subscription terms; trial-to-paid conversion with inadequate disclosure |
| **FTC v. Publishers Clearing House** | 2023 | **$18.5 million** | Deceptive design tricking consumers into recurring charges |
| **FTC v. Vonage** | 2022 | **$100 million** | Cancellation process requiring phone call with intentionally long hold times; hidden early termination fees |

### 3.5 FTC "Bringing Dark Patterns to Light" Report (September 2022)

The FTC published a staff report identifying four categories of concern:

1. **Misleading consumers and obscuring material information** (hidden costs, drip pricing)
2. **Making it difficult to cancel subscriptions or charges** (roach motel)
3. **Burying key terms in dense disclosures** (clickwrap with material terms not highlighted)
4. **Tricking consumers into sharing data** (privacy zuckering)

### 3.6 California -- Automatic Renewal Law (ARL)

**California Business & Professions Code Sections 17600-17606** -- one of the strongest state-level protections.

**Key requirements (as amended July 2025):**

1. **Clear and conspicuous disclosure** of automatic renewal terms, including:
   - That the subscription will continue until cancelled
   - The cancellation policy and procedure
   - The recurring charge amount and frequency
   - The length of any trial or promotional period

2. **Affirmative consent:** Consumer must affirmatively consent to the agreement; consent must be documented

3. **Acknowledgment:** Seller must provide an acknowledgment (email, text, or other recordable format) that includes:
   - The automatic renewal terms
   - The cancellation policy
   - Information on how to cancel

4. **Online cancellation mechanism:** Must provide a "prominently located direct link or button" to cancel online if the consumer signed up online. Toll-free telephone number must also be provided

5. **Free gift/trial requirements:** If a trial requires payment information:
   - Must explain how to cancel and the date by which cancellation must occur to avoid charges
   - Must obtain affirmative consent before charging
   - Must send a reminder notification 3-21 days before the trial ends

6. **Amendments effective July 2025:**
   - Strengthened requirements for the cancellation mechanism to be "immediately accessible" without requiring login
   - Clarified that cancellation must be completed within the same session and medium (online cancellation for online signup)
   - Increased scrutiny on "save" offers during cancellation (must not obstruct)

**Penalties:** Up to **$2,500 per violation** under the UCL (California Business & Professions Code Sec. 17206). Can also give rise to private right of action and class actions.

### 3.7 California Consumer Privacy Act / CPRA

**California Civil Code Section 1798.140(h):**

> "Consent" means any freely given, specific, informed and unambiguous indication of the consumer's wishes... Agreement obtained through use of dark patterns does not constitute consent.

**Section 1798.140(l):**

> "Dark pattern" means a user interface designed or manipulated with the substantial effect of subverting or impairing user autonomy, decisionmaking, or choice, as further defined by regulation.

**Practical impact:** If a SaaS product obtains consent to sell/share personal information or to process sensitive personal information via a dark pattern, that consent is **legally void**. The business is treated as having **no consent** and faces CPRA enforcement exposure.

**CPRA penalty:** Up to **$7,500 per intentional violation** involving consumers under 16; **$2,500 per unintentional violation**.

### 3.8 Other US State Laws Addressing Dark Patterns

| State | Law | Dark Pattern Provision |
|---|---|---|
| Colorado | Colorado Privacy Act (CPA) | Consent obtained through dark patterns is not valid consent |
| Connecticut | Connecticut Data Privacy Act (CTDPA) | Same -- dark-pattern consent is void |
| Texas | Texas Data Privacy and Security Act (TDPSA) | Defines dark patterns; consent via dark patterns invalid |
| Oregon | Oregon Consumer Privacy Act | Consent via dark patterns not valid |
| Montana | Montana Consumer Data Privacy Act | Same approach |
| Indiana | Indiana Consumer Data Protection Act | Dark pattern consent void |
| Iowa | Iowa Consumer Data Protection Act | Dark pattern consent void |
| Delaware | Delaware Personal Data Privacy Act | Dark pattern consent void |
| New Hampshire | New Hampshire Privacy Act | Dark pattern consent void |
| New Jersey | New Jersey Data Privacy Act | Dark pattern consent void |
| Maryland | Maryland Online Data Privacy Act (MODPA) (2024) | Consent via dark patterns not valid; additional children's protections |

---

## 4. United Kingdom -- DMCCA 2024

### 4.1 Digital Markets, Competition and Consumers Act 2024 (DMCCA)

The DMCCA received Royal Assent on **24 May 2024**. It introduces a new Subscription Contract Regime under Part 4, Chapter 2.

### 4.2 Subscription Contract Regime (Expected Autumn 2026)

The subscription provisions are expected to come into force via secondary legislation in **Autumn 2026**. Key requirements:

**Pre-contract information (Section 251):**
- All material terms must be presented **together** and not via hyperlink to a separate page
- Must include: full price, billing frequency, minimum commitment period, cancellation rights and process, trial terms
- Information must be provided in a "durable medium" (email, in-app message that can be saved)

**Reminder notices (Section 253):**
- Reminder notice required **before each renewal** (for contracts that auto-renew)
- Must be sent between 3 and 5 days before the renewal date for monthly+ periods
- Must include: date of renewal, amount to be charged, how to cancel, and a direct link or mechanism to cancel

**Cooling-off period (Section 254):**
- 14-day cooling-off period for new subscription contracts
- Applies to each renewal if the consumer was not sent a compliant reminder notice

**Cancellation rights (Section 257):**
- Consumer must be able to cancel through the same channel used to subscribe (or an equally accessible channel)
- Cancellation must be possible with "a single communication" -- no multi-step retention flows
- Cancellation takes effect at the end of the current billing period

### 4.3 CMA Enforcement Powers

The Competition and Markets Authority (CMA) gains enhanced direct enforcement powers under the DMCCA:

- **Fines:** Up to **10% of global annual turnover** for infringements
- **Enhanced consumer measures:** CMA can require businesses to pay compensation directly to affected consumers
- **Redress orders:** CMA can order the business to **contact all affected consumers** to inform them of the breach and their rights
- **Undertakings:** CMA can accept binding commitments from businesses

### 4.4 Existing UK Law (Pre-DMCCA)

Even before the DMCCA subscription regime takes effect, dark patterns are addressable under:

- **Consumer Protection from Unfair Trading Regulations 2008 (CPRs)** -- SI 2008/1277
  - Regulation 5: Misleading actions
  - Regulation 6: Misleading omissions
  - Regulation 7: Aggressive commercial practices
  - Schedule 1: Practices which are always unfair (blacklist), including:
    - Para 7: Creating false impression that consumer cannot leave premises (analogous to roach motel)
    - Para 11: Using editorial content to promote a product without clear labeling (disguised ads)
    - Para 20: Describing a product as "free" when it is not

- **Consumer Rights Act 2015, Part 2** -- Unfair terms in consumer contracts. A term creating significant imbalance to the detriment of the consumer may be deemed unfair and unenforceable.

- **Consumer Contracts (Information, Cancellation and Additional Charges) Regulations 2013** -- SI 2013/3134
  - Regulation 10: Pre-contract information for distance contracts
  - Regulation 13: Pre-ticked boxes prohibition -- "The trader must not use default options which the consumer is required to reject in order to avoid additional payments"
  - Regulation 29: Right to cancel within 14 days for distance contracts

### 4.5 ICO (Data Protection) Position on Dark Patterns

The UK Information Commissioner's Office (ICO) has issued guidance on "deceptive design patterns" in the context of:

- **Children's Code (Age Appropriate Design Code)** -- Standard 3 prohibits nudge techniques that lead children to provide unnecessary personal data or weaken privacy protections
- **Cookie consent:** ICO enforcement actions against cookie banners that make "Reject All" harder than "Accept All"

---

## 5. Russia -- Dark Patterns in Consumer Protection Context

### 5.1 Regulatory Framework

Russia does not have a dedicated "dark patterns" law. However, dark patterns are caught by the intersection of several statutes:

1. **Federal Law No. 2300-1 "On Protection of Consumer Rights" (ZoZPP)** dated 07.02.1992 (as amended)
2. **Federal Law No. 376-FZ** dated 28.11.2025 "On Amending Certain Legislative Acts" (subscription protections, effective **March 2026**)
3. **Code of Administrative Offenses (KoAP RF)**
4. **Civil Code of the Russian Federation**

### 5.2 ZoZPP Article 16 -- Prohibition on Imposing Services

**Article 16(2) ZoZPP** prohibits conditioning the sale of one good or service on the mandatory purchase of another (tying). This directly addresses **sneak-into-basket** patterns.

**Article 16(3)** (as amended by 376-FZ) provides that the consumer's silence or inaction cannot be treated as consent to additional services or charges. This targets **pre-checked boxes** and **forced continuity**.

Key protections:
- Seller cannot condition purchase on acceptance of additional paid services
- Consumer must give **express separate consent** to each additional service
- Pre-checked boxes for additional services are non-compliant
- Services imposed without proper consent must be refunded in full

### 5.3 Federal Law 376-FZ -- Subscription Protections (March 2026)

376-FZ amends the ZoZPP and the Law on Information to add specific subscription-related requirements:

- **Clear disclosure** of subscription terms before enrollment, including price, billing period, and auto-renewal terms
- **Express consent** required for auto-renewal; a standalone consent mechanism separate from general T&C acceptance
- **Pre-renewal notification** required at least 3 days before each renewal charge
- **Simplified cancellation:** Consumer must be able to cancel through the same channel used to subscribe
- **Aggregator liability:** Digital platforms (app stores, marketplaces) bear subsidiary liability for non-compliant merchants

### 5.4 KoAP Penalties

| Article | Offense | Fine (Rubles) |
|---|---|---|
| **14.8** | Violating consumer's right to information about goods/services | 20,000 - 50,000 (legal entities) |
| **14.43** | Violation of requirements for sale of goods/services through the internet | 300,000 - 1,000,000 (legal entities); repeat violations up to 3,000,000 |
| **14.7(1)** | Misleading consumers | 100,000 - 500,000 (legal entities) |

### 5.5 Civil Code Provisions

- **Article 10 GK RF:** Prohibition on abuse of rights, including exercising rights solely to cause harm (can apply to deliberately obstructive cancellation flows)
- **Article 179 GK RF:** Transactions made under the influence of deception can be voided
- **Article 434.1 GK RF:** Pre-contractual liability for negotiating in bad faith (applicable to bait-and-switch)

### 5.6 Rospotrebnadzor Enforcement

Rospotrebnadzor (Federal Service for Consumer Rights Protection) actively monitors online services and has issued warnings and fines to major platforms for:

- Hidden auto-renewal charges
- Inability to cancel subscriptions online
- Bundled services without separate consent
- Inadequate disclosure of subscription terms

---

## 6. United Arab Emirates

### 6.1 General Framework

The UAE does not have legislation explicitly targeting "dark patterns" by name. However, several legal instruments provide coverage:

### 6.2 Federal Decree-Law No. 15/2020 on Consumer Protection

- **Article 4:** Prohibits misleading consumers regarding the nature, quality, quantity, or price of goods and services
- **Article 5:** Requires clear and accurate disclosure of all terms and conditions
- **Article 8:** Prohibits fraudulent commercial practices
- **Article 9:** Consumer's right to return goods purchased through distance selling within specified period
- **Penalties:** Fines of AED 10,000 to AED 2,000,000; repeat offenders may face business closure

### 6.3 Central Bank Law and Financial Services

The **Central Bank of the UAE Regulations (2025)** impose transparency mandates on financial services products:

- Clear disclosure of all fees, charges, and recurring payments
- Prohibition on hidden charges in financial products
- Consumer must receive a complete fee schedule before entering into any agreement
- Auto-renewal of financial service subscriptions requires explicit opt-in consent

### 6.4 DIFC and ADGM

The Dubai International Financial Centre (DIFC) and Abu Dhabi Global Market (ADGM) free zones have their own consumer protection frameworks, both emphasizing:

- Fair dealing obligations
- Prohibition on misleading or deceptive conduct
- Requirements for clear and transparent disclosure of material terms

### 6.5 Sanadak Platform

The UAE Ministry of Economy operates the **Sanadak** consumer complaints platform. Consumers can file complaints about:

- Hidden charges and undisclosed fees
- Difficulty cancelling subscriptions
- Misleading pricing or terms
- Unauthorized charges

Businesses operating in the UAE should be aware that Sanadak complaints can trigger Ministry investigations and potential enforcement action.

### 6.6 Telecommunications and Digital Services Authority (TDRA)

TDRA regulations require:

- Clear terms of service for digital services
- Transparent pricing with no hidden fees
- Consumer right to cancel digital subscriptions
- Adequate notification before any price change

### 6.7 Practical Guidance for UAE Operations

- No specific "dark pattern" jurisprudence exists yet
- General consumer protection and fraud provisions provide a backstop
- The regulatory trend is toward stricter transparency requirements
- SaaS products should apply EU/UK-level compliance standards to UAE operations as a safe harbor approach

---

## 7. Audit Checklist: Detecting Dark Patterns on a SaaS Website

Use this checklist to audit any SaaS product for potential dark pattern violations. Each item should be tested from the perspective of a new user, a trial user, and a paying subscriber.

### 7.1 Subscription Enrollment

- [ ] **Pre-checked boxes:** Are there any pre-selected add-ons, premium tiers, or additional services at checkout?
  - **Violation if:** Any box is pre-checked that adds cost or changes the service level
  - **Relevant law:** EU DSA Art. 25; UK Consumer Contracts Reg. 13; ROSCA; California ARL

- [ ] **Hidden costs:** Are all fees (service fees, processing fees, taxes, setup costs) displayed before the user enters payment information?
  - **Violation if:** Any charge appears for the first time at or after payment confirmation
  - **Relevant law:** UCPD Art. 6-7; FTC Act Sec. 5; California ARL Sec. 17602

- [ ] **Trial-to-paid disclosure:** If a free trial requires payment info, is it clearly stated when the trial ends, what the charge will be, and how to cancel?
  - **Violation if:** User is not clearly informed of the exact date charges begin and the exact amount
  - **Relevant law:** ROSCA; California ARL; UK DMCCA Sec. 251; Russia 376-FZ

- [ ] **Consent mechanism:** Is enrollment consent obtained through a clear affirmative action (unchecked checkbox, explicit button click) that is separate from other agreements?
  - **Violation if:** Consent is bundled with T&C acceptance, uses pre-checked boxes, or requires no affirmative action
  - **Relevant law:** GDPR Art. 7; CPRA Sec. 1798.140(h); ROSCA

### 7.2 Auto-Renewal and Billing

- [ ] **Pre-renewal notification:** Does the system send a reminder before each auto-renewal with the charge amount and date?
  - **Violation if:** No reminder is sent, or reminder does not include charge amount and cancellation instructions
  - **Relevant law:** California ARL Sec. 17602(a)(2); UK DMCCA Sec. 253; Russia 376-FZ

- [ ] **Hidden auto-renewal terms:** Are auto-renewal terms clearly and conspicuously disclosed at the point of enrollment (not buried in T&C)?
  - **Violation if:** Auto-renewal terms are only in linked T&C that the user must actively seek out
  - **Relevant law:** UK DMCCA (terms must be presented "together"); ROSCA; California ARL

- [ ] **Forced continuity:** Does the trial convert to paid automatically without a clear, timely warning?
  - **Violation if:** Conversion happens silently or with only a buried email notification
  - **Relevant law:** All jurisdictions; universal enforcement priority

### 7.3 Cancellation Process

- [ ] **Cancellation parity:** Is the cancellation process comparable in ease and medium to the signup process?
  - **Violation if:** Online signup but cancellation requires phone call, email, or physical letter
  - **Relevant law:** FTC Click-to-Cancel (vacated but signals enforcement posture); California ARL; UK DMCCA Sec. 257; Russia 376-FZ; ROSCA

- [ ] **Number of steps:** How many clicks/steps are required to complete cancellation?
  - **Red flag if:** More than 3 steps after the user initiates cancellation
  - **Relevant law:** FTC enforcement precedent (Amazon Prime case); UK DMCCA

- [ ] **Obstructive retention flows:** Are "save" offers or surveys mandatory before cancellation can be completed?
  - **Violation if:** User cannot skip retention offers or must engage with them before reaching the cancel button
  - **Relevant law:** FTC position (save offers must be opt-in, not mandatory); California ARL (2025 amendments)

- [ ] **Confirmshaming on cancellation:** Does the cancellation flow use emotionally manipulative language?
  - **Examples:** "Are you sure? You'll lose all your data forever!" or "No, I want to keep paying full price"
  - **Relevant law:** EU DSA Art. 25; UCPD Art. 8-9; EDPB Guidelines 3/2022

- [ ] **Cancel button visibility:** Is the cancellation option clearly visible in account settings, or is it hidden?
  - **Violation if:** User must search through multiple pages, FAQs, or contact support to find cancellation
  - **Relevant law:** All jurisdictions

### 7.4 Pricing and Checkout

- [ ] **Drip pricing:** Is the total price clear from the beginning, or do additional charges "drip" in during checkout?
  - **Violation if:** Price increases between product selection and payment confirmation due to previously undisclosed fees
  - **Relevant law:** UCPD Art. 6(1)(d); FTC Act Sec. 5; UAE Consumer Protection Art. 4

- [ ] **Sneak into basket:** Are any items, services, or add-ons automatically added to the user's cart?
  - **Violation if:** Cart contains items the user did not explicitly add
  - **Relevant law:** EU DSA Art. 25; UK Consumer Contracts Reg. 13; Russia ZoZPP Art. 16(2)

- [ ] **False urgency:** Are there countdown timers, "limited time" banners, or scarcity indicators?
  - **Violation if:** Timers reset, "limited" offers recur indefinitely, or stock indicators are fabricated
  - **Relevant law:** UCPD Annex I (blacklisted practices); FTC Act Sec. 5

### 7.5 Consent and Privacy

- [ ] **Cookie/consent banners:** Is "Reject All" or "Necessary Only" as easy to click as "Accept All"?
  - **Violation if:** Accept is a prominent button while Reject requires navigating through settings
  - **Relevant law:** GDPR Art. 7; ePrivacy Directive; EDPB Guidelines 3/2022; UK ICO guidance

- [ ] **Default privacy settings:** Do privacy settings default to minimum sharing, or maximum sharing?
  - **Violation if:** All data-sharing toggles default to ON; user must manually turn them OFF
  - **Relevant law:** GDPR Art. 25 (data protection by default); CPRA dark pattern provisions

- [ ] **Trick questions in forms:** Are opt-in/opt-out choices phrased in a clear, straightforward manner?
  - **Violation if:** Double negatives, confusing phrasing, or inconsistent checkbox logic
  - **Relevant law:** EU DSA Art. 25; GDPR (clear and plain language requirement); CPRA

### 7.6 Interface Design

- [ ] **Visual hierarchy manipulation:** Are the options the business prefers given disproportionate visual prominence?
  - **Violation if:** "Accept" is a large bright button while "Decline" is small gray text, or upgrade button is prominent while downgrade is hidden
  - **Relevant law:** EU DSA Art. 25; EDPB Guidelines 3/2022 (stirring)

- [ ] **Disguised ads:** Are advertisements or sponsored content clearly labeled?
  - **Violation if:** Ads look like organic content, navigation, or system messages
  - **Relevant law:** UCPD Annex I; FTC Endorsement Guides; UK CPRs Schedule 1

- [ ] **Bait and switch:** Does clicking a button produce the action the user expects?
  - **Violation if:** "Close" button triggers a subscription; "Skip" button actually accepts
  - **Relevant law:** FTC Act Sec. 5; UCPD Art. 6; all jurisdictions

- [ ] **Nagging patterns:** Are there persistent or recurring popups pushing the user toward a specific action?
  - **Red flag if:** Same upgrade modal appears more than once per session, or dismissal is not persistent
  - **Relevant law:** EU DSA Art. 25 (overloading); general unfair practices

### 7.7 Comprehensive Testing Protocol

1. **Sign up for the lowest-tier plan or free trial** and document every screen, disclosure, and consent mechanism
2. **Attempt to cancel within 24 hours** and count every click, page, and retention offer
3. **Compare visual prominence** of upgrade vs. downgrade, accept vs. reject, subscribe vs. skip
4. **Check all pre-selected options** at checkout -- document any that add cost
5. **Wait for renewal** -- verify that pre-renewal notifications are sent with adequate lead time and complete information
6. **Review privacy settings** -- verify defaults are privacy-protective
7. **Test on mobile** -- dark patterns may differ between desktop and mobile interfaces
8. **Screenshot everything** -- enforcement agencies and courts rely on visual evidence

---

## Cross-Reference: Key Penalty Summary

| Jurisdiction | Maximum Fine | Legal Basis |
|---|---|---|
| **EU (DSA)** | 6% global annual turnover | DSA Art. 52(3) |
| **EU (GDPR)** | 4% global annual turnover or EUR 20M | GDPR Art. 83(5) |
| **US (FTC)** | $53,088 per violation (ROSCA/FTC Act) | 15 U.S.C. Sec. 45, 8401-8405 |
| **US (CPRA)** | $7,500 per intentional violation | Cal. Civ. Code Sec. 1798.155 |
| **US (California ARL)** | $2,500 per violation + private action | Cal. B&P Code Sec. 17206 |
| **UK (DMCCA)** | 10% global annual turnover | DMCCA 2024, Part 4 |
| **Russia (KoAP)** | RUB 300K-3M per violation | KoAP Art. 14.43, 14.8 |
| **UAE** | AED 10K-2M + potential closure | Federal Decree-Law 15/2020 |

---

## Practical Recommendations for SaaS Products

1. **Design for the strictest jurisdiction.** If you operate in the EU, UK, and US, apply EU/UK standards globally. This simplifies compliance and future-proofs against tightening regulations elsewhere.

2. **Cancellation parity is non-negotiable.** Every major jurisdiction is converging on the principle that cancellation must be as easy as signup. Implement a self-service, online, same-session cancellation flow.

3. **Eliminate pre-checked boxes.** No jurisdiction permits them for paid add-ons. Most privacy frameworks (GDPR, CPRA, CPA, CTDPA) invalidate consent obtained through pre-checked boxes.

4. **Send pre-renewal notices.** Even where not yet legally required, pre-renewal notices are rapidly becoming a universal expectation and reduce chargeback and regulatory risk.

5. **Document consent.** Maintain timestamped records of what was disclosed, what the user consented to, and how consent was obtained. This is your defense in any enforcement action.

6. **Audit quarterly.** Dark patterns can be introduced inadvertently through A/B tests, growth experiments, or feature updates. Regular audits using this checklist prevent drift.

7. **Treat confirmshaming as high-risk.** While not explicitly banned everywhere, confirmshaming is increasingly cited in enforcement guidance and is a reputational liability.

8. **Cookie consent must be symmetric.** "Accept All" and "Reject All" must be equally prominent. Burying rejection behind multiple clicks is a well-established violation in both EU and UK enforcement.
