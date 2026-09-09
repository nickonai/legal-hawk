# ePrivacy Directive & Cookie Compliance for SaaS

> **Directive 2002/58/EC** (ePrivacy Directive), as amended by **Directive 2009/136/EC** (Cookie Directive)
> Transposed into national law by each EU/EEA member state
> Supplemented by GDPR for consent requirements
> Planned replacement: **ePrivacy Regulation** (still in legislative process)

---

## 1. Cookie Categories

Understanding cookie categories is essential for implementing proper consent. The classification determines whether consent is required.

### Category 1: Strictly Necessary / Essential Cookies
**No consent required.**

| Purpose | Examples |
|---|---|
| Session management | Session ID cookies |
| Authentication | Login state cookies |
| Security | CSRF tokens, fraud prevention |
| Load balancing | Server routing cookies |
| User preferences stored at user request | Language selection (if explicitly chosen by user) |
| Shopping cart | Cart contents for current session |
| Cookie consent preferences | Storing the user's consent choice itself |

**Key rule**: a cookie is only "strictly necessary" if the service **explicitly requested by the user** cannot function without it. Internal business needs (analytics, A/B testing) do not qualify.

### Category 2: Preference / Functionality Cookies
**Consent required.**

| Purpose | Examples |
|---|---|
| Language preference (auto-detected) | Locale cookies not explicitly set by user |
| UI customisation | Theme, layout, font size |
| Region/country | Auto-detected geo preferences |
| Remembering form inputs | Autofill of non-essential fields |
| Video player preferences | Volume, quality settings |

### Category 3: Analytics / Statistics Cookies
**Consent required** (with nuances).

| Purpose | Examples |
|---|---|
| Page view counting | Google Analytics, Matomo, Plausible |
| Session recording | Hotjar, FullStory, LogRocket |
| A/B testing | Optimizely, VWO, Google Optimize |
| Performance monitoring | Core Web Vitals tracking |
| Heatmaps | Click/scroll tracking |
| Conversion tracking | Funnel analysis |

**Nuance -- some DPAs allow exemption for privacy-friendly analytics:**
- France (CNIL): exempts strictly audience-measurement cookies if: data is anonymised, used only for aggregated statistics, no cross-site tracking, users are informed, and opt-out is available. Matomo (self-hosted, anonymised) can qualify.
- Germany (DSK): generally requires consent for all analytics.
- Most DPAs: require consent for Google Analytics and similar third-party tools.

### Category 4: Marketing / Advertising Cookies
**Consent always required.**

| Purpose | Examples |
|---|---|
| Behavioural advertising | Google Ads remarketing, social media ad pixels |
| Retargeting | AdRoll, Criteo |
| Social media tracking | Social network Like buttons, share widgets |
| Cross-site tracking | Third-party ad network cookies |
| Interest-based profiling | DMP cookies |
| Affiliate tracking | Commission tracking cookies |
| Email marketing pixels | Tracking email opens/clicks |

---

## 2. Consent Requirements

### Core principles (Art. 5(3) ePrivacy Directive + GDPR Art. 4(11), 7):

**Consent must be:**

| Requirement | What it means in practice |
|---|---|
| **Prior** | Obtained BEFORE cookies are set (no "implied consent" by browsing) |
| **Informed** | User knows what cookies do, who uses the data, for how long |
| **Specific** | Separate consent for each purpose/category |
| **Freely given** | Genuine choice; no cookie walls blocking essential content |
| **Unambiguous** | Clear affirmative action (click, toggle); NOT inferred from inaction |
| **Granular** | User can accept some categories and reject others |
| **Easy to withdraw** | Revoking consent must be as easy as giving it |
| **Documented** | Record when, how, and what the user consented to |

### What is NOT valid consent:
- Scrolling or continuing to browse.
- Pre-ticked checkboxes.
- "By using this site you agree to cookies" banners with no action button.
- Only offering an "Accept" button (no reject option).
- Bundling cookie consent with Terms of Service acceptance.
- Cookie walls that completely block access (debated -- most DPAs consider these non-compliant).

---

## 3. No Pre-Ticked Boxes, No Dark Patterns

### CJEU Planet49 ruling (C-673/17):
- Confirmed that **pre-ticked boxes do not constitute valid consent**.
- Consent must be indicated by **active behaviour**.
- Applies to all types of cookies (including analytics).

### Dark patterns to avoid:

| Dark Pattern | Description | Why Non-Compliant |
|---|---|---|
| **Pre-ticked boxes** | Categories enabled by default | Not an affirmative act |
| **Asymmetric buttons** | "Accept All" is prominent, "Reject" is hidden/grey | Not freely given |
| **Hidden reject option** | Reject buried in settings, Accept on main banner | Not as easy to reject as to accept |
| **Confusing language** | "Personalise" instead of "Reject non-essential" | Not informed |
| **Forced consent** | Cookie wall blocking access entirely | Not freely given |
| **Misleading toggle colours** | Green = off, Red = on (reversed) | Not unambiguous |
| **Confirm-shaming** | "No, I don't want a better experience" | Manipulative, not freely given |
| **Repeated prompts** | Re-asking after rejection | Not respecting withdrawal/refusal |
| **Fake X button** | Close button that accepts all cookies | Not an affirmative act |

### Best practice for button design:
- "Accept All" and "Reject All" buttons must be **equally prominent** (same size, colour, visibility).
- A "Manage Preferences" option should be available on the first layer.
- CNIL (France) and EDPB guidelines are particularly strict on this.

---

## 4. Periodic Renewal

### When to re-ask for consent:
- No universal fixed period -- depends on jurisdiction and DPA guidance.
- **CNIL (France)**: recommends re-consent every **6 months** maximum.
- **ICO (UK)**: does not specify a fixed period but says consent should be "refreshed at appropriate intervals."
- **General best practice**: **6-12 months** is the accepted range.

### Triggers for re-consent:
- New cookie categories or purposes added.
- New third-party processors added.
- Significant changes to data processing.
- Changes in the cookies/trackers used.
- Expiry of the consent cookie itself.

### Consent record retention:
- Keep records of consent for the duration of processing + a reasonable period after.
- Records should include: timestamp, scope (which categories), method (banner interaction), version of the consent notice.

---

## 5. Cookie Banner Best Practices

### Layer 1 -- Initial Banner:
- Brief description of cookie use.
- List cookie categories (or summarise).
- **"Accept All"** button.
- **"Reject All"** button (equally prominent).
- **"Manage Preferences"** / "Customise" link/button.
- Link to full Cookie Policy.
- No cookies set until user acts (except strictly necessary).

### Layer 2 -- Preference Centre:
- Toggle for each category: essential (locked on), preferences, analytics, marketing.
- Brief description of each category.
- List of specific cookies per category (or link to full list).
- **"Save Preferences"** button.
- **"Accept All"** and **"Reject All"** buttons still available.

### Layer 3 -- Cookie Policy:
- Full list of cookies: name, provider, purpose, type, duration.
- Explanation of each category.
- How to manage cookies in browser settings.
- How to withdraw consent.
- Link back to consent manager to change preferences.

### Technical implementation:
- **Block scripts until consent** -- use tag manager consent mode or manual blocking.
- No cookies (except essential) set on page load before consent.
- Google Consent Mode v2 integration if using Google services.
- Consent signal should propagate to all tags/scripts.
- IAB Transparency & Consent Framework (TCF 2.2) for programmatic advertising.

### Accessibility:
- Banner must be keyboard-navigable.
- Screen reader compatible.
- Sufficient colour contrast.
- Must not block essential page functionality.

---

## 6. Popular Consent Management Platforms (CMPs)

| CMP | Key Features | Pricing | Notes |
|---|---|---|---|
| **Cookiebot (Usercentrics)** | Auto-scanning, TCF 2.2, GPC, multi-language, Google CMP partner | Free up to 50 pages; paid plans from ~EUR 9/mo | Strong EU compliance focus |
| **OneTrust** | Enterprise-grade, cookie scanning, preference centre, DSR management | Enterprise pricing (custom quotes) | Comprehensive privacy platform |
| **Osano** | Simple setup, automatic blocking, consent analytics | Free tier available; paid from ~$199/mo | Focus on ease of use |
| **CookieYes** | Affordable, auto-scanning, GDPR/CCPA, Google CMP partner | Free tier; paid from ~$10/mo | Good for small-medium SaaS |
| **Iubenda** | Cookie solution + privacy policy generator, TCF 2.2 | Free tier; paid from ~$29/yr | All-in-one legal compliance |
| **Termly** | Cookie consent + policy generator | Free tier; paid from ~$10/mo | Budget-friendly |
| **Didomi** | Enterprise CMP, TCF 2.2, high customisation | Custom pricing | Strong in publishing/media |
| **Sourcepoint** | TCF 2.2, CMP + messaging platform | Custom pricing | Ad-tech focused |

### Choosing a CMP -- evaluation criteria:
- [ ] Supports **TCF 2.2** (if running programmatic ads).
- [ ] Is a **Google-certified CMP** (required for Google Ads/Analytics consent mode).
- [ ] Auto-scans and classifies cookies.
- [ ] Blocks scripts before consent (not just records consent).
- [ ] Supports **GPC (Global Privacy Control)** signals.
- [ ] Multi-language support.
- [ ] Provides consent logging and proof.
- [ ] Customisable design (match your brand).
- [ ] Accessible (WCAG 2.1 AA).
- [ ] Handles regional variations (show different banners per jurisdiction).

---

## 7. Country-Specific Variations

### Germany (stricter)
- **Telekommunikation-Telemedien-Datenschutz-Gesetz (TTDSG)** s.25: explicit consent required for all non-essential cookies.
- No exemption for analytics cookies.
- German DPAs (DSK) take a strict approach -- reject button must be as easy as accept.
- Active enforcement: Planet49 case originated in Germany.
- Google Analytics: multiple German DPAs have declared standard GA implementations non-compliant.

### France (CNIL -- strict with detailed guidance)
- CNIL guidelines of 1 October 2020: "Reject All" must be as prominent as "Accept All."
- **6-month maximum** consent validity recommended.
- Audience measurement cookies can be exempt under specific conditions (aggregated, no cross-site, anonymous, opt-out available).
- CNIL has issued significant fines for cookie violations (Google: EUR 150M; a major social network: EUR 60M in 2022).

### Belgium
- Belgian DPA issued a landmark ruling against IAB Europe's TCF (2022).
- Strict on legitimate interest for cookies -- consent is the expected basis.

### Italy (Garante)
- Cookie guidelines of June 2021: first-layer banner must include reject option.
- Consent records must be maintained.
- Scrolling is not consent.
- Re-consent after 6 months.

### Spain (AEPD)
- Guide on cookies (2020 update): consent required for analytics.
- Cookie wall guidance: generally not acceptable.
- Cookie information must be in Spanish for Spanish-targeted services.

### Netherlands (AP)
- Strict on analytics cookies requiring consent.
- Fined companies for tracking cookies without consent.
- Clear guidance that "continue browsing" is not consent.

### Austria
- Telecom Act (TKG 2021) s.165: consent required for non-essential cookies.
- Austrian DPA follows EDPB guidelines closely.

### Ireland (DPC)
- Important as lead supervisory authority for many Big Tech companies.
- Cookie guidance aligns with EDPB.
- Enforcement primarily through GDPR rather than national ePrivacy transposition.

### Poland
- Telecommunications Law Art. 173: consent required for cookies.
- UODO guidance follows EDPB position.
- Less active enforcement on cookies specifically.

### Nordics (Sweden, Denmark, Finland, Norway)
- Generally follow EDPB guidance.
- Moderate enforcement intensity on cookies.
- Some flexibility on analytics if anonymised.

---

## 8. Practical Decision Guide

### Do I need consent for this cookie/tracker?

```
Is it a cookie, pixel, fingerprint, local storage, or similar technology
that accesses or stores info on the user's device?
  |
  YES --> Is it STRICTLY NECESSARY for the service
  |       explicitly requested by the user?
  |         |
  |         YES --> No consent needed (but must still inform in cookie policy)
  |         |
  |         NO --> CONSENT REQUIRED before setting
  |
  NO --> Not covered by ePrivacy (but may still need GDPR basis
         if processing personal data server-side)
```

### Quick reference -- common tools and consent:

| Tool/Service | Consent Required? |
|---|---|
| Session cookie (auth) | No -- strictly necessary |
| CSRF token | No -- strictly necessary |
| Cookie consent preference | No -- strictly necessary |
| Google Analytics (standard) | **Yes** |
| Google Analytics (anonymised IP, no cross-site) | **Yes** (possible exemption in France only under strict conditions) |
| Matomo (self-hosted, anonymised, no cross-site) | **Yes** in most countries; possible exemption in France |
| Plausible Analytics (cookieless) | **No** -- does not use cookies (but check if any local storage/fingerprinting occurs) |
| Social media ad pixels | **Yes** |
| Google Ads remarketing | **Yes** |
| Hotjar / FullStory | **Yes** |
| Intercom chat widget | **Likely yes** (sets tracking cookies; core chat functionality may be essential) |
| Stripe (payment) | **No** -- strictly necessary for payment processing |
| reCAPTCHA | Debated -- Google sets cookies; best practice is consent or use alternatives |
| YouTube embeds | **Yes** (use youtube-nocookie.com domain to reduce but not eliminate tracking) |
| Social share buttons with tracking | **Yes** |
| Language/locale (auto-detected) | **Yes** (unless user explicitly selected) |

---

## 9. Compliance Checklist

- [ ] **Audit all cookies and trackers** on your SaaS application (use CMP scanner or browser dev tools).
- [ ] **Classify each cookie** into the correct category (essential, preferences, analytics, marketing).
- [ ] **Implement a CMP** that blocks non-essential cookies before consent.
- [ ] **Design the banner** with equally prominent Accept and Reject buttons.
- [ ] **No pre-ticked boxes** in the preference centre.
- [ ] **Granular toggles** for each category (essential locked on).
- [ ] **Publish a Cookie Policy** with a complete cookie list (name, provider, purpose, type, duration).
- [ ] **Log consent** with timestamp, scope, and version.
- [ ] **Enable consent withdrawal** -- accessible link/button to re-open preferences.
- [ ] **Set consent expiry** (6-12 months) and re-prompt.
- [ ] **Honour GPC signals** where applicable (CCPA/CPRA, some EU guidance).
- [ ] **Implement Google Consent Mode v2** if using Google services.
- [ ] **Test across jurisdictions** -- show appropriate banner based on user location.
- [ ] **Review when adding new tools** -- any new third-party script may introduce new cookies.
- [ ] **Ensure accessibility** -- banner is keyboard-navigable and screen-reader compatible.
