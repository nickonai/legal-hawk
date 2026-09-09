# GDPR Key Requirements for SaaS Companies

> **Regulation (EU) 2016/679 -- General Data Protection Regulation**
> Effective: 25 May 2018 | Applies to: any entity processing personal data of EU/EEA residents

---

## 1. Territorial Scope (Art. 3)

GDPR applies to a SaaS company if **any** of these is true:

- The company is established in the EU/EEA.
- The company offers goods or services to individuals in the EU/EEA (even for free).
- The company monitors the behaviour of individuals in the EU/EEA (analytics, profiling, tracking).

A SaaS product accessible from the EU with no geo-blocking is almost certainly in scope.

---

## 2. Lawful Bases for Processing (Art. 6)

Every processing activity must rely on **exactly one** lawful basis. Choose carefully -- you cannot switch later without re-assessment.

| # | Lawful Basis | Typical SaaS Use Case |
|---|---|---|
| a | **Consent** | Marketing emails, analytics cookies, third-party tracking |
| b | **Performance of a contract** | Providing the SaaS service itself to a paying customer |
| c | **Legal obligation** | Tax record retention, anti-money-laundering checks |
| d | **Vital interests** | Rarely applicable in SaaS (emergency/health scenarios) |
| e | **Public interest / official authority** | Almost never applicable for commercial SaaS |
| f | **Legitimate interest** | Fraud prevention, security logging, basic analytics (requires LIA) |

### Consent Requirements (Art. 7)
- Must be **freely given, specific, informed, unambiguous**.
- Obtained by a **clear affirmative act** (no pre-ticked boxes).
- Must be as easy to **withdraw** as to give.
- Must be **recorded** with timestamp, scope, and method.
- Separate consent for each distinct purpose.
- For children: parental consent required (age threshold 13-16 depending on member state).

### Legitimate Interest Assessment (LIA)
1. Purpose test: identify the legitimate interest.
2. Necessity test: is processing necessary for that purpose?
3. Balancing test: does the interest override data subjects' rights/freedoms?
4. Document the outcome and keep it on file.

---

## 3. Privacy Policy -- Mandatory Contents (Art. 13 & 14)

A GDPR-compliant privacy policy **must** include:

- [ ] Identity and contact details of the **controller** (company name, address, email).
- [ ] Contact details of the **DPO** (if appointed).
- [ ] **Purposes** of processing and the **lawful basis** for each.
- [ ] If relying on legitimate interest: describe the interest.
- [ ] **Categories of personal data** collected.
- [ ] **Recipients** or categories of recipients (sub-processors, third parties).
- [ ] Details of **international transfers** and safeguards (SCCs, adequacy decisions).
- [ ] **Retention periods** (or criteria for determining them).
- [ ] **Data subject rights** (access, rectification, erasure, restriction, portability, objection, complaint to supervisory authority).
- [ ] Whether data provision is a **contractual/statutory requirement** and consequences of not providing.
- [ ] Information about **automated decision-making/profiling** (Art. 22) -- logic, significance, envisaged consequences.
- [ ] **Right to withdraw consent** at any time (if consent is the basis).
- [ ] Right to lodge a **complaint** with a supervisory authority.
- [ ] **Source of data** if not collected directly from the data subject (Art. 14).
- [ ] Date of last update.

### Language & Accessibility
- Written in **clear, plain language**.
- Easily accessible (persistent footer link, not buried in ToS).
- Separate child-friendly version if targeting minors.

---

## 4. Records of Processing Activities -- ROPA (Art. 30)

Required for organisations with 250+ employees, **OR** if processing:
- is likely to result in a risk to data subjects,
- is not occasional, or
- includes special categories of data or criminal conviction data.

**In practice: every SaaS company should maintain a ROPA.**

### Controller ROPA must contain:
| Field | Description |
|---|---|
| Controller name & contact | Legal entity, DPO |
| Purposes of processing | Per activity |
| Categories of data subjects | Users, employees, leads |
| Categories of personal data | Email, IP, payment info |
| Categories of recipients | Sub-processors, third parties |
| Transfers to third countries | Countries + safeguards |
| Retention periods | Per data category |
| Technical & org measures | Encryption, access control |

### Processor ROPA must contain:
- Name & contact of processor and each controller.
- Categories of processing carried out for each controller.
- Transfers to third countries and safeguards.
- General description of technical and organisational security measures.

---

## 5. Data Protection Impact Assessment -- DPIA (Art. 35)

### When required:
- **Systematic and extensive profiling** with significant effects on individuals.
- **Large-scale processing** of special categories or criminal conviction data.
- **Systematic monitoring** of publicly accessible areas on a large scale.
- Processing using **new technologies** where likely high risk.
- **Automated decision-making** with legal or similarly significant effects.
- Large-scale **cross-referencing** of datasets.

### DPIA must include:
1. Systematic description of the processing and purposes.
2. Assessment of necessity and proportionality.
3. Assessment of risks to the rights and freedoms of data subjects.
4. Measures to mitigate risks.

### Process:
- Conduct **before** processing begins.
- Consult the DPO (if appointed).
- If residual high risk remains after mitigation: **prior consultation** with the supervisory authority (Art. 36).

---

## 6. Data Protection Officer -- DPO (Art. 37-39)

### Mandatory appointment when:
- Processing is carried out by a **public authority**.
- **Core activities** consist of processing requiring **regular and systematic monitoring** of data subjects on a large scale.
- **Core activities** consist of large-scale processing of **special categories of data** or criminal conviction data.

### DPO requirements:
- Can be internal employee or external contractor.
- Must have **expert knowledge** of data protection law and practices.
- Must be given **adequate resources** and **no instructions** regarding the exercise of tasks.
- Must report to **highest management level**.
- Cannot be **dismissed or penalised** for performing DPO tasks.
- Contact details must be published and communicated to the supervisory authority.

### DPO tasks:
- Inform and advise the controller/processor.
- Monitor compliance.
- Advise on DPIAs.
- Cooperate with the supervisory authority.
- Act as contact point for data subjects.

---

## 7. Data Processing Agreement -- DPA (Art. 28)

Required whenever a controller engages a processor. For SaaS: you are typically a **processor** for B2B customers, and a **controller** (or joint controller) for your own users.

### Mandatory DPA clauses:
- [ ] Subject matter, duration, nature and purpose of processing.
- [ ] Types of personal data and categories of data subjects.
- [ ] Obligations and rights of the controller.
- [ ] Processing only on **documented instructions** from the controller.
- [ ] **Confidentiality** obligations for authorised personnel.
- [ ] **Security measures** (Art. 32) -- technical and organisational.
- [ ] Conditions for engaging **sub-processors** (prior specific or general written authorisation).
- [ ] **Assistance** with data subject requests.
- [ ] **Assistance** with security obligations, breach notification, DPIAs, prior consultation.
- [ ] **Deletion or return** of data upon termination.
- [ ] Making available all information to **demonstrate compliance** and allow **audits**.
- [ ] Processor must inform controller if an instruction infringes GDPR.

### Sub-processor chain:
- General authorisation: controller may object to new sub-processors within a reasonable period.
- Specific authorisation: each sub-processor requires individual approval.
- Same data protection obligations must flow down to sub-processors.

---

## 8. Data Subject Rights (Chapter III)

| Right | Article | SaaS Implementation |
|---|---|---|
| **Right of access** | Art. 15 | Provide copy of all personal data within 1 month |
| **Right to rectification** | Art. 16 | Allow users to correct inaccurate data |
| **Right to erasure ("right to be forgotten")** | Art. 17 | Delete data upon request (unless legal retention applies) |
| **Right to restriction of processing** | Art. 18 | Mark data and cease processing (but keep stored) |
| **Right to data portability** | Art. 20 | Export data in structured, machine-readable format (JSON, CSV) |
| **Right to object** | Art. 21 | Especially to direct marketing (must stop immediately) |
| **Rights re: automated decision-making** | Art. 22 | Right not to be subject to solely automated decisions with legal effects; right to human intervention |
| **Right to notification** | Art. 19 | Notify recipients of rectification/erasure/restriction |

### Practical requirements:
- Respond within **1 month** (extendable to 3 months for complex requests).
- **Free of charge** (except manifestly unfounded or excessive requests).
- Verify identity before fulfilling requests.
- Log all requests and responses.
- Provide a self-service data export/delete feature where feasible.

---

## 9. Data Breach Notification (Art. 33 & 34)

### To Supervisory Authority (Art. 33):
- Notify **within 72 hours** of becoming aware.
- If not within 72 hours: provide reasons for delay.
- Notification must include:
  - Nature of the breach (categories and approximate number of data subjects and records).
  - DPO or contact point name.
  - Likely consequences of the breach.
  - Measures taken or proposed to address/mitigate.

### To Data Subjects (Art. 34):
- Required when breach is likely to result in **high risk** to rights and freedoms.
- Must describe in **clear, plain language**.
- Not required if: data was encrypted/rendered unintelligible, subsequent measures eliminated the high risk, or it would involve disproportionate effort (use public communication instead).

### SaaS breach response plan:
1. Detect and contain.
2. Assess severity and risk.
3. Notify supervisory authority within 72 hours.
4. Notify affected data subjects if high risk.
5. Document everything (even if you decide not to notify).
6. Review and improve security measures.

---

## 10. Penalties (Art. 83)

### Tier 1 -- Up to EUR 10 million or 2% of global annual turnover (whichever is higher):
- Violations of controller/processor obligations (Art. 8, 11, 25-39, 42, 43).
- Violations of certification body obligations.
- Violations of monitoring body obligations.

### Tier 2 -- Up to EUR 20 million or 4% of global annual turnover (whichever is higher):
- Violations of basic processing principles (Art. 5, 6, 7, 9).
- Violations of data subject rights (Art. 12-22).
- Violations of international transfer provisions (Art. 44-49).
- Non-compliance with supervisory authority orders.

### Aggravating factors:
- Nature, gravity, and duration of the infringement.
- Intentional or negligent character.
- Number of data subjects affected.
- Level of damage suffered.
- Degree of cooperation with the supervisory authority.
- Previous infringements.

---

## 11. Digital Services Act (DSA) -- Hosting Provider Obligations

If your SaaS qualifies as a **hosting service** (stores content for users), DSA imposes:

- **Notice-and-action mechanism**: process reports of illegal content.
- **Transparency reporting**: publish reports on content moderation.
- **Terms of service**: clearly state content policies, restrictions, and algorithmic decision-making.
- **Contact point** for authorities and users.
- **Legal representative** in the EU if not established there.
- **Trusted flaggers** cooperation (for large platforms).
- **Statement of reasons** when restricting content.

### Thresholds:
- Micro/small enterprises: lighter obligations.
- Very Large Online Platforms (VLOPs, 45M+ monthly EU users): full set including systemic risk assessments, audits, data access for researchers.

---

## 12. European Accessibility Act (EAA) -- Directive 2019/882

**Effective: 28 June 2025** for new products and services.

### Applies to:
- E-commerce services (SaaS selling to consumers).
- Websites and mobile applications of services covered by the Directive.
- Banking, transport, e-books, and other specified sectors.

### Requirements:
- **WCAG 2.1 Level AA** compliance (by reference via EN 301 549).
- Perceivable, operable, understandable, robust interfaces.
- Accessible customer support channels.
- Information about accessibility features in documentation.

### Exemptions:
- Micro-enterprises (fewer than 10 employees and less than EUR 2M turnover) are exempt.
- Disproportionate burden defense (must document and report).

### Penalties:
- Set by member states -- must be effective, proportionate, and dissuasive.

---

## 13. Practical GDPR Compliance Checklist for SaaS

### Foundation
- [ ] Map all personal data flows (collection, storage, processing, sharing, deletion).
- [ ] Maintain Records of Processing Activities (ROPA).
- [ ] Identify and document the lawful basis for each processing activity.
- [ ] Appoint a DPO if required (or voluntarily for good practice).
- [ ] Designate an EU Representative if not established in the EU (Art. 27).

### Documentation
- [ ] Publish a GDPR-compliant **Privacy Policy**.
- [ ] Prepare **Data Processing Agreements** for all sub-processors.
- [ ] Offer a DPA for your B2B customers (you as processor).
- [ ] Create internal **data protection policies** (access control, retention, deletion).
- [ ] Document **Legitimate Interest Assessments** where applicable.

### Technical Measures
- [ ] Implement encryption at rest and in transit (TLS 1.2+).
- [ ] Apply pseudonymisation where possible.
- [ ] Enforce role-based access control.
- [ ] Maintain audit logs.
- [ ] Implement data minimisation in product design.
- [ ] Build self-service data export (JSON/CSV) for portability.
- [ ] Build self-service account deletion feature.

### Consent & Cookies
- [ ] Implement a GDPR-compliant **cookie consent banner** (no pre-ticked, granular, easy reject).
- [ ] Obtain and log **explicit consent** for marketing communications.
- [ ] Provide easy unsubscribe / consent withdrawal mechanisms.

### Breach Response
- [ ] Create and test a **breach response plan**.
- [ ] Define roles: who detects, assesses, notifies.
- [ ] Pre-draft notification templates for supervisory authorities and data subjects.
- [ ] Maintain a **breach register** (even for non-notifiable breaches).

### Data Subject Rights
- [ ] Implement a process/portal for handling DSR requests.
- [ ] Train support team on handling DSR requests.
- [ ] Set up tracking to ensure 1-month response deadline.
- [ ] Verify identity before fulfilling requests.

### International Transfers
- [ ] Identify all cross-border data flows.
- [ ] Implement appropriate safeguards (SCCs, adequacy decisions, BCRs).
- [ ] Conduct Transfer Impact Assessments (TIAs) where required.

### Ongoing Compliance
- [ ] Conduct annual GDPR compliance reviews.
- [ ] Conduct DPIAs for new features/products with potential high risk.
- [ ] Train employees on data protection (at onboarding and annually).
- [ ] Review and update sub-processor list regularly.
- [ ] Monitor regulatory guidance and enforcement actions.

---

## Quick Reference: Key Articles

| Article | Topic |
|---|---|
| Art. 5 | Principles of processing |
| Art. 6 | Lawful bases |
| Art. 7 | Conditions for consent |
| Art. 12-22 | Data subject rights |
| Art. 25 | Data protection by design and by default |
| Art. 28 | Processor obligations / DPA |
| Art. 30 | Records of processing activities |
| Art. 32 | Security of processing |
| Art. 33-34 | Breach notification |
| Art. 35-36 | DPIA and prior consultation |
| Art. 37-39 | DPO |
| Art. 44-49 | International transfers |
| Art. 83 | Penalties |
