# CCPA / CPRA -- California Privacy Law for SaaS Companies

> **California Consumer Privacy Act (CCPA)** -- effective 1 January 2020
> **California Privacy Rights Act (CPRA)** -- amendments effective 1 January 2023, enforcement from 1 July 2023
> Enforced by: California Privacy Protection Agency (CPPA) and California Attorney General

---

## 1. Applicability Thresholds

A for-profit business must comply if it collects California consumers' personal information **AND** meets **any one** of:

| Threshold | Detail |
|---|---|
| **Annual gross revenue** | Exceeds **$25 million** (in prior calendar year) |
| **Consumer data volume** | Buys, sells, or shares personal information of **100,000+ consumers or households** per year |
| **Data revenue share** | Derives **50% or more** of annual revenue from **selling or sharing** consumers' personal information |

### Notes:
- "Consumer" = California resident (not just customers -- includes website visitors, employees, B2B contacts).
- CPRA removed the "devices" count -- now only "consumers or households."
- Non-profits and government agencies are exempt.
- Applies regardless of where the business is physically located.

### Service Provider vs. Third Party vs. Contractor:
- **Service provider / Contractor**: processes data on behalf of the business under a written contract; must not sell/share the data.
- **Third party**: any entity that is not a service provider/contractor.
- **Contractor** (CPRA addition): similar to service provider but with additional certification obligations.

---

## 2. Categories of Personal Information

CCPA/CPRA defines personal information broadly:

| Category | Examples |
|---|---|
| Identifiers | Name, email, IP address, account name, SSN, driver's license |
| Commercial info | Purchase history, products/services considered |
| Internet/network activity | Browsing history, search history, interaction with website/app |
| Geolocation data | Precise location |
| Professional/employment info | Job title, employer |
| Education information | Non-public education records |
| Inferences | Profiles reflecting preferences, characteristics, behaviour |
| **Sensitive personal info** (CPRA) | SSN, financial account + credentials, precise geolocation, racial/ethnic origin, religious beliefs, union membership, mail/email/text contents, genetic data, biometric data, health info, sex life/sexual orientation, government ID |

---

## 3. Privacy Policy Requirements

### Must disclose:
- [ ] **Categories of personal information** collected in the preceding 12 months.
- [ ] **Categories of sources** from which data is collected.
- [ ] **Business or commercial purposes** for collection.
- [ ] **Categories of third parties** with whom data is shared.
- [ ] **Categories of personal information sold or shared** (if any) and categories of third parties to whom it was sold/shared.
- [ ] For each category: **retention period** or criteria for determining it (CPRA addition).
- [ ] Description of each **consumer right** and how to exercise them.
- [ ] Contact information for exercising rights (toll-free number, web form, email).
- [ ] Whether the business sells or shares personal information of consumers under 16.
- [ ] Date of last update.

### Format:
- Must be available in the **same language(s)** as contracts/services.
- Updated **at least every 12 months**.
- Accessible via a clear link on the homepage (usually titled "Privacy Policy" or "Privacy").

---

## 4. Consumer Rights

### Right to Know (Art. 1798.100, 1798.110)
- Categories and specific pieces of personal information collected.
- Sources, purposes, and third parties.
- Business must provide information for the **preceding 12 months** (CPRA extends to information collected on or after 1 January 2022).

### Right to Delete (Art. 1798.105)
- Request deletion of personal information.
- Business must also direct service providers/contractors to delete.
- Exceptions: complete a transaction, detect security incidents, comply with legal obligations, internal expected uses compatible with consumer expectations.

### Right to Opt-Out of Sale/Sharing (Art. 1798.120)
- Consumers can opt out of the **sale** of their personal information.
- CPRA adds: opt out of **sharing** for cross-context behavioural advertising.
- Must honour **Global Privacy Control (GPC)** signals as a valid opt-out.
- Cannot require account creation to opt out.

### Right to Correct (Art. 1798.106 -- CPRA)
- Request correction of inaccurate personal information.
- Business must use commercially reasonable efforts to correct.

### Right to Limit Use of Sensitive Personal Information (Art. 1798.121 -- CPRA)
- Consumers can limit processing of sensitive personal information to what is necessary to provide the service.
- Must provide a "Limit the Use of My Sensitive Personal Information" link.

### Right to Non-Discrimination (Art. 1798.125)
- Cannot deny goods/services, charge different prices, or provide different quality based on exercising privacy rights.
- Financial incentives for data collection are allowed if disclosed and not unjust.

### Right to Data Portability (implied via Right to Know)
- When providing specific pieces, must deliver in a portable, readily usable format.

---

## 5. "Do Not Sell or Share My Personal Information" Link

### Requirements:
- **Clear and conspicuous link** on the homepage.
- Exact or substantially similar title: **"Do Not Sell or Share My Personal Information"**.
- Can be combined with "Limit the Use of My Sensitive Personal Information" as a single link.
- Can use a single clearly labelled link: **"Your Privacy Choices"** or **"Your California Privacy Choices"** with an opt-out icon.
- Must actually effectuate the opt-out -- not just a form to submit a request that gets reviewed.
- Must process the opt-out within **15 business days**.
- Cannot use **dark patterns** to steer consumers away from opting out.

### What counts as "sale" or "sharing":
- **Sale**: making personal information available to a third party for monetary or other valuable consideration.
- **Sharing**: making personal information available for cross-context behavioural advertising (even without monetary consideration).
- Using third-party analytics/advertising pixels (Google Analytics, social media ad pixels, etc.) likely constitutes "sharing."

---

## 6. Sensitive Personal Information Handling (CPRA)

### Additional obligations:
- Disclose in privacy policy if collecting sensitive PI.
- Provide the **"Limit the Use of My Sensitive Personal Information"** link.
- When consumer exercises this right: only process sensitive PI for:
  - Providing the goods/services requested.
  - Ensuring security and integrity.
  - Verifying or maintaining quality of service.
  - Short-term transient use (not profiling or building profiles).

### Categories of sensitive PI:
- Government ID numbers (SSN, driver's license, passport).
- Financial account info with access credentials.
- Precise geolocation.
- Racial/ethnic origin, religious beliefs, union membership.
- Contents of mail, email, text messages (unless business is the intended recipient).
- Genetic data, biometric data for ID purposes.
- Health information.
- Sex life or sexual orientation.

---

## 7. CPRA Additions and Key Changes

| Area | CCPA (original) | CPRA (amended) |
|---|---|---|
| **Enforcement** | Attorney General only | California Privacy Protection Agency (CPPA) + AG |
| **Scope** | 50,000+ consumers/households/devices | 100,000+ consumers/households (devices removed) |
| **Right to correct** | Not included | Added |
| **Sensitive PI** | Not separately defined | New category with use-limitation right |
| **Retention limits** | Not explicit | Must disclose retention periods; cannot retain longer than reasonably necessary |
| **Contractor** | Not defined | New category with certification obligations |
| **Automated decision-making** | Not addressed | Right to opt out of automated decision-making (CPPA rulemaking in progress) |
| **Data minimisation** | Not explicit | Collection must be reasonably necessary and proportionate |
| **Purpose limitation** | Not explicit | Cannot use data for purposes incompatible with disclosed purposes |
| **Audit rights** | Not explicit | CPPA may require annual cybersecurity audits and risk assessments for high-risk processing |
| **Children** | Opt-in consent for under-16 sale | Extended to sharing; double penalties for children's data violations |
| **Cure period** | 30-day cure period | Eliminated for CPPA enforcement (AG retains discretion) |

---

## 8. Responding to Consumer Requests

### Process:
1. **Verify identity** -- match at least two data points for "know" requests; reasonable verification for delete/correct.
2. **Acknowledge** receipt within **10 business days**.
3. **Respond** within **45 calendar days** (extendable by additional 45 days with notice).
4. **Free of charge** -- may charge reasonable fee or deny only if manifestly unfounded or excessive.
5. Provide response in a **portable, readily usable format** (for Right to Know specific pieces).
6. Provide at least **two methods** for submitting requests (e.g., web form + email; toll-free number required if you have a website).

### Authorised agents:
- Consumers may designate an authorised agent.
- Business may require written authorisation or power of attorney.
- Business may still verify the consumer's identity directly.

---

## 9. Penalties and Enforcement

### California Privacy Protection Agency (CPPA):
- Administrative enforcement -- no 30-day cure period (CPRA).
- Can investigate, audit, and issue fines.

### Attorney General:
- Civil enforcement in court.
- Retains discretionary cure period.

### Penalty amounts:
| Type | Amount |
|---|---|
| **Unintentional violation** | Up to **$2,500 per violation** |
| **Intentional violation** | Up to **$7,500 per violation** |
| **Violations involving children under 16** | Up to **$7,500 per violation** (CPRA doubles from CCPA's original amounts) |

### Private right of action (Art. 1798.150):
- Limited to **data breaches** caused by business's failure to implement reasonable security.
- Damages: $100-$750 per consumer per incident, or actual damages (whichever is greater).
- Injunctive/declaratory relief available.
- Must provide **30-day written notice** and opportunity to cure before filing suit for statutory damages.

---

## 10. Practical Compliance Checklist for SaaS

### Assessment
- [ ] Determine if thresholds are met ($25M revenue, 100K consumers, 50% data revenue).
- [ ] Map all personal information collected from California consumers.
- [ ] Identify all "sales" and "sharing" of personal information.
- [ ] Classify sensitive personal information separately.

### Website / App
- [ ] Publish compliant **Privacy Policy** with all required disclosures.
- [ ] Add **"Do Not Sell or Share My Personal Information"** link on homepage.
- [ ] Add **"Limit the Use of My Sensitive Personal Information"** link (if applicable).
- [ ] Honour **Global Privacy Control (GPC)** browser signals.
- [ ] Implement **cookie consent** mechanism that treats opt-out signals properly.
- [ ] Ensure no **dark patterns** in opt-out flows.

### Consumer Rights Infrastructure
- [ ] Build intake system (web form + email + toll-free number if applicable).
- [ ] Implement identity verification process.
- [ ] Build workflows to fulfill know, delete, correct, and portability requests.
- [ ] Track 10-business-day acknowledgment and 45-day response deadlines.
- [ ] Maintain records of requests and responses for **24 months**.

### Contracts
- [ ] Update service provider/contractor agreements with CCPA/CPRA-required terms.
- [ ] Include restrictions on selling/sharing, data use limitations, and compliance certifications.
- [ ] Ensure sub-contractor flow-down provisions.

### Security
- [ ] Implement **reasonable security measures** (encryption, access controls, vulnerability testing).
- [ ] Conduct risk assessments for high-risk processing (CPRA rulemaking pending).
- [ ] Prepare for potential CPPA-mandated cybersecurity audits.

### Training & Governance
- [ ] Train employees handling consumer inquiries on CCPA/CPRA rights.
- [ ] Designate internal privacy lead/team.
- [ ] Review and update practices at least annually.
- [ ] Monitor CPPA rulemaking for new requirements (automated decision-making, audits).
