# Cross-Border Data Transfers for SaaS Companies

> Transferring personal data across borders is one of the most complex compliance areas for SaaS.
> This reference covers EU/EEA, UK, US, Russia, UAE, and provides practical decision frameworks.

---

## 1. EU/EEA -- Transfer Mechanisms Overview

Under GDPR Chapter V (Art. 44-49), transfers of personal data to countries outside the EEA are prohibited unless one of the following mechanisms is in place:

| Mechanism | Article | When to Use |
|---|---|---|
| **Adequacy decision** | Art. 45 | Destination country has EU adequacy status |
| **Standard Contractual Clauses (SCCs)** | Art. 46(2)(c) | Most common mechanism for B2B SaaS |
| **Binding Corporate Rules (BCRs)** | Art. 47 | Intra-group transfers within a multinational |
| **Approved code of conduct** | Art. 46(2)(e) | Industry-specific codes |
| **Approved certification** | Art. 46(2)(f) | GDPR certification schemes |
| **Derogations** | Art. 49 | Limited, specific situations only (not for systematic transfers) |

---

## 2. EU Adequacy Decisions (Art. 45)

Countries/territories with an EU adequacy decision (transfers allowed without additional safeguards):

| Country/Territory | Decision Date | Notes |
|---|---|---|
| Andorra | 2010 | |
| Argentina | 2003 | |
| Canada | 2001 | Commercial organisations under PIPEDA only |
| Faroe Islands | 2010 | |
| Guernsey | 2003 | |
| Isle of Man | 2004 | |
| Israel | 2011 | |
| Japan | 2019 | Supplementary rules apply |
| Jersey | 2008 | |
| New Zealand | 2013 | |
| Republic of Korea (South Korea) | 2022 | |
| Switzerland | 2000 | |
| United Kingdom | 2021 | Valid until June 2025, expected renewal |
| Uruguay | 2012 | |
| United States | 2023 | **Only for DPF-certified organisations** |
| EU/EEA internal transfers | N/A | Free flow within EEA |

**Important**: adequacy decisions can be reviewed and revoked. Monitor updates.

---

## 3. Standard Contractual Clauses -- SCCs (2021)

The current EU SCCs were adopted by **Commission Implementing Decision (EU) 2021/914** on 4 June 2021, replacing the old 2001/2010 SCCs.

### Four modules:

| Module | Scenario | Common SaaS Use |
|---|---|---|
| **Module 1** | Controller to Controller (C2C) | SaaS sharing data with independent third-party controller |
| **Module 2** | Controller to Processor (C2P) | SaaS customer (controller) engaging SaaS vendor (processor) outside EEA |
| **Module 3** | Processor to Processor (P2P) | SaaS vendor (processor) engaging sub-processor outside EEA |
| **Module 4** | Processor to Controller (P2C) | Less common; processor transferring back to controller in third country |

### Key provisions in 2021 SCCs:
- **Docking clause**: additional parties can accede over time without re-executing.
- **Data subject rights**: third-party beneficiary rights for data subjects.
- **Sub-processor obligations**: must flow down SCC protections.
- **Governing law**: must be law of an EU member state.
- **Competent supervisory authority**: DPA of the data exporter's establishment.
- **Annex I**: description of parties, transfer, and competent authority.
- **Annex II**: technical and organisational measures (security).
- **Annex III**: list of sub-processors (for Modules 2 and 3).

### Cannot be modified:
- The SCC clauses themselves cannot be altered.
- Additional clauses can be added if they do not contradict or diminish SCC protections.
- Annexes must be completed with specific transfer details.

---

## 4. Transfer Impact Assessment (TIA)

### Required for every transfer relying on SCCs (Schrems II, CJEU C-311/18):
A TIA evaluates whether the legal framework of the recipient country provides essentially equivalent protection to GDPR.

### TIA steps:

**Step 1: Know your transfer**
- What data is transferred?
- Who is the data exporter and importer?
- What is the legal basis for the transfer?
- Which SCC module applies?

**Step 2: Assess the recipient country's legal framework**
- Surveillance laws (government access to data).
- Data protection laws and enforcement.
- Rule of law and judicial independence.
- Specific sector regulations.

**Step 3: Evaluate relevance of problematic laws**
- Do the laws apply in practice to the specific transfer?
- Is the data importer subject to these laws?
- Has the data importer received government access requests?
- What is the likelihood of access based on data type and importer category?

**Step 4: Identify supplementary measures (if needed)**
| Type | Examples |
|---|---|
| **Technical** | End-to-end encryption (where importer has no key), pseudonymisation, split processing |
| **Contractual** | Transparency obligations, challenge/notify commitments, warrant canary |
| **Organisational** | Access controls, security certifications, internal policies |

**Step 5: Document and review**
- Record the assessment and reasoning.
- Review periodically (at least annually) or when laws change.
- Be prepared to suspend transfers if protection cannot be ensured.

---

## 5. Binding Corporate Rules (BCRs) -- Art. 47

### When to use:
- Intra-group transfers within a multinational corporate group.
- Approved by the lead supervisory authority with cooperation from other concerned DPAs.

### Types:
- **BCR for controllers** (BCR-C): WP256.
- **BCR for processors** (BCR-P): WP257.

### Approval process:
- Complex and lengthy (12-18 months or more).
- Requires a lead DPA (where EU headquarters is located).
- Must include: binding and enforceable commitments, data protection principles, data subject rights, complaint handling, cooperation with DPAs, training, audit programme.
- Must be legally binding on all group members.

### Practical note for SaaS:
- BCRs are typically pursued by large enterprises.
- For most SaaS companies, SCCs are more practical.
- BCRs can be combined with SCCs for transfers to entities outside the corporate group.

---

## 6. US Data Privacy Framework (DPF)

### Background:
- **Safe Harbor**: invalidated by Schrems I (2015).
- **Privacy Shield**: invalidated by Schrems II (2020).
- **EU-US Data Privacy Framework**: adequacy decision adopted **10 July 2023**.
- **UK Extension**: adopted for UK-US transfers.
- **Swiss-US DPF**: separate framework.

### How it works:
- US organisations **self-certify** with the US Department of Commerce.
- Must commit to DPF Principles (notice, choice, accountability for onward transfer, security, data integrity and purpose limitation, access, recourse/enforcement/liability).
- Certification is public (searchable on dataprivacyframework.gov).
- Applies only to **certified organisations** -- check certification status before relying on adequacy.

### Protections for EU/UK individuals:
- Access to independent dispute resolution.
- Arbitration panel (Data Privacy Framework Panel).
- Oversight by the US Data Protection Review Court (DPRC).
- Limits on US intelligence access under Executive Order 14086.

### SaaS practical use:
- If your US sub-processors are DPF-certified: adequacy applies (no SCCs needed for that specific transfer).
- **Best practice**: maintain SCCs as backup even for DPF-certified partners (in case of invalidation or lapse of certification).
- Always verify active certification status: dataprivacyframework.gov.

---

## 7. Russia -- Cross-Border Transfer Rules (152-FZ)

### Federal Law No. 152-FZ "On Personal Data" -- transfer provisions:

### Data localisation (Art. 18, para. 5):
- **Primary collection and storage of Russian citizens' personal data must occur in databases located in Russia.**
- Processing may occur abroad, but the primary database must be in Russia.
- Applies to any operator collecting personal data of Russian citizens, regardless of where the operator is located.

### Cross-border transfer rules (Art. 12):

**Unrestricted transfers to:**
- Countries that are parties to the **Council of Europe Convention 108** (most of Europe, plus others).
- Countries on Roskomnadzor's **adequate protection list** (largely overlaps with Convention 108 signatories).

**Transfers to other countries require one of:**
- **Written consent** of the data subject (specific, informed, conscious).
- Performance of a contract with the data subject.
- Protecting the life, health, or vital interests of the data subject.
- Federal law requirements (e.g., taxation, anti-money laundering).

### Roskomnadzor notification:
- Before commencing cross-border transfers to countries NOT on the adequate list, the operator must **notify Roskomnadzor**.
- Roskomnadzor may **restrict or prohibit** the transfer if the receiving country does not provide adequate protection.

### Practical implications for SaaS:
- If collecting data of Russian users: **store the primary database in Russia** (use Russian hosting/cloud provider or Russia-located servers).
- Cross-border processing is permissible but the master copy stays in Russia.
- Ensure consent forms for Russian users explicitly cover cross-border transfer.
- Monitor Roskomnadzor enforcement -- they can block non-compliant services.
- **Penalties**: fines up to RUB 6 million for first violation of localisation; up to RUB 18 million for repeated violations (as of recent amendments).

### Key differences from GDPR transfers:
| Aspect | GDPR | Russia 152-FZ |
|---|---|---|
| **Localisation** | No requirement to store in EU | **Must store primary database in Russia** |
| **Mechanism** | SCCs, adequacy, BCRs | Adequate country list + consent/contract |
| **Regulator approval** | Not required for SCCs | Notification to Roskomnadzor may be required |
| **Blocking** | DPA can order suspension | Roskomnadzor can block the service entirely |

---

## 8. UAE -- Cross-Border Transfer Rules (PDPL)

### Federal Decree-Law No. 45 of 2021 on the Protection of Personal Data (PDPL):
- Effective: 2 January 2022; enforcement provisions phased in.
- Implementing regulations issued by the UAE Data Office.

### Cross-border transfer rules:

**Transfers allowed if:**
1. Destination country is on the **UAE adequate countries list** (published by UAE Data Office).
2. Appropriate safeguards are in place (SCCs, binding agreements, BCRs equivalent).
3. **Explicit consent** of the data subject.
4. Performance of a contract.
5. Legal claims.
6. Vital interests.
7. Public interest recognised by UAE law.

### Key requirements:
- **Data must not be transferred in a way that prejudices UAE national security or vital interests.**
- The UAE Data Office can issue decisions restricting transfers to specific countries.
- Controllers must ensure the receiving party provides adequate protection.

### Free zone considerations:
- **DIFC (Dubai International Financial Centre)**: has its own data protection law (DIFC Data Protection Law No. 5 of 2020) -- modelled on GDPR. Separate adequacy list and transfer mechanisms.
- **ADGM (Abu Dhabi Global Market)**: has its own Data Protection Regulations 2021 -- also GDPR-influenced. Separate transfer rules.
- **IFZA, DMCC, other free zones**: generally fall under the federal PDPL unless they have their own data protection framework.

### Practical implications for SaaS in UAE:
- Determine which framework applies: federal PDPL, DIFC, or ADGM.
- If operating from DIFC/ADGM: follow their specific transfer rules (more GDPR-like).
- If operating under federal PDPL: check the UAE adequate countries list and implement appropriate safeguards.
- Consent-based transfers are common in practice.
- Keep primary data processing transparent and documented.

---

## 9. Practical Decision Tree

### "Where is your server? Where are your users?"

```
START: Where are your USERS located?
|
+---> EU/EEA users?
|     |
|     YES --> Where is your SERVER / data stored?
|     |       |
|     |       +---> In the EU/EEA
|     |       |     --> No cross-border transfer issue
|     |       |     --> Standard GDPR compliance applies
|     |       |
|     |       +---> In an ADEQUATE country (UK, Japan, etc.)
|     |       |     --> Transfer is permitted
|     |       |     --> Document the adequacy basis
|     |       |
|     |       +---> In the US
|     |       |     --> Is your provider DPF-certified?
|     |       |     |   YES --> Adequacy applies (verify certification)
|     |       |     |   NO  --> Sign SCCs (Module 2 or 3) + conduct TIA
|     |       |     --> Best practice: maintain SCCs as backup even with DPF
|     |       |
|     |       +---> In another country (no adequacy)
|     |             --> Sign SCCs + conduct TIA
|     |             --> Consider supplementary measures
|     |             --> If TIA shows inadequate protection: consider
|     |                 relocating data or implementing strong encryption
|     |
+---> UK users?
|     |
|     YES --> Where is your SERVER / data stored?
|             |
|             +---> In the UK
|             |     --> No transfer issue; UK GDPR applies
|             |
|             +---> In the EU/EEA
|             |     --> UK adequacy to EU: OK (EU has adequacy for UK)
|             |     --> EU to UK: covered by UK adequacy decision
|             |
|             +---> In the US
|             |     --> UK Extension to DPF: check certification
|             |     --> Or: UK IDTA / UK Addendum to EU SCCs + TRA
|             |
|             +---> Other country
|                   --> UK IDTA or UK Addendum + Transfer Risk Assessment
|
+---> Russian users?
|     |
|     YES --> PRIMARY database MUST be in Russia
|     |       --> Cross-border processing permitted with safeguards
|     |       --> Check if destination is on Convention 108 / Roskomnadzor list
|     |       --> If not: obtain explicit consent + notify Roskomnadzor
|     |       --> Consider: Russian hosting for primary storage + sync to main infra
|
+---> UAE users?
|     |
|     YES --> Which framework applies?
|             |
|             +---> DIFC --> DIFC Data Protection Law (GDPR-like transfers)
|             +---> ADGM --> ADGM Data Protection Regulations (GDPR-like)
|             +---> Federal PDPL --> Check UAE adequate countries list
|                   --> If not adequate: obtain consent or implement safeguards
|                   --> Ensure no prejudice to UAE national security
|
+---> California (US) users?
|     |
|     YES --> CCPA/CPRA does not have transfer restrictions per se
|     |       --> But: "sharing" for cross-context behavioural advertising
|     |             must comply with opt-out requirements
|     |       --> Service provider contracts must restrict use
|
+---> Other jurisdictions?
      |
      --> Check local data protection law for transfer restrictions
      --> Common pattern: adequacy list + contractual safeguards + consent
      --> Examples: Brazil LGPD, India DPDPA, South Korea PIPA,
          China PIPL (strict -- separate analysis required)
```

---

## 10. Sub-Processor Chain -- Practical Guidance

### Typical SaaS data flow:
```
Your EU Customer (Controller)
    |
    v
Your SaaS App (Processor) -- may be in EU or US
    |
    +---> Cloud provider (Sub-processor: AWS, GCP, Azure)
    |     |
    |     Location: EU region? US region? Both?
    |
    +---> Email service (Sub-processor: SendGrid, Mailgun)
    |
    +---> Analytics (Sub-processor: Mixpanel, Amplitude)
    |
    +---> Payment (Sub-processor: Stripe)
    |
    +---> Support (Sub-processor: Zendesk, Intercom)
```

### For each sub-processor, determine:
1. Where do they store/process data?
2. Do they have DPF certification (if US)?
3. Do they offer EU data residency?
4. Do they sign SCCs / DPA?
5. Do they have sub-sub-processors and where are those located?

### Recommendations:
- Choose **EU data residency** options where available (most major cloud providers offer this).
- Maintain a **public sub-processor list** (GDPR Art. 28 requirement for general authorisation model).
- Notify customers of sub-processor changes (typically 30 days advance notice).
- Ensure SCCs flow down the entire chain.
- Conduct TIAs for each link in the chain where data leaves the EEA.

---

## 11. Compliance Checklist -- Cross-Border Transfers

- [ ] **Map all data flows** -- where data originates, where it is stored, where it is processed, where it is accessed from.
- [ ] **Identify transfer mechanisms** for each cross-border flow.
- [ ] **Sign SCCs (2021 version)** for all transfers lacking adequacy.
- [ ] **Conduct TIAs** for each SCC-based transfer.
- [ ] **Verify DPF certification** for US recipients (dataprivacyframework.gov).
- [ ] **Implement UK IDTA or UK Addendum** for UK-origin transfers.
- [ ] **Comply with Russian localisation** if collecting data from Russian users.
- [ ] **Check UAE framework** (federal PDPL, DIFC, or ADGM) for UAE-based operations.
- [ ] **Maintain sub-processor list** with locations and transfer mechanisms.
- [ ] **Implement supplementary measures** where TIA identifies risks (encryption, pseudonymisation).
- [ ] **Document everything** -- transfer maps, TIAs, SCC copies, adequacy assessments.
- [ ] **Review annually** or when laws/adequacy decisions change.
- [ ] **Choose EU data residency** for cloud providers where feasible.
- [ ] **Prepare suspension plan** -- what happens if a transfer mechanism is invalidated?
