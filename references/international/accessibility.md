# Web Accessibility Legal Requirements for SaaS

## Overview

Web accessibility is no longer just a best practice -- it is a legal requirement in most major markets. SaaS businesses face litigation risk in the US, mandatory compliance deadlines in the EU, and potential penalties across multiple jurisdictions. This reference covers the legal frameworks, standards, common failures, and practical compliance guidance.

---

## How This Risk Actually Works -- Read First

Accessibility does not behave like the other topics in this skill. Explain the mechanism before quoting any statute, because clients reason about it by analogy to GDPR and every conclusion they draw that way is wrong.

### 1. Two completely different regimes wear the same name

| | **US** | **EU** |
|---|---|---|
| Who enforces | **Nobody.** Private plaintiffs sue. | Market surveillance authority. |
| Is there a technical standard? | **No.** DOJ shelved Title III rulemaking Oct 2025. | Yes — EN 301 549, precise and citable. |
| How you find out | A demand letter or a complaint. | An audit or a complaint to the regulator. |
| Can you become "compliant"? | **No — there is no safe harbor.** | Yes, in the ordinary sense. |
| What it costs | Settlement + your own counsel, repeatedly. | Administrative fine, once. |

**The US absence of a rule is the risk, not relief from it.** A client who hears "DOJ dropped the rule" concludes they are safe; the correct reading is that there is no target to hit and therefore no way to end the exposure. 2025 was a record filing year *while* rulemaking was being withdrawn.

### 2. It is a litigation market with an economic model

Understand the plaintiff's business before advising the defendant:

1. A firm runs an automated scanner across thousands of sites.
2. The scanner output becomes the complaint. A named plaintiff with a real disability states they tried to buy and could not.
3. Defense costs more than settlement, so the defendant settles — typically **$5,000-$20,000** for a straightforward serial-plaintiff case, $10K-$100K+ where the site is bad or the business is larger.

Consequences that follow directly from this model, and that clients rarely anticipate:

- **Targets are chosen by scanner error count, not by company size.** Large firms have remediated, so the pool is now small and mid-size e-commerce. In 2025 the majority of e-commerce defendants had **under $25M revenue**.
- **Settling marks you as a payer.** 1,427 of 2025's filings hit companies already sued once.
- **Fixing the one page named in the letter is insufficient** — the next plaintiff scans the rest of the site. Always remediate the *class* of defect.

### 3. Jurisdiction follows the customers, not the incorporation

Where the entity is registered (UAE, Cyprus, BVI) is close to irrelevant. What matters is **where the buyers are, where fulfillment happens, and where payments are processed.** A foreign seller aimed at US consumers is a realistic target; the fight is over personal jurisdiction, and arguing it costs more than settling. Do not let a client treat an offshore entity as an accessibility shield — it is not one, in the same way it is not a CCPA or COPPA shield.

### 4. The obligation attaches to the store, not to the product

A frequent and expensive confusion. The law requires that a disabled user be able to **transact** — browse, configure, pay, get support. It does **not** require the product itself to be perceivable by every user. A blind customer need not be able to see the comic book, the photo print, or the film; they must be able to *buy* it. Applied to an audit, this means: forms, checkout, error messages and support channels are the exposure; inherently visual deliverables are not, and saying so in Known Limitations is legitimate.

### 5. What actually defends you is the record, not the document

Ranked by what moves outcomes:

1. **A dated, contemporaneous record** — audit reports, before/after screenshots, remediation log, testing dates. This is what separates "did nothing" from "has a program", and it is the main lever on settlement value.
2. **Real remediation of the underlying code.**
3. **A monitored feedback channel plus an alternative way to transact** (phone *and* email — different disabilities favour different channels). This resolves complaints before they become filings.
4. **A published statement and remediation plan** — worth only what items 1-3 are worth.

Procedural defenses exist but are situational, not a strategy: **standing** (plaintiff cannot show actual interference or genuine intent to return), **mootness** (site fully remediated, no reasonable expectation of recurrence — jurisdiction-dependent and rarely dispositive alone), and a **motion to stay** to remediate while capping fee exposure. Counsel with actual Title III volume experience picks among these; a generalist overpays.

### 6. Advice that is actively harmful

- ❌ "Install an overlay widget" — see the overlay section; it is a liability, and plaintiff firms screen for it.
- ❌ "Put up an accessibility statement saying you comply" — without a dated audit this creates two new claims (see the statement section).
- ❌ "There is no DOJ rule, so this is theoretical."
- ❌ "We are not a US company." — see point 3.
- ❌ "We passed the automated scan, so we are done." Automated tools catch roughly **30-40%** of issues; keyboard operation, focus order, and alt-text *quality* are only testable by hand.

---

## United States -- ADA Title III

### Legal Framework

The Americans with Disabilities Act (ADA) Title III prohibits discrimination by "places of public accommodation." While the ADA was enacted in 1990 (before the commercial internet), courts have increasingly interpreted Title III to cover websites and digital services.

### Litigation Landscape

**The risk driver in the US is private litigation, not agency enforcement.** There is no federal regulation requiring private websites to meet any technical standard, and none is coming in the near term (see "Regulatory status" below). This does not lower the risk — it *is* the risk model. Serial plaintiffs sue under a statute with no safe harbor, so there is nothing to "be compliant with" that ends the exposure.

2025 filing data (federal ADA website suits):

- **3,948 ADA website lawsuits filed in 2025**, up ~24% year over year. Counting state-court filings the total exceeds 5,000. Demand letters that settle pre-litigation are not counted anywhere and are believed to be a multiple of the filing number.
- **~69% of cases targeted online retailers.** E-commerce is the single most-targeted category.
- **The majority of e-commerce defendants had under $25M revenue.** Small D2C shops are the core target, not big brands.
- **Venue concentration**: New York ~1,108, Florida ~950, California ~787.
- **1,427 of 2025 filings targeted companies that had already been sued once** for web accessibility. Settling one case does not remove you from the target list — it confirms you as a payer.
- **Serial plaintiffs**: A small number of plaintiffs and firms file the bulk of cases ("surf-by" suits, by analogy to "drive-by" physical ADA suits). They screen sites with automated scanners; the complaint is usually generated from the scanner output.
- **Typical settlement costs**: **$10,000 to $100,000+** per case — legal fees (usually the largest component), plaintiff payment, an agreement to remediate, and 1-3 years of monitoring. Major brands and class actions reach $500K to several million.

### Regulatory status (as of mid-2026) — read this before telling a client "the DOJ requires X"

- **Title II rule (state/local government), April 2024**: DOJ set WCAG 2.1 AA as the technical standard for public entities. In **April 2026 DOJ extended the Title II compliance deadlines** via an interim final rule; the extension is being litigated. This rule has never applied to private businesses.
- **Title III (private businesses)**: DOJ **shelved digital-accessibility rulemaking in October 2025** and in November 2025 signalled it would revisit both Title II and Title III. **No Title III technical standard exists or is expected under the current administration.**
- **What this means practically**: the absence of a rule is not a defense and does not reduce litigation volume — 2025 was a record year *while* rulemaking was being withdrawn. Courts continue to apply WCAG as the yardstick because both sides' experts use it. Do not let a client read "DOJ dropped the rule" as "we are fine."

### Standard: WCAG 2.1 AA (moving to 2.2)

The ADA specifies no technical standard. **WCAG 2.1 Level AA** is the de facto benchmark via consent decrees, settlements, and expert testimony. **WCAG 2.2 AA** (W3C Recommendation, October 2023) adds nine success criteria and is the current version — target 2.2 for new work, but note that settlements and the DOJ Title II rule are still written to 2.1 AA. Conforming to 2.2 satisfies 2.1.

### Who is at Risk

- **Any business with a consumer-facing website** is potentially subject to ADA Title III. There is **no revenue or headcount threshold.**
- Highest-risk profile, in order: **consumer e-commerce with an online checkout** > education / healthcare / financial services > interactive dashboards and multimedia.
- **Foreign-domiciled sellers are not out of reach.** A non-US entity (UAE, EU, offshore) operating an e-commerce site aimed at US consumers, with US fulfillment or US payment processing, is a realistic target: the practical question is personal jurisdiction and cost of defense, not whether the ADA "applies abroad." Serial plaintiffs file first and let the defendant pay counsel to argue jurisdiction — which usually costs more than settling.

---

## United States -- State Law (this is where the money actually is)

Federal ADA Title III provides **injunctive relief and attorney's fees only — no damages**. The reason plaintiffs file volume suits is state law that stacks statutory damages on top.

### California -- Unruh Civil Rights Act (Cal. Civ. Code § 51)

- A 1992 amendment **incorporates the ADA by reference**, so **any ADA violation is a per-se Unruh violation** — the plaintiff does not have to prove disability discrimination independently.
- **Statutory damages of no less than $4,000 per violation**, with no requirement to prove actual harm. Courts have allowed up to treble actual damages, and "violation" can be pleaded per visit.
- This is why California is a primary venue despite ranking third by filing count: the per-visit math turns a scanner report into a five-figure demand.
- **Pending reform**: two bills would introduce "notice and cure" (a window to fix before damages attach), and a Second Appellate District panel heard argument on a related question in February 2026 with judges reportedly skeptical of the plaintiffs' position. **Nothing has passed — do not advise a client to rely on notice-and-cure.**

### New York

- **NY State Human Rights Law and NYC Human Rights Law** both reach public accommodations and allow **compensatory damages plus attorney's fees**; NYC HRL permits punitive damages.
- New York is the highest-volume federal venue (~1,108 filings in 2025), typically pleaded as ADA + NYSHRL + NYCHRL together so the plaintiff gets injunctive relief federally and damages under state law.

### Other states

- **Florida** (~950 filings in 2025) — mostly straight ADA Title III, no state damages analogue, but venue is plaintiff-friendly.
- **Colorado HB21-1110** — state and local government only, WCAG 2.1 AA, does not reach private business.
- A growing number of states have public-sector accessibility statutes. **Check for a private-sector damages statute before estimating exposure** — its presence or absence is what determines whether a demand letter is a $5K or a $50K problem.

---

## Accessibility Overlays and Widgets -- Treat as a Liability, Not a Fix

**Never recommend an accessibility overlay (accessiBe, UserWay, AudioEye widget mode, EqualWeb, and similar "one line of JavaScript" products) as a compliance measure.** This is now a documented legal trap, not a matter of opinion.

- **FTC v. accessiBe (announced January 2025, final order April 2025): $1,000,000.** The FTC alleged accessiBe falsely claimed its `accessWidget` would "automatically comply" with WCAG 2.1 AA. The complaint alleged the widget **created accessibility barriers** on sites where it was installed, and separately that accessiBe formatted paid third-party articles and reviews to look like independent opinion without disclosing the material connection.
- The final order **bars accessiBe from claiming its automated product makes any website WCAG-compliant, or keeps it compliant over time, absent supporting evidence.**
- **Consequences for the client, not just the vendor:**
  1. Overlays do not stop lawsuits. Sites running overlays are sued — plaintiff firms specifically screen for them, because the overlay is evidence the business knew about accessibility and chose a cosmetic fix.
  2. **Repeating the vendor's marketing claim on your own site is your own FTC §5 deception exposure**, not the vendor's. If the client's site says "we are WCAG 2.1 AA compliant" because the overlay vendor said so, the client owns that statement.
  3. Screen reader users and disability advocacy organizations actively campaign against overlays; several maintain public lists of sites using them.
- **Correct advice**: remediate the underlying HTML/CSS/JS. If the client has already bought an overlay, tell them it does not discharge the obligation and that any conformance language it generated must come off the site.

---

## European Union -- European Accessibility Act (EAA)

### Key Provisions

The European Accessibility Act (Directive (EU) 2019/882) establishes accessibility requirements for products and services across the EU.

### Deadline

- **June 28, 2025**: Member states must apply the requirements. All covered products and services placed on the market or provided after this date must comply.
- Products and services already on the market before June 28, 2025, have a transition period until June 28, 2030, but only for existing contracts. New features, updates, or substantial changes trigger immediate compliance requirements.

### Scope -- What's Covered

The EAA covers the following services (relevant to SaaS):

- **E-commerce services**: Any website or application used to sell products or services online. This includes SaaS checkout and purchase flows.
- **Banking and financial services**: Online banking, investment platforms, payment services.
- **Electronic communications**: VoIP, messaging, email services.
- **Audio-visual media services**: Streaming platforms, video hosting.
- **E-books and dedicated reading software**
- **Transport services**: Ticketing, check-in, real-time travel information.
- **Education platforms**: While "education" is not explicitly listed as a named category, educational services delivered through e-commerce platforms, or educational software provided as a product, are covered through other categories. Additionally, many member states have broader national accessibility laws covering education.

### Technical Standard: EN 301 549 (WCAG 2.1 AA today, 2.2 AA next) + PDF/UA

- The EAA references the harmonized European standard **EN 301 549**. The current published version, **v3.2.1, incorporates WCAG 2.1 Level AA** in full.
- **EN 301 549 v4.1.1 is expected to publish in 2026**, incorporating **WCAG 2.2 Level AA** and aligning more closely with the EAA. Once cited in the Official Journal it becomes the operative standard. **Build new work to WCAG 2.2 AA** so the client is not re-remediating in a year.
- **PDF/UA (ISO 14289-1)**: Any PDF documents published on accessible services must meet PDF/UA standards. This includes:
  - Terms of service
  - Privacy policies
  - Invoices
  - Reports or downloadable content
  - Course materials (for education platforms)

### Microenterprise Exemption

- **Microenterprises** (fewer than 10 employees AND annual turnover or balance sheet total not exceeding EUR 2 million) providing services are exempt from the EAA.
- This exemption does NOT apply to products -- only services.
- Member states may choose to narrow or eliminate this exemption.

### Country-Specific EAA Penalties

Each EU member state sets its own penalties for non-compliance with the EAA (within their national transposition legislation):

| Country | Penalty Range | Notes |
|---------|--------------|-------|
| **Cyprus** | EUR 1,000 -- 20,000 | Per violation |
| **Czech Republic** | Up to CZK 2,000,000 (~EUR 100,000) | Per violation, enforced by Czech Trade Inspection |
| **Finland** | Up to EUR 150,000 | Per violation; Market surveillance authority enforces |
| **Ireland** | Up to EUR 200,000 | Per violation; potential criminal penalties for serious breaches |
| **Netherlands** | Up to EUR 250,000 | Per violation; enforced by the Authority for Consumers and Markets |
| **Italy** | EUR 5,000 -- 150,000 | Per violation; AGID (Agenzia per l'Italia Digitale) and AGCM enforce |
| **Poland** | Up to PLN 1,000,000 (~EUR 200,000) | For severe violations; lower penalties for minor non-compliance |
| **Germany** | Not yet specified in detail | Enforcement through market surveillance; fines expected in line with other product safety penalties |
| **France** | Up to EUR 25,000 | Per violation for digital services; additional daily penalties possible |
| **Spain** | EUR 301 -- 1,000,000 | Tiered: minor (301-30K), serious (30K-150K), very serious (150K-1M) |

**Severe (repeated/systematic) violations**:
- Some member states impose significantly higher penalties for repeated or systematic non-compliance.
- **Poland**: Up to **EUR 1,000,000** for severe violations.
- **Spain**: Up to **EUR 1,000,000** for "very serious" violations.
- Market surveillance authorities can also order products/services to be withdrawn from the market.

---

## WCAG 2.1 Level AA -- Key Requirements

The Web Content Accessibility Guidelines (WCAG) 2.1 Level AA is the standard referenced by both US courts and the EU EAA. It is organized around four principles: Perceivable, Operable, Understandable, and Robust (POUR).

### Common Failures (and How to Fix Them)

#### 1. No Alt Text for Images (WCAG 1.1.1 -- Non-text Content)

**The problem**: Images without alt text are invisible to screen reader users.

**What fails**:
- Product screenshots with no alt attribute
- Icons used as buttons with no accessible label
- Decorative images that are not properly hidden from assistive technology
- Complex charts or infographics with no text alternative

**How to fix**:
- Add descriptive `alt` attributes to all meaningful images
- Use `alt=""` (empty alt) for decorative images so screen readers skip them
- For complex images (charts, diagrams), provide a detailed text description nearby or via a long description link
- For icon buttons, use `aria-label` or visually hidden text

#### 2. Poor Color Contrast (WCAG 1.4.3 -- Contrast Minimum)

**The problem**: Text that does not have sufficient contrast against its background is difficult or impossible to read for users with low vision or color blindness.

**WCAG 2.1 AA requirements**:
- **Normal text**: Contrast ratio of at least **4.5:1**
- **Large text** (18pt+ or 14pt+ bold): Contrast ratio of at least **3:1**
- **UI components and graphical objects**: Contrast ratio of at least **3:1** against adjacent colors (WCAG 1.4.11)

**Common offenders**:
- Light gray text on white backgrounds
- Placeholder text in form fields (often fails contrast)
- Colored buttons with white text where the color is too light
- Links that are only distinguished from surrounding text by color (also need underline or other non-color indicator)

**How to fix**:
- Use a contrast checker tool (built into browser dev tools, or use WebAIM Contrast Checker)
- Establish accessible color palettes in your design system
- Test with grayscale view to ensure information is not conveyed by color alone

#### 3. No Keyboard Navigation (WCAG 2.1.1 -- Keyboard)

**The problem**: Users who cannot use a mouse (motor disabilities, screen reader users) must be able to operate all functionality using only a keyboard.

**What fails**:
- Custom dropdown menus that only open on mouse hover
- Modal dialogs that cannot be closed with Escape key
- Interactive elements (sliders, drag-and-drop) with no keyboard alternative
- Focus traps (focus gets stuck in a component with no way to leave)
- No visible focus indicator (users cannot see where they are on the page)

**How to fix**:
- Ensure all interactive elements are reachable via Tab key
- Provide visible focus styles (`:focus-visible` CSS)
- Implement keyboard event handlers for custom components
- Test by navigating your entire site using only Tab, Shift+Tab, Enter, Space, Escape, and Arrow keys

#### 4. Inaccessible Forms (WCAG 1.3.1, 3.3.1, 3.3.2, 4.1.2)

**The problem**: Forms are where users perform critical actions (sign up, purchase, enter data). Inaccessible forms block users completely.

**What fails**:
- Form fields without associated `<label>` elements
- Error messages that are not programmatically associated with the field or not announced by screen readers
- Required fields not indicated (or only indicated by color)
- CAPTCHA with no accessible alternative
- Custom form controls (date pickers, autocomplete) that are not accessible

**How to fix**:
- Use `<label>` elements with `for` attribute matching the input `id`
- Use `aria-describedby` to associate error messages and help text with form fields
- Mark required fields with `aria-required="true"` and visible indicators
- Use `aria-invalid="true"` when a field has an error
- Provide accessible CAPTCHA alternatives (e.g., hCaptcha accessible mode, audio CAPTCHA)
- Test forms with a screen reader (NVDA, VoiceOver, JAWS)

#### 5. Missing Page Structure (WCAG 1.3.1 -- Info and Relationships)

**What fails**:
- Pages with no heading hierarchy (or incorrect heading hierarchy -- jumping from h1 to h4)
- Data tables without proper `<th>` elements and scope attributes
- Lists not marked up as `<ul>`/`<ol>`/`<li>`
- Navigation not marked up with `<nav>` element
- Regions not identified with landmarks (header, main, footer, aside)

#### 6. Missing or Inadequate Captions and Transcripts (WCAG 1.2.2, 1.2.4)

**What fails**:
- Videos without captions
- Live audio/video without live captions
- Audio content without transcripts

---

## Automated Testing Tools

Automated tools catch approximately 30-40% of accessibility issues. Manual testing is required for the remainder. However, automated testing is an essential first line of defense.

### axe (Deque Systems)

- **What it is**: The most widely used accessibility testing engine. Available as:
  - Browser extension (axe DevTools for Chrome, Firefox, Edge)
  - CLI tool (`@axe-core/cli`)
  - Library for integration into CI/CD (`axe-core` npm package)
  - API for automated testing (`@axe-core/playwright`, `@axe-core/puppeteer`)
- **What it tests**: 80+ WCAG 2.1 rules, including alt text, color contrast, form labels, keyboard accessibility, ARIA usage
- **Strengths**: Very low false positive rate. Industry standard. Free core engine.
- **Limitations**: Cannot test keyboard navigation flows, cannot assess alt text quality (only presence), cannot test complex interaction patterns.

### Google Lighthouse

- **What it is**: Built into Chrome DevTools (Audits tab). Also available as a CLI tool and CI integration.
- **What it tests**: Includes an accessibility audit section powered by axe-core. Also tests performance, SEO, and best practices.
- **Strengths**: Free, easy to use, provides an accessibility score (0-100). Good for quick checks.
- **Limitations**: Only tests the current state of the page (does not interact with dynamic content). Accessibility score can be misleading -- a score of 100 does not mean the site is fully accessible. Tests a subset of WCAG rules.

### WAVE (WebAIM)

- **What it is**: Web accessibility evaluation tool from WebAIM. Available as:
  - Online tool (wave.webaim.org -- paste a URL)
  - Browser extension (Chrome, Firefox)
  - API for automated testing
- **What it tests**: Similar rules to axe, plus visual indicators overlaid on the page showing errors, alerts, and structural elements.
- **Strengths**: Visual presentation makes it easy to locate issues on the page. Distinguishes between errors (definite problems) and alerts (potential problems needing manual review).
- **Limitations**: Same general limitations as other automated tools -- cannot fully assess dynamic content or interaction patterns.

### Additional Tools

- **Pa11y**: Open-source automated accessibility testing tool. Good for CI/CD integration.
- **Tenon**: Cloud-based accessibility testing API.
- **SortSite**: Comprehensive site-wide accessibility and quality checker.
- **Screen readers for manual testing**: NVDA (free, Windows), VoiceOver (free, macOS/iOS), JAWS (paid, Windows), TalkBack (free, Android).

---

## The Accessibility Statement -- When It Helps, When It Hurts

A public "Accessibility" / "Accessibility Statement" page is one of the few legal documents where **a badly drafted version is worse than no version at all.** Handle it as drafting, not as a checkbox.

### Is it legally required?

| Jurisdiction | Statement required? | Basis |
|---|---|---|
| **US -- ADA Title III** | **No.** No federal law requires a private business to publish an accessibility statement. | No Title III regulation exists at all (see Regulatory status above). |
| **US -- state law (Unruh, NYSHRL/NYCHRL)** | **No.** These create damages for inaccessibility; none mandates a statement. | — |
| **EU -- EAA (Directive 2019/882)** | **Yes**, for covered services. The service provider must publish accessibility information — how the service meets the requirements, and (per national transposition) a complaints/enforcement route. | EAA Art. 13 + Annex V; national transposition varies. |
| **EU/UK -- public sector** | **Yes**, and the form is prescribed. | Web Accessibility Directive 2016/2102; UK PSBAR 2018. |
| **EAA microenterprise** | Exempt from EAA **service** obligations: fewer than 10 employees **AND** turnover or balance sheet ≤ EUR 2M. Exemption does **not** cover products, and member states may narrow it. | EAA Art. 4(5). |

**So for a US-only business the page is optional.** Recommend it on *practical* grounds, and be honest with the client that it is not a compliance gap the way a missing privacy policy is.

### What it actually buys you (US)

- **A documented feedback channel.** Some plaintiff firms and their screeners deprioritize sites that offer a monitored, responsive accessibility contact — a user who gets a real answer is a user who does not become a named plaintiff.
- **Good-faith evidence at settlement.** A dated statement plus dated audit records plus a remediation plan is the standard package that moves settlement numbers down. The statement alone does essentially nothing; **it is only worth what the underlying work is worth.**
- **It genuinely helps disabled users**, which is the point and also the best litigation defense.

**What it does not buy you:** immunity. A statement does not prevent a suit, is not a safe harbor, and is not a defense on the merits.

### The overpromise trap -- the main thing to get right

**Never publish a conformance claim the client cannot evidence.** "This site is WCAG 2.1 AA compliant" / "fully accessible" / "ADA compliant" on an unaudited site is:

1. **A gift to a plaintiff.** It is an admission of the applicable standard, and the scanner output becomes proof of breach against your own stated benchmark. You have removed the argument about what standard applies.
2. **An independent FTC §5 deception exposure** — an unsubstantiated objective claim to consumers. This is precisely the theory behind the $1M accessiBe order; nothing in that theory is limited to vendors.
3. **Potentially a state UDAP claim**, which in several states carries its own statutory damages and fee-shifting.

**Rule: the statement's conformance language must never be stronger than the client's last dated audit.** If there is no audit, there is no conformance claim.

### Two drafting patterns

**Pattern A -- US, no completed audit (the defensive statement).** Commitment and process language only, no conformance claim. This is what most competent US D2C sites publish, and it is the correct default:

- *Our commitment* — plain-language statement that accessibility matters and is part of ongoing development. No standard named as achieved.
- *Our efforts* — accessibility is considered as part of the regular development process. Hedged verbs throughout: "we work to", "where practical and feasible", "we make ongoing efforts". **Avoid "we ensure", "we guarantee", "fully", "all".**
- *Known limitations* — name the genuinely hard areas honestly (third-party embeds, interactive builders, user- or AI-generated imagery, PDFs). **This section is protective:** disclosed limitations are much harder to characterize as concealment, and it pre-empts the "they claimed accessibility while knowing otherwise" framing.
- *Feedback and assistance* — a real monitored email address, plus an offer of an alternative way to get the same service (phone/email ordering assistance). **The alternative-access offer is the single most useful line in the document** and is often what resolves a demand letter.
- *Continuous improvement* — statement is reviewed and may be updated as the service evolves.
- *Last updated: [Month Year]* — and it must be true. A statement dated three years ago is worse than none.

**Pattern B -- audit completed, or EU/EAA in scope.** Now you may make a scoped conformance claim, and under the EAA you must say more:

- Named standard and level, **scoped and dated**: "conforms to WCAG 2.2 Level AA, based on an audit of [pages/flows] completed [date]." Never unscoped, never undated.
- **Non-conformances listed explicitly**, with reason and target remediation date.
- Evaluation method (self-assessment vs. third-party audit — say which, and name the auditor if third-party).
- **(EAA)** The complaints procedure and the national enforcement authority the user may escalate to.
- Review cadence, and a commitment to re-date after each review.

### Audit questions to ask about an existing statement

1. Does it claim conformance? If yes — **is there a dated audit backing it?** If not, that language comes off today.
2. Is the "last updated" date real and recent? A stale date evidences abandonment of the stated process.
3. Is the contact address **actually monitored**? Send a test message. An unanswered accessibility inbox converts a good-faith document into evidence of bad faith.
4. Is there an alternative-access route for users who cannot complete the flow?
5. Does the site run an **overlay**, and did the overlay generate conformance language? Both come off.
6. Is the statement page **itself** accessible, and is it linked from every page (footer)? A statement reachable only from the homepage is a bad look in a complaint.

---

## If a Demand Letter or Complaint Arrives -- First Steps

Order matters here, and the first instinct is usually the wrong one.

1. **Do not remediate silently and say nothing, and do not delete or alter the site before preserving its state.** Capture the current state (scanner reports, screenshots, HTML archive) and preserve it. Spoliation arguments are avoidable and expensive.
2. **Do not respond substantively without counsel.** Anything conceding the standard or the barrier will be quoted back. Acknowledge receipt only.
3. **Retain counsel with actual ADA Title III experience** — this is a volume practice with known plaintiff firms and known settlement ranges; a generalist will overpay.
4. **Run a real audit immediately** (axe + manual keyboard/screen-reader pass on the flows named in the letter). You need to know whether the alleged barriers are real before negotiating. Scanner-generated complaints frequently allege issues that do not reproduce.
5. **Start remediation of anything genuinely broken, and date every step.** Mootness arguments are jurisdiction-dependent and rarely dispositive, but a documented remediation record is the strongest lever on settlement value.
6. **Fix the class of defect, not the specific page cited.** A repeat suit against the same defendant is common (1,427 of 2025's filings), and the second plaintiff will scan the rest of the site.
7. **Only then revisit the statement** — updated, dated, and matching what the audit actually found.

---

## Practical Compliance Checklist for SaaS Sites

### Immediate Actions

- [ ] **Run an automated audit**: Use axe DevTools or WAVE on your homepage, login page, main dashboard, pricing page, checkout flow, and key feature pages. Fix all errors.
- [ ] **Check color contrast**: Verify all text meets 4.5:1 (normal) or 3:1 (large) contrast ratios. Pay special attention to: placeholder text, button text, link text, error messages, and disabled state text.
- [ ] **Add alt text to all images**: Audit every image on your site. Meaningful images get descriptive alt text. Decorative images get `alt=""`.
- [ ] **Test keyboard navigation**: Navigate your entire site using only a keyboard. Every interactive element must be reachable and operable. Focus must be visible at all times.
- [ ] **Label all form fields**: Every input must have an associated `<label>`. Every error message must be programmatically linked to its field.

### Structural Improvements

- [ ] **Implement proper heading hierarchy**: One `<h1>` per page, logical descending structure (h1 > h2 > h3), no skipped levels.
- [ ] **Add landmark roles**: Use `<header>`, `<nav>`, `<main>`, `<aside>`, `<footer>` semantic elements. For single-page apps, ensure landmarks are present and meaningful.
- [ ] **Add skip navigation link**: A "Skip to main content" link as the first focusable element on every page.
- [ ] **Ensure accessible modals/dialogs**: Focus must be trapped within open modals, Escape key must close them, focus must return to the trigger element when closed.
- [ ] **Make data tables accessible**: Add `<th>` with `scope` attributes, `<caption>` elements, and `aria-describedby` for complex tables.

### Content and Media

- [ ] **Add captions to all videos**: Both pre-recorded and live. Use professional captioning services for accuracy (auto-generated captions alone do not meet WCAG requirements).
- [ ] **Provide transcripts for audio content**: Podcasts, audio tutorials, webinars.
- [ ] **Make PDFs accessible**: All downloadable PDFs must meet PDF/UA standards (especially for EU EAA compliance). Use tagged PDFs with proper reading order, alt text for images, and bookmarks for navigation.
- [ ] **Ensure animations respect prefers-reduced-motion**: Users who set this OS preference should not see animations, auto-playing carousels, or parallax effects.

### Ongoing Processes

- [ ] **Integrate automated testing into CI/CD**: Run axe-core tests on every build. Fail the build if new accessibility errors are introduced.
- [ ] **Conduct manual testing quarterly**: Have a team member (or hire an accessibility consultant) manually test key flows with a screen reader.
- [ ] **User testing with disabled users**: At least annually, conduct usability testing with actual users who have disabilities.
- [ ] **Publish an accessibility statement** — see "The Accessibility Statement" section above for drafting. **Do not name a conformance standard unless a dated audit supports it**; without one, use the defensive pattern (commitment + known limitations + monitored contact + alternative access + real date).
- [ ] **Never install an accessibility overlay/widget as a remediation measure**, and remove any conformance language one has generated (see the overlay section above).
- [ ] **Train your development team**: Ensure designers and developers understand accessibility principles. Include accessibility in code review checklists.
- [ ] **Keep a dated accessibility record — this is the single highest-value defensive artifact.** Not a folder of good intentions: a running log with dates. Each entry = date, what was tested, tool/method, what was found, what was fixed, commit or ticket reference. Keep before/after screenshots and raw scanner output. A client with 18 months of this settles far cheaper than one without, and it is the difference between "has a program" and "did nothing."
- [ ] **Offer an alternative way to transact** — a monitored phone number **and** email through which a user can place an order or get help completing one. Different disabilities favour different channels, so offer both. This is frequently what resolves a complaint before it becomes a filing, and it is cheap.
- [ ] **Re-scan after every significant release.** Accessibility regresses silently; a site audited once and shipped against for a year is un-audited.

### Priority Order for SaaS Sites

If resources are limited, prioritize accessibility fixes in this order:

1. **Authentication flows** (login, signup, password reset) -- users cannot use your product if they cannot log in
2. **Core product functionality** (the main features users pay for)
3. **Checkout and payment** (cannot convert if checkout is inaccessible)
4. **Marketing pages and landing pages** (legal exposure from ADA lawsuits)
5. **Help and support** (documentation, knowledge base, contact forms)
6. **Settings and account management**
7. **Secondary features and edge cases**

---

## Key Compliance Dates

| Jurisdiction | Regulation | Deadline | Standard |
|-------------|-----------|----------|----------|
| **US** | ADA Title III (private) | Already enforceable via private suit; **no technical regulation exists**, Title III rulemaking shelved Oct 2025 | WCAG 2.1 AA (de facto, via settlements/experts) |
| **US -- CA** | Unruh Civil Rights Act § 51 | Already enforceable | ADA incorporated by reference; **≥ $4,000 statutory damages per violation** |
| **US -- NY** | NYSHRL + NYCHRL | Already enforceable | Compensatory damages + fees; NYC allows punitive |
| **US** | ADA Title II (state/local gov only) | April 2024 rule; **deadlines extended April 2026**, under litigation | WCAG 2.1 AA |
| **EU** | European Accessibility Act | **June 28, 2025** (existing contracts transition to June 28, 2030) | EN 301 549 v3.2.1 (WCAG 2.1 AA + PDF/UA); **v4.1.1 w/ WCAG 2.2 AA expected 2026** |
| **UK** | Equality Act 2010 + Public Sector Bodies Accessibility Regulations 2018 | Already enforceable (public sector); Equality Act ongoing for private sector | WCAG 2.1 AA |
| **Canada** | Accessible Canada Act + provincial laws | Phased implementation through 2040 | WCAG 2.1 AA |
| **Australia** | Disability Discrimination Act 1992 | Already enforceable | WCAG 2.1 AA (referenced in DDA guidance) |
