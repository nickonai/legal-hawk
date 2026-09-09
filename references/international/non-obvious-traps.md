# Non-Obvious Legal Traps for SaaS & Education Platforms

> **Disclaimer:** This document is for informational purposes only and does not constitute legal advice. Laws and regulations change frequently. Always consult qualified legal counsel in the relevant jurisdiction before making compliance decisions.
>
> **Last updated:** 2026-03-30

---

## Table of Contents

1. [Free Trial to Paid Conversion](#1-free-trial-to-paid-conversion)
2. [Web Accessibility Lawsuits](#2-web-accessibility-lawsuits)
3. [COPPA -- Children's Data](#3-coppa--childrens-data)
4. [Testimonials and Income Claims](#4-testimonials-and-income-claims)
5. [EU Geoblocking Regulation](#5-eu-geoblocking-regulation-2018302)
6. [Data Portability (GDPR Art. 20)](#6-data-portability-gdpr-art-20)
7. [Affiliate/Referral Programs](#7-affiliatereferral-programs)
8. [User-Generated Content Liability](#8-user-generated-content-liability)
9. [Currency, Tax, and Pricing](#9-currency-tax-and-pricing)
10. [AI in Education Platforms](#10-ai-in-education-platforms)
11. [PCI DSS v4.0 for Stored Cards](#11-pci-dss-v40-for-stored-cards)
12. [Cooling-Off Periods Summary](#12-cooling-off-periods-summary-table)
13. [Anti-Money Laundering](#13-anti-money-laundering)
14. [Key Compliance Deadlines 2025-2026](#14-key-compliance-deadlines-2025-2026)

---

## 1. Free Trial to Paid Conversion

Free trials that silently convert to paid subscriptions are one of the most heavily regulated areas in consumer protection law. Multiple jurisdictions have enacted specific rules targeting this practice, and enforcement is intensifying.

### EU: Consumer Rights Directive (2011/83/EU)

- **14-day cooling-off period** (Art. 9): Consumers may withdraw from any distance contract within 14 calendar days without giving any reason and without incurring any costs beyond the direct cost of returning goods.
- **Explicit consent to waive withdrawal right** (Art. 16(m)): For digital content supplied on a non-tangible medium, the consumer must give explicit prior consent to begin performance during the withdrawal period AND acknowledge that they thereby lose their right of withdrawal. Both conditions must be met.
- **Pre-contractual information** (Art. 6(1)(h)-(i)): The trader must inform the consumer about the existence of the right of withdrawal, the conditions, the time limit, and procedures for exercising it. If no right of withdrawal exists, the trader must inform the consumer that they will not benefit from it.
- **Confirmation on a durable medium** (Art. 8(7)): The trader must provide confirmation of the contract on a durable medium within a reasonable time after conclusion, at the latest at the time of delivery or before performance begins.
- **Omnibus Directive (2019/2161)**: Amends the Consumer Rights Directive; penalties for cross-border infringements can reach at least 4% of annual turnover in the affected Member State(s), or EUR 2 million where turnover information is not available.
- **Dark patterns prohibition**: The Digital Services Act (Regulation 2022/2065, Art. 25) prohibits online platforms from designing interfaces in a way that deceives or manipulates users, which includes deceptive trial-to-paid flows.

**Common trap:** A checkbox that says "I agree to start receiving the service immediately" is not enough if it does not also explicitly state "and I acknowledge that I lose my right of withdrawal." Both statements are required under Art. 16(m).

### US / California: Automatic Renewal Law (ARL)

- **California Business & Professions Code sections 17600-17606** (amended effective July 1, 2022):
  - **Clear and conspicuous disclosure** of the automatic renewal offer terms before the consumer subscribes (section 17602(a)(1)).
  - Disclosure must include: (a) that the subscription will continue until cancelled; (b) the cancellation policy; (c) the recurring charge amount or range of charges; (d) the length of each renewal term.
  - **Affirmative consent**: Must obtain the consumer's affirmative consent to the agreement containing the automatic renewal terms (section 17602(a)(2)).
  - **Acknowledgment**: Must provide an acknowledgment that includes the automatic renewal terms, cancellation policy, and information on how to cancel in a manner that is capable of being retained by the consumer (section 17602(a)(3)).
  - **Free trial specifics** (section 17602(a)(1)): If the offer includes a free trial, the disclosure must include the price that will be charged after the trial ends, the date or conditions under which the trial ends, and that the consumer will be charged unless they cancel.
  - **Easy cancellation** (section 17602(c)): Must provide a cost-effective, timely, and easy-to-use mechanism for cancellation, including an online mechanism if the consumer agreed online.
- **FTC Negative Option Rule (16 CFR Part 425)** and the 2023 proposed "Click-to-Cancel" rule (finalized October 2024):
  - Sellers must make it at least as easy to cancel as it was to subscribe.
  - Must obtain express informed consent before charging.
  - Must provide simple cancellation mechanisms.
  - Penalties: Civil penalties up to $50,120 per violation (adjusted annually for inflation).
- **Restore Online Shoppers' Confidence Act (ROSCA), 15 U.S.C. sections 8401-8405**: Prohibits charging consumers for goods or services sold through negative option features unless the seller clearly and conspicuously discloses all material terms, obtains express informed consent, and provides simple cancellation mechanisms.

**Common trap:** Placing the auto-renewal terms in the general Terms of Service that nobody reads does NOT satisfy the "clear and conspicuous" requirement. The terms must be presented at the point of purchase, separate from the general terms.

### Russia

- **Federal Law No. 2300-1 "On Protection of Consumer Rights" (07.02.1992), Art. 10, Art. 16**: The consumer must receive full and accurate information about the service in advance. Conditions that infringe on consumer rights compared to the rules established by law are void.
- **Federal Law No. 38-FZ "On Advertising" (13.03.2006), Art. 5, Art. 28**: Advertising of financial and similar services must contain all conditions that affect the price. Omitting the auto-renewal price while advertising a free trial may constitute misleading advertising.
- **Civil Code of the Russian Federation, Art. 428**: Contracts of adhesion (standard-form contracts) may be challenged if they contain terms that the consumer would not have accepted given a choice.
- **Explicit consent and notification**: While there is no single statute identical to California's ARL, the combination of consumer protection law and advertising law requires: (1) explicit consent to the terms of conversion, (2) notification before the first charge (recommended at least 3 days before), (3) clear information about pricing and cancellation.
- **Rospotrebnadzor enforcement**: The Federal Service for Consumer Rights Protection actively investigates consumer complaints. Fines range from RUB 10,000 to RUB 500,000 for legal entities (Administrative Code Art. 14.7, Art. 14.8).

### UAE

- **Federal Decree-Law No. 15/2020 on Consumer Protection**, Art. 4-5: Suppliers must provide accurate and clear information about goods and services, including pricing. Misleading or deceptive commercial practices are prohibited.
- **Cabinet Resolution No. 66/2023** on E-Commerce: Establishes requirements for electronic contracts, including clear disclosure of terms before purchase.
- No statutory automatic renewal law specifically, but the general consumer protection framework applies. The Department of Economic Development (DED) in each emirate handles complaints and can impose fines.
- **DIFC/ADGM**: For entities operating from financial free zones, additional consumer protection rules may apply under common law frameworks.

**Common trap:** Assuming that the absence of specific auto-renewal legislation means anything goes. The general consumer protection laws are broad enough to cover deceptive trial-to-paid conversions.

### Pre-Trial Disclosure Checklist

Before any free trial begins, the following must be clearly disclosed and the consumer must affirmatively consent:

- [ ] The fact that the trial will automatically convert to a paid subscription
- [ ] The exact date or event that triggers the conversion
- [ ] The price that will be charged after conversion (including currency and frequency)
- [ ] The billing frequency (monthly, annual, etc.)
- [ ] How to cancel before the trial ends (specific steps, not just "contact support")
- [ ] The cancellation deadline (e.g., "cancel at least 24 hours before the trial ends")
- [ ] For EU consumers: explicit acknowledgment that beginning the service during the cooling-off period means waiving the right of withdrawal
- [ ] A direct link or path to the cancellation mechanism
- [ ] Confirmation sent via email or other durable medium immediately after sign-up

---

## 2. Web Accessibility Lawsuits

Web accessibility litigation is a fast-growing risk area that most SaaS and education platforms ignore until they receive a demand letter. The financial exposure is significant: in the US alone, there were over 4,600 federal ADA digital accessibility lawsuits in 2023, with numbers continuing to climb.

### US: ADA Title III

- **Americans with Disabilities Act (42 U.S.C. sections 12181-12189), Title III**: Prohibits discrimination on the basis of disability in places of "public accommodation." Courts have increasingly held that websites and mobile applications qualify as places of public accommodation or are sufficiently connected to a physical place of public accommodation.
- **DOJ Final Rule (April 2024, 28 CFR Part 36)**: The Department of Justice issued a final rule requiring state and local government web content to conform to WCAG 2.1 Level AA. While this applies directly to government entities, it signals the standard that courts and regulators consider reasonable for the private sector as well.
- **Lawsuit volume**: 4,600+ federal lawsuits filed in 2023; plaintiff's attorneys send thousands more demand letters that settle without litigation. The most targeted industries include e-commerce, food service, education, and SaaS.
- **Serial plaintiffs**: A small number of plaintiffs and law firms file the majority of cases. Firms like Murphy, Falto & Murphy, and individuals who file 100+ cases per year are common. Settling one case does not prevent another plaintiff from suing over the same issues.
- **Damages and costs**: Typical settlement: $5,000-$50,000 for a first lawsuit, plus plaintiff's attorney fees ($10,000-$50,000+). Injunctive relief requiring remediation is standard. Repeat offenders face higher settlements.
- **California Unruh Civil Rights Act (Cal. Civ. Code section 51)**: Provides statutory minimum damages of $4,000 per occurrence. An ADA violation is automatically an Unruh violation. "Per occurrence" can be interpreted as each visit or each barrier encountered, potentially creating six- or seven-figure exposure.
- **New York**: Second most common jurisdiction for accessibility lawsuits. No statutory damages like California, but heavy litigation volume.

### EU: European Accessibility Act (EAA) -- Directive 2019/882

- **Mandatory compliance deadline: June 28, 2025** (already in effect at time of writing).
- **Scope**: Applies to products and services placed on the EU market, including: e-commerce services, banking services, e-books, and certain SaaS platforms that provide services covered by the directive.
- **Standard**: WCAG 2.1 Level AA (referenced through harmonized standard EN 301 549).
- **Applies to**: Any business offering covered services to EU consumers, regardless of where the business is located.
- **Enforcement**: Each Member State designates its own market surveillance authority. Penalties vary by country:

| Member State | Authority | Penalty Range | Legal Reference |
|---|---|---|---|
| Cyprus | Dept. of Labour Inspection | EUR 1,000 - 20,000 | Law 89(I)/2023 |
| Finland | Finnish Transport and Communications Agency (Traficom) | Up to EUR 150,000 | Act on Digital Services (306/2019, as amended) |
| Netherlands | Netherlands Authority for Consumers & Markets (ACM) | Up to EUR 250,000 | Implementation of Directive 2019/882 |
| Italy | AGID / AGCOM | EUR 5,000 - 150,000 | Law 4/2004 (Stanca Act, as amended by D.Lgs. 82/2022) |
| Germany | Federal states (Laender) | Up to EUR 100,000 | BFSG (Barrierefreiheitstaerkungsgesetz) |
| France | ARCOM / DINUM | Up to EUR 50,000 per year | RGAA (Referentiel General d'Amelioration de l'Accessibilite) |
| Spain | Ministry of Social Rights | EUR 301 - 1,000,000 | Royal Decree 1112/2018, updated 2023 |

### Common Accessibility Failures on SaaS / Education Sites

1. **Missing or incorrect alt text on images**: Decorative images without `alt=""`, informational images without descriptive alt text.
2. **Unlabeled form fields**: Login, registration, and checkout forms without associated `<label>` elements or `aria-label` attributes.
3. **Keyboard navigation traps**: Modal dialogs, dropdown menus, or custom widgets that cannot be operated or dismissed via keyboard alone.
4. **Insufficient color contrast**: Text-to-background contrast below the WCAG 2.1 AA minimum of 4.5:1 for normal text, 3:1 for large text.
5. **Auto-playing video/audio** without controls: Course content or promotional videos that play automatically without pause/stop controls.
6. **Missing captions on video content**: Education platforms often have extensive video content without captions or transcripts, violating both WCAG and, in the US, potentially Section 508 and the 21st Century Communications and Video Accessibility Act.
7. **Dynamic content updates without ARIA live regions**: Ajax-loaded content, progress indicators, and error messages that are not announced to screen readers.
8. **Inaccessible PDF documents**: Course materials, certificates, and invoices distributed as inaccessible PDFs.
9. **Touch target size**: Interactive elements smaller than the WCAG 2.2 minimum target size of 24x24 CSS pixels (WCAG 2.1 AA recommends 44x44).
10. **Missing skip navigation links**: Large navigation menus without a "skip to main content" link.

### How to Check: Testing Approach

**Automated tools** (catch approximately 30-40% of issues):
- **axe DevTools** (Deque Systems): Browser extension and CI integration. Free core rules, paid for full ruleset.
- **Lighthouse** (Google Chrome DevTools): Built-in accessibility audit. Good for quick checks but limited rule coverage.
- **WAVE** (WebAIM): Browser extension and API. Good visual overlay of issues.
- **Pa11y**: Open-source CLI tool for CI/CD pipeline integration.
- **IBM Equal Access Accessibility Checker**: Free browser extension and CI tool.

**Manual testing** (required for the remaining 60-70%):
- **Keyboard-only navigation**: Tab through the entire site. Can you reach and operate every interactive element? Can you see where focus is? Can you escape modals?
- **Screen reader testing**: Test with NVDA (Windows, free), JAWS (Windows, paid), VoiceOver (macOS/iOS, built-in), TalkBack (Android, built-in). At minimum, test with VoiceOver + Safari and NVDA + Chrome.
- **Zoom/magnification**: Test at 200% and 400% zoom. Does content reflow? Is anything cut off or overlapping?
- **Color contrast**: Use a contrast checker tool (e.g., Colour Contrast Analyser by TPGi) on all text elements.
- **Reduced motion**: Test with `prefers-reduced-motion` enabled. Do animations respect this setting?

**Recommended audit frequency**: Full audit annually; automated scans in CI/CD on every deployment; spot-check after major UI changes.

---

## 3. COPPA -- Children's Data

The Children's Online Privacy Protection Act is one of the most dangerous regulatory traps for education platforms. It applies even if you do not intend to collect data from children and even if your terms of service prohibit users under 13. If you have actual knowledge that you are collecting data from children under 13, you are subject to COPPA.

### Core Law: COPPA (15 U.S.C. sections 6501-6506)

- **Scope**: Applies to operators of commercial websites and online services directed to children under 13, or that have actual knowledge that they are collecting personal information from children under 13.
- **Implementing Rule**: 16 CFR Part 312 (FTC COPPA Rule).
- **"Personal information" under COPPA** includes: first and last name, home or physical address, email address, telephone number, Social Security number, persistent identifiers (cookies, device IDs) when used to track a user across sites, photographs/video/audio containing a child's image or voice, geolocation data, and any combination of information that permits physical or online contacting of a specific individual.

### Why Education Platforms Are Especially at Risk

- **Actual knowledge standard**: If a student profile says "age: 11" or "grade: 5th," or if a teacher creates accounts for a class of 10-year-olds, the platform has actual knowledge of collecting children's data.
- **School-issued accounts**: Many education platforms onboard students through school accounts. The platform cannot assume all students are 13+ without verification.
- **Analytics and tracking**: Even if the platform itself does not ask for age, third-party analytics tools (Google Analytics, Mixpanel, etc.) that set persistent identifiers on children's devices trigger COPPA.

### Verifiable Parental Consent (VPC)

Before collecting personal information from a child under 13, operators must obtain VPC using one of the FTC-approved methods:
1. Signed consent form returned by mail, fax, or electronic scan.
2. Credit card, debit card, or other online payment system transaction (where the parent is notified a charge will be placed).
3. Call to a toll-free number staffed by trained personnel.
4. Video conference with trained personnel.
5. Government-issued ID checked against a database, with the ID deleted after verification.
6. Knowledge-based authentication with security questions.
7. Face-matching technology comparing a parent's photo ID to a real-time selfie.

### 2024-2025 COPPA Rule Amendments (Effective April 22, 2025)

Key changes from the FTC's amended COPPA Rule:
- **School authorizations limited**: Schools may no longer consent on behalf of parents for commercial purposes. School consent is restricted to the educational context. If the education platform uses student data for any commercial purpose (advertising, product improvement unrelated to the service, marketing), separate parental consent is required.
- **Data retention limits**: Operators must retain children's personal information only as long as reasonably necessary to fulfill the purpose for which it was collected.
- **Enhanced security requirements**: Operators must implement and maintain reasonable procedures to protect the confidentiality, security, and integrity of children's personal information.
- **Expanded definition of personal information**: Biometric identifiers explicitly included.
- **Safe harbor programs**: Updated obligations for COPPA safe harbor organizations (e.g., CARU, iKeepSafe, kidSAFE, PRIVO).

### Enforcement Actions and Fines

| Company | Year | Fine | Violation |
|---|---|---|---|
| Epic Games (Fortnite) | 2022 | $275,000,000 | Collected personal information from children without parental consent; used dark patterns; enabled live communications with children without consent |
| Google/YouTube | 2019 | $170,000,000 | Tracked children across channels using persistent identifiers without parental consent |
| Musical.ly (now TikTok) | 2019 | $5,700,000 | Failed to obtain parental consent before collecting children's personal information |
| VTech Electronics | 2018 | $650,000 | Failed to obtain parental consent; poor data security leading to breach |
| Unacademy (India, but US-accessible) | 2024 | Investigation ongoing | Collecting data from child users without consent |

**Civil penalty**: Up to $53,088 per violation (2024 adjusted amount; adjusted annually for inflation). "Per violation" can mean per child, per instance of collection, or per day of ongoing violation.

### COPPA Compliance Checklist for Education Platforms

- [ ] Age gate or age verification at registration
- [ ] If users under 13 are permitted: full COPPA compliance program
- [ ] Verifiable parental consent mechanism implemented
- [ ] Direct notice to parents describing data collection practices
- [ ] Parental access and deletion rights implemented
- [ ] No behavioral advertising to children
- [ ] No conditioning participation on unnecessary data collection
- [ ] Audit all third-party SDKs and analytics for persistent identifiers
- [ ] If relying on school consent: restrict use to educational purposes only; do not use data for commercial purposes
- [ ] Data retention policy specific to children's data
- [ ] Annual COPPA compliance review

---

## 4. Testimonials and Income Claims

Testimonials and income claims are the single most common FTC enforcement trigger for education platforms, coaching businesses, and online course providers. The revised FTC Endorsement Guides dramatically changed the rules in 2023.

### FTC Endorsement Guides (16 CFR Part 255, revised June 29, 2023)

Key provisions:
- **section 255.2(b) -- Consumer endorsements**: An endorsement that makes representation about the experience of consumers in general (or a group of consumers) must either reflect the results that consumers generally achieve, OR clearly and conspicuously disclose the generally expected results.
- **Elimination of "results not typical" safe harbor**: The pre-2023 practice of adding "results not typical" or "individual results may vary" disclaimers is no longer sufficient. Advertisers must now either: (a) have evidence that the endorser's experience represents what consumers will generally achieve, or (b) clearly and conspicuously disclose what the generally expected results actually are.
- **section 255.5 -- Material connections**: When there is a connection between the endorser and the advertiser that might materially affect the weight or credibility of the endorsement, the connection must be clearly and conspicuously disclosed. This includes: payment, free products, employment, family relationships, business relationships, and any other material connection.
- **Endorser liability (new in 2023)**: Endorsers themselves (not just advertisers) may be liable for their statements in endorsements. This means influencers, affiliates, and students who provide testimonials can face personal liability.

### Income Claims

- **FTC Act, Section 5 (15 U.S.C. section 45)**: Prohibits unfair or deceptive acts or practices in or affecting commerce.
- **Income claims must be substantiated**: Any claim about income, earnings, or financial results must be supported by competent and reliable evidence at the time the claim is made. This means actual data, not projections or aspirational numbers.
- **Typical results standard**: If you showcase a student who earned $100,000 after taking your course, you must either: (a) have evidence that this result is typical, or (b) disclose what the typical student actually earns after completing the course.
- **Penalty**: Up to $50,120 per violation under the FTC Act (2024 adjusted amount). Each advertisement shown to each consumer can be a separate violation.

**Examples of violations in education:**
- "Earn 6 figures after completing our course" -- violation unless this is the typical result AND you have data to prove it.
- Showing screenshots of student earnings without disclosing they are atypical -- violation.
- "Our graduates earn an average of $85,000" -- must be substantiated with actual graduate outcome data, not cherry-picked.
- Student video testimonial saying "I made $50K in my first month" without disclosing this is an outlier -- violation.

### FTC Enforcement Examples in Education

- **FTC v. MOBE Ltd. (2018)**: $900 million judgment against online business education company for making deceptive income claims.
- **FTC v. Agora Financial / The Oxford Club (2020)**: Investigated for misleading income claims in financial education marketing.
- **FTC Operation Income Illusion (2022)**: Coordinated enforcement against multiple companies making deceptive income claims in business coaching and online education.

### Russia: Federal Law No. 38-FZ "On Advertising"

- **Art. 5**: Advertising must be trustworthy. Advertising is deemed untrustworthy if it contains information that does not correspond to reality regarding the results of use of the product or service.
- **Art. 28**: Advertising of financial services must contain all conditions that determine the actual cost. By analogy, income claims in education advertising must reflect actual, not exceptional, outcomes.
- **Fines**: RUB 100,000 to RUB 500,000 for legal entities for misleading advertising (Administrative Code, Art. 14.3). The Federal Antimonopoly Service (FAS) is the enforcement body.

### Compliance Requirements

- [ ] Audit all marketing materials for income or results claims
- [ ] Collect and maintain data on typical student/user outcomes
- [ ] Replace atypical testimonials with typical-result disclosures
- [ ] Add clear disclosures adjacent to any testimonial: "This result is not typical. The average student achieves [X]."
- [ ] Disclose material connections in all endorsements (paid, free access, affiliate, etc.)
- [ ] Review and update affiliate/influencer contracts to require FTC-compliant disclosures
- [ ] Document substantiation for every claim before publication
- [ ] Implement review process for user-submitted testimonials before publication

---

## 5. EU Geoblocking Regulation 2018/302

This regulation is widely misunderstood and routinely violated by SaaS platforms that do not realize they are covered.

### Core Requirements (Regulation (EU) 2018/302)

- **Art. 3 -- Access to online interfaces**: A trader cannot block or limit a customer's access to an online interface based on the customer's nationality, place of residence, or place of establishment. Automatic re-routing to a different version of the site based on IP address is also prohibited unless the customer explicitly consents and the original version remains accessible.
- **Art. 4 -- Access to goods or services**: A trader cannot apply different general conditions of access (including pricing) to customers based on nationality, place of residence, or place of establishment, in the following situations:
  - (a) Sale of goods delivered to a location where the trader offers delivery, or collected by the customer at a location agreed upon.
  - (b) Electronically supplied services (this covers most SaaS).
  - (c) Services received at a physical location in the territory of the trader.
- **Art. 5 -- Non-discrimination related to payment**: A trader cannot apply different conditions for a payment transaction based on the customer's nationality, place of residence, place of establishment, the location of the payment account, or the place of establishment of the payment service provider within the EU.

### What This Means for SaaS Platforms

1. **You cannot charge different prices to EU customers based on their country** (for the same electronically supplied service). A customer in Romania must be able to access the same offer at the same price as a customer in Germany.
2. **You cannot block access from certain EU countries**. If your SaaS is available in France, it must also be accessible from Bulgaria.
3. **You cannot refuse EU payment methods**. If you accept Visa from a German customer, you must also accept Visa from a Polish customer, even if the card was issued in Poland.
4. **You CAN offer different localized websites**, but you cannot force users to use them. A French customer must be able to access the .de version if they choose.

### Exceptions

- **Copyright-protected content** (Art. 4(1)(b) exception): Services whose main feature is providing access to copyright-protected works (e.g., streaming video, e-books, music) are currently exempt from Art. 4(1)(b). However, Art. 3 (access to the interface) still applies.
- **Audiovisual services**: Regulated under the Audiovisual Media Services Directive, not the Geoblocking Regulation.
- **Financial services, transport, healthcare, social services**: Excluded from the scope.
- **The exemption review** was due by March 2023 (Art. 9), and the Commission's evaluation considered extending the regulation to cover copyright-protected content. As of 2025, the exemption remains but is under ongoing review.

### Common SaaS Violations

- IP-based redirects that force users to a country-specific version without consent.
- Different pricing tiers displayed to users from different EU countries.
- Checkout pages that reject credit cards issued in certain EU countries.
- Requiring a local phone number or address for registration when the service is fully digital.
- Displaying "this service is not available in your country" to EU users.

### Enforcement

- Each Member State designates enforcement bodies. In many cases, this is the national consumer protection authority.
- **Penalties vary by Member State**; the regulation requires penalties to be "effective, proportionate and dissuasive."
- The European Commission published a list of designated enforcement bodies and provides a complaint mechanism for consumers.

---

## 6. Data Portability (GDPR Art. 20)

This right is often overlooked by SaaS and education platforms that focus their GDPR compliance on consent and data deletion, while ignoring the affirmative obligation to export data.

### GDPR Article 20: Right to Data Portability

- **Art. 20(1)**: The data subject has the right to receive their personal data in a structured, commonly used, and machine-readable format, and has the right to transmit that data to another controller without hindrance.
- **Art. 20(2)**: Where technically feasible, the data subject has the right to have personal data transmitted directly from one controller to another.
- **Applies when**: (a) Processing is based on consent (Art. 6(1)(a)) or on a contract (Art. 6(1)(b)), AND (b) processing is carried out by automated means.

### What Must Be Exportable

For education platforms:
- Student profile data (name, email, preferences, settings)
- Course progress and completion records
- Quiz and assessment results
- Certificates and credentials earned
- Notes and annotations created by the student
- Forum posts and comments authored by the student
- Files uploaded by the student
- Learning path history and activity logs
- Subscription and payment history (as it relates to the data subject)

For SaaS platforms generally:
- User account data
- All content created by the user
- Usage history and activity logs
- Customization and settings
- Integrations and connected service configurations (where the data relates to the user)

### Format Requirements

- **"Structured, commonly used, and machine-readable"**: The EDPB (European Data Protection Board) Guidelines on Data Portability (WP242 rev.01) recommend formats such as CSV, JSON, XML. Proprietary formats that require specific software to read do not satisfy the requirement.
- **API option**: Providing a well-documented API for data export can satisfy Art. 20(2) (direct transmission). This is considered best practice by the EDPB.

### Penalties

- Data portability violations are penalized under GDPR Art. 83(5)(b): up to EUR 20,000,000 or 4% of total worldwide annual turnover, whichever is higher.
- While there have been relatively few enforcement actions specifically for Art. 20 violations to date, DPAs are increasingly scrutinizing data portability in their audits. The Austrian DPA (DSB) and French DPA (CNIL) have both issued guidance specifically on Art. 20 compliance for online services.

### Common Failures

- Offering only a PDF export (not machine-readable for most data types).
- Export function that takes weeks to process (must be without undue delay; GDPR Art. 12(3) sets a one-month maximum, extendable by two months for complex requests).
- Requiring the user to contact support instead of providing a self-service export tool.
- Omitting certain data categories from the export (e.g., exporting profile data but not activity logs).
- Exporting data in a format that cannot be imported into a competing service.

---

## 7. Affiliate/Referral Programs

Affiliate and referral programs create legal exposure that many platforms underestimate. The platform is typically liable for the claims its affiliates make, even if those claims violate the affiliate agreement.

### US: FTC Requirements

- **FTC Endorsement Guides, section 255.5**: Any material connection between an endorser and the seller must be disclosed clearly and conspicuously. An affiliate commission is a material connection.
- **Disclosure requirements**:
  - Must be clear and unambiguous (e.g., "#ad," "Paid partnership," "I earn a commission if you purchase through my link").
  - Must be placed where consumers will see it before clicking or engaging (not buried at the bottom of a page or in a collapsed section).
  - Must be in the same medium as the endorsement (video endorsement requires disclosure in the video, not just the description).
  - Vague terms like "ambassador" or "partner" are insufficient.
- **Platform liability**: The FTC holds advertisers responsible for the statements made by their affiliates. If an affiliate makes a deceptive income claim while promoting your education platform, you are liable. (See FTC Enforcement Policy Statement on Deceptive Advertising, appended to Cliffdale Associates, 103 F.T.C. 110 (1984).)
- **Required affiliate agreement provisions**: Platform should require affiliates to (a) disclose the material connection, (b) not make unauthorized claims, (c) comply with FTC guidelines, (d) submit promotional materials for review, and (e) indemnify the platform for non-compliant promotions.

### EU: Unfair Commercial Practices Directive (2005/29/EC)

- **Art. 6 -- Misleading actions**: A commercial practice is misleading if it contains false information or deceives the average consumer, including with respect to the nature or origin of the recommendation.
- **Art. 7 -- Misleading omissions**: Failing to disclose the commercial intent of a practice (including that an endorsement is paid) is a misleading omission.
- **Annex I, No. 11**: Using editorial content in the media to promote a product where a trader has paid for the promotion without making that clear (advertorials) is a practice deemed unfair in all circumstances.
- **Digital Services Act (2022/2065), Art. 26**: Online platforms must ensure that advertisements are clearly identifiable as such, including the identity of the person on whose behalf the advertisement is presented.
- **Penalty**: Varies by Member State. Under the Omnibus Directive (2019/2161), cross-border infringements can attract fines of at least 4% of annual turnover or EUR 2 million.

### Russia: Federal Law No. 38-FZ "On Advertising"

- **Art. 5(9)**: Advertising that is presented as a personal opinion or recommendation without disclosing that it is paid advertising is prohibited.
- **Art. 18.1 (added 2022)**: Specific requirements for advertising distributed on the internet, including mandatory labeling ("erid" identifier) and registration with the Unified Register of Internet Advertising (ERIR / ORD system). All online advertising, including affiliate links, must be registered and labeled. Non-compliance: fines from RUB 100,000 to RUB 500,000 for legal entities.
- **Art. 12**: Advertising of products using other people's endorsements without their consent is prohibited. When consent is given, the material connection must be disclosed.

### Compliance Checklist for Affiliate Programs

- [ ] Written affiliate agreement with FTC/EU/local compliance requirements
- [ ] Mandatory disclosure language provided to affiliates (with examples)
- [ ] Prohibition on unauthorized income, earnings, or results claims
- [ ] Pre-approval process for affiliate marketing materials (or random auditing)
- [ ] Monitoring program to audit affiliate compliance
- [ ] Termination provisions for non-compliant affiliates
- [ ] Russia-specific: registration with ORD, erid labeling on all affiliate content
- [ ] Record-keeping: maintain evidence of disclosures made by affiliates
- [ ] Training materials or onboarding guide for new affiliates

---

## 8. User-Generated Content Liability

Platforms that host user-generated content (UGC) face a complex web of liability regimes. The legal requirements differ significantly between the US, EU, and Russia, and getting them wrong can mean losing safe harbor protections entirely.

### EU: Digital Services Act (Regulation 2022/2065)

- **Art. 6 -- Conditional exemption for hosting services**: Hosting providers (including SaaS platforms hosting UGC) are not liable for user-stored information provided they: (a) do not have actual knowledge of illegal content, or (b) upon obtaining such knowledge, act expeditiously to remove or disable access.
- **Art. 16 -- Notice-and-action mechanisms**: All hosting service providers must put in place mechanisms to allow any individual or entity to notify them of the presence of illegal content. The mechanism must be easy to access, user-friendly, and allow submission electronically. Notices must include: explanation of why the content is illegal, exact URL or identifier, name and email of the notifying party, and a declaration of good faith.
- **Art. 17 -- Statement of reasons**: When a platform removes or restricts content, it must provide a clear and specific statement of reasons to the affected content provider.
- **Art. 20 -- Internal complaint-handling**: Online platforms must provide an internal complaint-handling system for at least 6 months following a content moderation decision.
- **Art. 21 -- Out-of-court dispute settlement**: Users must be informed of their right to out-of-court dispute settlement via certified bodies.
- **Art. 22 -- Trusted flaggers**: Platforms must prioritize notices from "trusted flaggers" designated by Digital Services Coordinators.
- **Very Large Online Platforms (VLOPs, >45 million EU users)**: Additional obligations under Arts. 33-43, including systemic risk assessments, independent audits, and transparency reporting.
- **Penalties (Art. 52)**: Up to 6% of worldwide annual turnover for the most serious violations.

### US: DMCA (17 U.S.C. section 512)

- **Section 512(c) -- Safe harbor for hosting**: Service providers are not liable for user-uploaded infringing content if they: (a) do not have actual knowledge that the material is infringing; (b) are not aware of facts or circumstances from which infringing activity is apparent; (c) upon obtaining such knowledge, act expeditiously to remove the material; and (d) do not receive a financial benefit directly attributable to the infringing activity where they have the right and ability to control it.
- **Section 512(c)(2) -- Designated agent**: The service provider must designate an agent to receive notifications of claimed infringement and register that agent with the U.S. Copyright Office. Failure to register means no safe harbor.
- **Section 512(c)(3) -- DMCA takedown notice requirements**: A valid notice must include: identification of the copyrighted work, identification of the infringing material and its location, contact information of the complaining party, a good faith statement, an accuracy statement under penalty of perjury, and the copyright owner's signature.
- **Section 512(g) -- Counter-notification and put-back**: The service provider must have a counter-notification procedure allowing the content uploader to contest the takedown. If a valid counter-notice is received and the copyright holder does not file a lawsuit within 10-14 business days, the material must be restored.
- **Section 512(f) -- Misrepresentation**: Any person who knowingly materially misrepresents that material is infringing (or that it was removed by mistake) may be liable for damages.
- **CDA Section 230 (47 U.S.C. section 230)**: Provides broad immunity for platforms from liability for user-generated content (excluding intellectual property, federal criminal law, and certain other exceptions). This is separate from and complementary to DMCA safe harbors.

### Russia: Federal Law No. 149-FZ "On Information, Information Technologies and Information Protection"

- **Art. 10.1 -- Information intermediary liability**: An information intermediary (hosting provider, search engine) is not liable for content posted by third parties provided they: (a) do not initiate the transfer, (b) do not select the recipient, (c) do not modify the information, and (d) were not aware of the illegality of the information.
- **Art. 15.1-15.8 -- Blocking and removal**: Roskomnadzor (the Federal Service for Supervision of Communications) maintains a registry of prohibited content. Hosting providers must remove content within 24 hours of receiving a Roskomnadzor notice for certain categories (child exploitation, drug promotion, suicide promotion) and must comply with court orders for other categories.
- **Art. 15.5 -- "Landing page" requirement**: Information dissemination organizers must store metadata of communications on Russian territory for 6 months and content for 6 months (Yarovaya Law amendments). This applies to messaging and social platforms.
- **Federal Law No. 236-FZ (2021) -- "Landing" law for social networks**: Social networks with over 500,000 daily Russian users must have a Russian legal entity or representative, implement content moderation per Russian law, and publish reporting forms for illegal content.

### Minimum UGC Compliance Setup

- [ ] Clearly published notice-and-takedown policy
- [ ] Easy-to-use reporting mechanism accessible from every content page
- [ ] DMCA designated agent registered with the U.S. Copyright Office (if US market)
- [ ] Counter-notification procedure
- [ ] Content moderation policy and statement of reasons template (DSA compliance)
- [ ] Internal complaint-handling system (DSA Art. 20)
- [ ] Response time SLAs: illegal content within 24 hours; other notices within 7 days
- [ ] Russia: compliance with Roskomnadzor requirements if accessible to Russian users
- [ ] Record retention: keep all notices, actions taken, and communications for at least 3 years

---

## 9. Currency, Tax, and Pricing

Pricing errors and tax non-compliance are among the most expensive traps for SaaS platforms operating internationally. VAT obligations alone can create millions in retroactive liability.

### EU VAT One-Stop Shop (OSS) -- Council Directive 2006/112/EC (as amended)

- **Art. 58**: Electronically supplied services provided to non-taxable persons (consumers) are taxed at the place where the consumer is established, has a permanent address, or usually resides.
- **VAT OSS (One-Stop Shop)**: Allows a business to register in a single EU Member State and declare/pay VAT for all EU B2C digital service sales through a single return. Eliminates the need to register in every Member State.
- **Threshold**: Since July 1, 2021, the previous EUR 10,000 distance selling threshold applies. Below this threshold, a business may charge its own Member State's VAT rate. Above it, the destination country's rate must be applied.
- **VAT rates for digital services** (selected, as of 2025):

| Country | Standard Rate | Reduced Rate (if applicable to digital education) |
|---|---|---|
| Germany | 19% | 7% (for certain educational materials) |
| France | 20% | 5.5% (for e-books and certain digital education) |
| Netherlands | 21% | 9% (for e-books) |
| Italy | 22% | 4% (for e-books); education may qualify |
| Spain | 21% | 4% (for e-books) |
| Ireland | 23% | 9% (for e-newspapers, e-books) |
| Poland | 23% | 5% (for e-books) |
| Sweden | 25% | 6% (for e-books) |

- **Invoice requirement**: VAT-compliant invoices must be issued for B2B transactions. For B2C digital services, the OSS return substitutes for individual invoices in most cases, but the platform must still maintain sufficient records.

### Pricing Display Requirements

- **EU Consumer Rights Directive (2011/83/EU), Art. 6(1)(e)**: The total price inclusive of taxes must be displayed before the consumer is bound by the contract. No hidden fees at checkout.
- **Omnibus Directive (2019/2161)**: Price reduction announcements must show the prior price (lowest price in the last 30 days). This applies to SaaS platforms running promotional pricing.
- **EU Price Indication Directive (98/6/EC)**: Selling price must include all taxes and charges.
- **Dark patterns**: Adding undisclosed fees at checkout ("drip pricing") is classified as a dark pattern under the DSA (Art. 25) and violates the Consumer Rights Directive.

### Russia

- **Federal Law No. 2300-1 "On Protection of Consumer Rights," Art. 10**: The seller must provide the consumer with necessary and reliable information about goods (services) in a timely manner, ensuring the opportunity to make the right choice. Prices must be in Russian rubles.
- **Civil Code, Art. 317**: Monetary obligations must be expressed in rubles. A contract may stipulate that the obligation is payable in rubles in an amount equivalent to a foreign currency or conventional monetary unit, but the actual payment must be in rubles (unless the parties are authorized for foreign currency transactions).
- **Practical effect for SaaS**: If you serve Russian consumers, you should either price in rubles or display a ruble equivalent alongside the foreign currency price. Payment in rubles must be accepted.

### UAE

- **VAT at 5%** applies to digital services (Federal Decree-Law No. 8/2017 on Value Added Tax, Art. 31). Non-resident providers of electronic services to UAE consumers must register for VAT if their supplies exceed AED 375,000 (mandatory) or AED 187,500 (voluntary).
- **Federal Tax Authority (FTA)** is the enforcement body. Non-registration penalties: AED 20,000. Late filing: AED 1,000 first offense, AED 2,000 for repeat offenses within 24 months.

### Common Pricing Traps

1. **Showing tax-exclusive prices to EU consumers**: All prices shown to consumers must include VAT. Showing "$19/mo" and adding VAT at checkout violates the Consumer Rights Directive.
2. **Not collecting VAT in countries where you have no entity**: The OSS system requires you to collect and remit VAT even if you have no physical presence. Failure to do so creates retroactive liability.
3. **Drip pricing / hidden fees**: Processing fees, "platform fees," or "service charges" added at checkout that were not disclosed on the pricing page.
4. **Dynamic pricing without disclosure**: Showing different prices to different users based on browsing history or device without disclosure may violate unfair commercial practices rules.
5. **Free-to-paid without tax recalculation**: When a free trial converts, the first charge must include the correct VAT rate for the consumer's location.

---

## 10. AI in Education Platforms

AI regulation is developing rapidly, and education is classified as a high-risk domain under the EU AI Act. Platforms that use AI for grading, assessment, personalization, or content generation face significant new compliance obligations.

### EU AI Act (Regulation 2024/1689)

- **Education as high-risk (Annex III, point 3)**: AI systems intended to be used for: (a) determining access to or assignment to educational and vocational training institutions; (b) evaluating learning outcomes, including when those outcomes are used to steer the learning process; (c) assessing the appropriate level of education an individual will receive or be able to access; (d) monitoring and detecting prohibited behavior during tests.
- **High-risk obligations (Chapter III, Section 2)**:
  - **Art. 9 -- Risk management system**: Continuous, iterative risk management throughout the AI system's lifecycle.
  - **Art. 10 -- Data governance**: Training, validation, and testing data must be subject to appropriate data governance and management practices.
  - **Art. 11 -- Technical documentation**: Detailed technical documentation must be drawn up before the system is placed on the market.
  - **Art. 13 -- Transparency and information**: The system must be designed to enable users to interpret its output and use it appropriately.
  - **Art. 14 -- Human oversight**: Designed to be effectively overseen by natural persons, including ability to override or reverse outputs.
  - **Art. 15 -- Accuracy, robustness, cybersecurity**: Must achieve appropriate levels of accuracy, robustness, and cybersecurity.
  - **Art. 16-29 -- Provider obligations**: Registration in EU database, conformity assessment, quality management system, post-market monitoring.
- **Timeline for high-risk AI in education**:
  - **August 1, 2025**: Prohibited AI practices (Art. 5) take effect.
  - **August 2, 2025**: Provisions on notified bodies.
  - **August 2, 2026**: High-risk AI system requirements (including education) become enforceable. This is the key deadline for education platforms.
- **Penalties (Art. 99)**:
  - Prohibited AI practices: up to EUR 35,000,000 or 7% of worldwide annual turnover.
  - High-risk non-compliance: up to EUR 15,000,000 or 3% of worldwide annual turnover.
  - Supplying incorrect information: up to EUR 7,500,000 or 1% of worldwide annual turnover.

### US State AI Legislation

Multiple US states have enacted or are enacting AI-specific legislation:

- **Colorado AI Act (SB 24-205)**: Effective February 1, 2026. Applies to "developers" and "deployers" of "high-risk AI systems," which includes systems making "consequential decisions" in education. Requirements: impact assessment, risk management, transparency notice to consumers, disclosure that an AI system is being used.
- **Texas AI Act (expected 2026)**: Pending legislation targeting high-risk AI with disclosure and impact assessment requirements.
- **California AB 2013 (GenAI Transparency Act)**: Effective January 1, 2026. Requires developers of generative AI to post documentation about training data on their website.
- **Illinois AI Video Interview Act (820 ILCS 42)**: Already in effect. Prohibits use of AI to analyze video interviews without consent. Relevant if education platforms use AI-assisted admissions interviews.
- **New York City Local Law 144 (2023)**: Restricts use of automated employment decision tools. While focused on employment, the regulatory framework is influential for education AI regulation.

### Specific Risks for Education Platforms

1. **AI-powered grading/assessment**: Classified as high-risk under EU AI Act. Must implement full conformity assessment, technical documentation, and human oversight.
2. **AI-generated course content**: Must disclose to students that content is AI-generated (EU AI Act Art. 50 transparency obligations for AI-generated content).
3. **Adaptive learning / personalized paths**: If the AI determines the "appropriate level of education," it is high-risk under Annex III(3)(c).
4. **Proctoring software**: AI-based exam proctoring is explicitly high-risk (Annex III(3)(d)). Several EU DPAs have already flagged proctoring tools for GDPR violations (CNIL, Dutch DPA).
5. **Student profiling**: Using AI to create profiles of students based on their behavior, performance, or characteristics for any purpose (recommendations, interventions, marketing) implicates both GDPR Art. 22 (automated individual decision-making) and the AI Act.

### Compliance Steps for AI in Education

- [ ] Inventory all AI systems used in the platform (including third-party tools)
- [ ] Classify each system under the EU AI Act risk categories
- [ ] For high-risk systems: begin conformity assessment process (before August 2026 deadline)
- [ ] Implement human oversight mechanisms for AI-driven grading and assessment
- [ ] Prepare technical documentation for each high-risk AI system
- [ ] Implement transparency notices: inform users when AI is being used
- [ ] For generative AI outputs: label AI-generated content
- [ ] Conduct and document impact assessments (Colorado requirement for US market)
- [ ] Review AI training data for bias and representativeness
- [ ] Establish post-market monitoring plan

---

## 11. PCI DSS v4.0 for Stored Cards

PCI DSS v4.0 compliance became mandatory on March 31, 2025. SaaS and education platforms that store credit card data for recurring subscription payments are directly affected.

### PCI DSS v4.0 (Payment Card Industry Data Security Standard)

- **Mandatory compliance date: March 31, 2025** (transition from v3.2.1 completed).
- **Applies to**: Any entity that stores, processes, or transmits cardholder data, or that could affect the security of the cardholder data environment. This includes SaaS platforms that store card-on-file for recurring billing.

### Key Changes from v3.2.1 to v4.0

1. **Requirement 3.5 -- Primary Account Number (PAN) secured wherever stored**: Enhanced encryption requirements. PAN must be rendered unreadable anywhere it is stored using strong cryptography with associated key-management processes.
2. **Requirement 8.3 -- Multi-Factor Authentication (MFA)**: MFA is now required for all access into the cardholder data environment (CDE), not just remote access. This includes administrative access from within the corporate network.
3. **Requirement 6.4.3 -- Client-side script management**: All payment page scripts that are loaded and executed in the consumer's browser must be managed. This includes: maintaining an inventory of all scripts, justification for each script, integrity verification mechanism. This requirement targets Magecart-style attacks and affects SaaS checkout pages.
4. **Requirement 12.3.1 -- Targeted risk analysis**: Organizations must perform targeted risk analyses to define the frequency of periodic activities (e.g., log reviews, vulnerability scans).
5. **Requirement 5.4.1 -- Anti-phishing mechanisms**: Automated mechanisms to detect and protect personnel against phishing attacks.
6. **Requirement 11.6.1 -- Change-detection mechanisms on payment pages**: A change-and-tamper-detection mechanism must be deployed on the payment page to alert on unauthorized modifications to HTTP headers and script contents.
7. **Requirement 8.6 -- System and application account management**: Enhanced requirements for managing application and system accounts (service accounts), including restricting interactive use and rotating credentials.

### Tokenization as Risk Reduction

- **Tokenization**: Replacing PAN with a non-sensitive token reduces PCI DSS scope significantly. If you use a payment processor's tokenization (e.g., Stripe, Braintree), your PCI scope is reduced to SAQ A or SAQ A-EP, depending on your checkout integration.
- **Hosted payment fields**: Using the payment processor's hosted iframes (e.g., Stripe Elements, Braintree Hosted Fields) ensures that card data never touches your servers, further reducing scope.
- **Important**: Even with tokenization, Requirement 6.4.3 (client-side script management on payment pages) and Requirement 11.6.1 (change detection) still apply to your checkout page.

### Non-Compliance Consequences

- **Fines from card brands**: Visa and Mastercard can fine acquiring banks $5,000-$100,000 per month for non-compliance, which is passed through to the merchant.
- **Increased transaction fees**: Non-compliant merchants may face higher interchange rates.
- **Breach liability**: In the event of a data breach, non-compliant merchants face full liability for fraud losses, forensic investigation costs, card reissuance costs, and regulatory fines.
- **Loss of payment processing**: Acquiring banks can terminate the merchant's ability to accept card payments.

---

## 12. Cooling-Off Periods Summary Table

Cooling-off periods (also called "withdrawal rights" or "cancellation periods") are among the most commonly ignored consumer rights in digital subscriptions. Failing to honor them can result in forced refunds and regulatory penalties.

| Jurisdiction | Period | Legal Basis | Conditions / Exceptions | Notification Requirement |
|---|---|---|---|---|
| **EU (all Member States)** | 14 calendar days from contract conclusion | Consumer Rights Directive 2011/83/EU, Art. 9 | Exception for digital content: consumer must explicitly consent to immediate performance AND acknowledge loss of withdrawal right (Art. 16(m)). Both conditions must be met; a pre-ticked checkbox is NOT valid consent. | Trader must inform consumer of the right before contract is concluded (Art. 6(1)(h)). If not informed, the period extends to 12 months + 14 days (Art. 10). |
| **UK** | 14 calendar days | Consumer Contracts (Information, Cancellation and Additional Charges) Regulations 2013, Reg. 29-30 | Similar to EU: consumer must give express consent to begin digital content delivery during the cancellation period AND acknowledge loss of cancellation right. | Trader must inform consumer before contract is concluded. If not informed, period extends up to 12 months. |
| **Russia** | 14 days for consumer contracts; services exception | Federal Law No. 2300-1, Art. 25, Art. 32 | Art. 32: Consumer may refuse to execute a services contract at any time, provided they pay the contractor for actually incurred expenses. For digital services fully rendered, no refund obligation. The 14-day return right (Art. 25) technically applies to goods, but courts have applied analogous reasoning to digital subscriptions. | Consumer must be informed of their rights under Art. 10. |
| **UAE** | No statutory cooling-off period for digital services | Federal Decree-Law No. 15/2020 on Consumer Protection | General consumer protection applies. No specific statutory withdrawal right for digital services. However, misleading practices that induce purchase may result in mandatory refund orders from DED. Some Dubai-specific regulations for e-commerce may apply. | N/A |
| **US (Federal)** | No federal cooling-off period for digital services | FTC Cooling-Off Rule (16 CFR 429) applies only to door-to-door sales | The FTC Cooling-Off Rule provides a 3-day right to cancel, but applies only to sales made at the buyer's home or at locations that are not the seller's permanent place of business. It does not apply to online sales. | N/A for online sales. |
| **US (California)** | No specific cooling-off period, but ARL applies | Cal. Bus. & Prof. Code sections 17600-17606 | California's ARL requires clear disclosure and easy cancellation, but does not provide a statutory cooling-off period. The consumer must be able to cancel at any time. California has a separate 3-day cooling-off right for home solicitation contracts (Cal. Civ. Code section 1689.5). | ARL requires acknowledgment with cancellation instructions. |
| **Australia** | 10 business days (for unsolicited consumer agreements) | Australian Consumer Law, sections 69-95 | The 10-day cooling-off applies to unsolicited agreements (e.g., telemarketing). Standard online subscriptions are not covered unless they were unsolicited. | Supplier must inform consumer of the right to terminate. |
| **South Korea** | 7 days | Act on Consumer Protection in Electronic Commerce (ECPA), Art. 17 | Consumer may withdraw within 7 days of receiving digital content, unless the digital content has been used or the benefit has been partly consumed. | Must inform consumer of withdrawal right. |
| **Brazil** | 7 days | Consumer Protection Code (CDC), Art. 49 | Applies to all distance contracts. Consumer may withdraw within 7 days of contract signature or receipt of product/service. Full refund required. | Seller must inform consumer. |

### Key Trap: EU 12-Month Extension

If you fail to inform an EU consumer of their right of withdrawal **before** the contract is concluded, the withdrawal period is automatically extended from 14 days to **12 months and 14 days** (Art. 10 of the Consumer Rights Directive). This applies retroactively, meaning the consumer can demand a refund up to 12 months and 14 days after purchase. Many SaaS platforms discover this only after receiving a wave of refund requests.

---

## 13. Anti-Money Laundering

AML obligations are a hidden trap for SaaS platforms that process high-value transactions or serve as financial intermediaries. Many platforms are surprised to learn that they may have AML obligations even though they are not financial institutions.

### When AML Applies to SaaS / Education Platforms

- **High-value subscriptions or courses**: In many jurisdictions, platforms facilitating transactions above certain thresholds may be classified as payment intermediaries or service providers subject to AML.
- **Marketplace models**: If your platform facilitates payments between instructors and students (taking a commission), you may be acting as a payment services provider, triggering AML obligations.
- **Stored value / credits / wallet features**: If users can pre-load funds, purchase credits, or maintain a balance on the platform, this may constitute e-money issuance, subject to AML under the EU's Anti-Money Laundering Directives and national implementations.

### EU: Anti-Money Laundering Directives (AMLD)

- **6th Anti-Money Laundering Directive (6AMLD, Directive 2018/1673)**: Harmonizes money laundering offenses across the EU.
- **AML Regulation (Regulation 2024/1624, "AMLR")**: Part of the 2024 AML package, creates a single EU rulebook for AML/CFT. Expected to apply from July 2027.
- **AMLA (Anti-Money Laundering Authority)**: New EU-level authority established by Regulation 2024/1620, headquartered in Frankfurt. Will directly supervise certain high-risk entities from 2025.
- **Obligated entities** include: credit institutions, financial institutions, certain professional service providers, and (critically) providers of services for the transfer of value, including virtual assets.
- **KYC / Customer Due Diligence (CDD)**: If applicable, platforms must: (a) identify and verify the customer's identity, (b) identify the beneficial owner, (c) assess the purpose and intended nature of the business relationship, (d) conduct ongoing monitoring.
- **Suspicious Activity Reporting**: Obligated entities must report suspicious transactions to the national Financial Intelligence Unit (FIU).

### Russia: Federal Law No. 115-FZ "On Counteracting the Legalization (Laundering) of Criminally Obtained Incomes"

- **Art. 6**: Transactions subject to mandatory control include cash transactions over RUB 600,000, certain electronic transfers, and transactions with entities from FATF-listed countries.
- **Art. 7**: Organizations carrying out operations with money or property must identify clients, maintain records, and report suspicious activity to Rosfinmonitoring.
- **Application to SaaS**: If the platform processes payments directly (not through a licensed payment provider), it may fall under the scope of 115-FZ.

### UAE: Federal Decree-Law No. 20/2018 on Anti-Money Laundering and Combating the Financing of Terrorism

- **Art. 4**: Financial institutions and designated non-financial businesses must conduct customer due diligence.
- **CBUAE (Central Bank of the UAE)** issues implementing regulations. Fines for non-compliance: up to AED 5,000,000 for legal entities.
- **Free zones (DIFC/ADGM)**: Have their own AML regimes that may apply to tech companies operating from these zones.

### Practical Steps

- Assess whether your payment model (marketplace, stored credits, high-value transactions) triggers AML obligations in any operating jurisdiction.
- If in doubt, consult with an AML specialist. The consequences of non-compliance include criminal liability for officers and directors.
- Use a licensed payment service provider (Stripe, PayPal, Adyen) to avoid becoming a payment intermediary subject to AML directly.
- Even when using third-party payment processors, if you operate a marketplace model with payouts to instructors, you may still have AML obligations.

---

## 14. Key Compliance Deadlines 2025-2026

This table consolidates upcoming regulatory deadlines that affect SaaS and online education platforms. Missing a deadline can result in immediate enforcement exposure.

| Deadline | Regulation / Requirement | Jurisdiction | Impact | Penalty for Non-Compliance |
|---|---|---|---|---|
| **Already in effect (as of March 2025)** | PCI DSS v4.0 mandatory compliance | Global | All entities storing/processing card data must comply with v4.0 | Card brand fines $5K-$100K/month; breach liability |
| **Already in effect** | FTC Click-to-Cancel Rule | US | Subscription services must make cancellation as easy as sign-up | Up to $50,120 per violation |
| **April 22, 2025** | COPPA Rule Amendments | US | New limits on school authorizations; enhanced data security for children's data | Up to $53,088 per violation |
| **June 28, 2025** | European Accessibility Act (EAA) enforcement | EU (all Member States) | Products and services must meet WCAG 2.1 AA accessibility standards | Varies by Member State (see Section 2) |
| **August 1, 2025** | EU AI Act -- Prohibited practices | EU | Prohibited AI practices (social scoring, real-time biometric ID in public spaces, etc.) become enforceable | Up to EUR 35M or 7% global turnover |
| **January 1, 2026** | California AB 2013 (GenAI Transparency Act) | California, US | Developers of GenAI must publish training data documentation | Enforcement by California AG |
| **February 1, 2026** | Colorado AI Act (SB 24-205) | Colorado, US | High-risk AI deployers must conduct impact assessments and provide transparency notices | Colorado AG enforcement |
| **Q1-Q2 2026** | Various US state AI laws (TX, IL updates) | Multiple US states | Varying AI transparency, disclosure, and impact assessment requirements | Varies by state |
| **August 2, 2026** | EU AI Act -- High-risk AI system requirements | EU | Full compliance required for high-risk AI systems including those in education | Up to EUR 15M or 3% global turnover |
| **October 2026** | DORA (Digital Operational Resilience Act) -- full enforcement | EU | ICT risk management for financial entities and their critical ICT service providers | Varies; supervisory authority enforcement |
| **July 2027** | EU AML Regulation (AMLR) | EU | New single rulebook for AML/CFT; expanded scope of obligated entities | Criminal liability; administrative fines |
| **2025-2026 (ongoing)** | DSA enforcement intensification | EU | Increased enforcement of DSA obligations for hosting services and online platforms | Up to 6% of worldwide annual turnover |
| **2025-2026 (ongoing)** | Russia: ORD advertising registration | Russia | All online advertising (including affiliates) must be registered and labeled | RUB 100K-500K per violation |

### How to Use This Table

1. **Identify which deadlines apply to your platform** based on your markets, features, and data practices.
2. **Work backwards from each deadline** to establish implementation timelines (most compliance projects take 3-12 months).
3. **Assign ownership** for each compliance workstream to a specific person or team.
4. **Set internal milestones** at 6 months, 3 months, and 1 month before each deadline.
5. **Budget for external counsel and auditors** where needed (particularly for PCI DSS, EU AI Act conformity assessment, and AML).

---

## Quick Reference: Risk Severity Matrix

| Trap | Likelihood of Trigger | Financial Exposure | Ease of Remediation |
|---|---|---|---|
| Free trial conversion violations | HIGH (especially CA, EU) | MEDIUM ($10K-$500K) | MEDIUM (disclosure changes + process) |
| Web accessibility lawsuits | HIGH (US); MEDIUM (EU from June 2025) | HIGH ($5K-$1M+ in US serial litigation) | HIGH EFFORT (full site remediation) |
| COPPA violations | HIGH (education platforms) | VERY HIGH ($50K-$275M) | HIGH EFFORT (consent system + data audit) |
| Testimonial / income claim violations | HIGH (education / coaching) | HIGH ($50K-$900M in FTC actions) | MEDIUM (marketing audit + disclosure) |
| Geoblocking violations | MEDIUM | MEDIUM (fines vary by Member State) | LOW (configuration changes) |
| Data portability non-compliance | LOW-MEDIUM (rising) | VERY HIGH (up to 4% global turnover) | MEDIUM (export feature development) |
| Affiliate program violations | HIGH | HIGH ($50K+ per violation) | MEDIUM (agreement + monitoring) |
| UGC liability exposure | MEDIUM | HIGH (loss of safe harbor = unlimited) | MEDIUM (notice-and-action system) |
| Pricing / VAT non-compliance | HIGH (cross-border SaaS) | VERY HIGH (retroactive VAT + penalties) | HIGH EFFORT (tax infrastructure) |
| AI in education non-compliance | MEDIUM (rising fast) | VERY HIGH (up to 7% turnover under AI Act) | VERY HIGH EFFORT (conformity assessment) |
| PCI DSS v4.0 non-compliance | HIGH (if storing cards) | HIGH (fines + breach liability) | MEDIUM (if using tokenization) |
| AML non-compliance | LOW-MEDIUM | VERY HIGH (criminal liability) | HIGH EFFORT (KYC/CDD systems) |

---

*This document should be reviewed quarterly and updated as regulations change. The next recommended review date is July 2026, ahead of the EU AI Act high-risk deadline.*
