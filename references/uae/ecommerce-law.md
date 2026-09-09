# UAE E-Commerce and Consumer Protection Law

> Reference covering Federal Decree-Law No. 46/2021 (Electronic Transactions and Trust Services),
> Federal Law No. 15/2020 (Consumer Protection), and E-Commerce Law No. 1/2006.
> For SaaS and EdTech companies operating in or selling to the UAE.
> Last updated: March 2026. Verify current requirements with legal counsel.

---

## 1. Federal Decree-Law No. 46/2021 -- Electronic Transactions and Trust Services

### Overview

This law replaced the earlier Electronic Transactions and Commerce Law (Federal Law No. 1/2006) and modernized the UAE's framework for electronic transactions, digital signatures, and trust services.

### Scope

- Applies to all electronic transactions, records, and signatures in the UAE.
- Covers both domestic and international electronic transactions where at least one party is in the UAE.
- Applies to commercial, civil, and administrative transactions conducted electronically.

### Key Provisions

#### Legal Recognition of Electronic Records and Signatures

- **Electronic records** have the same legal effect as paper documents.
- **Electronic signatures** are legally valid and enforceable. The law distinguishes between:
  - **Electronic signature**: Any data in electronic form attached to or associated with an electronic document (e.g., typed name, click-to-accept).
  - **Secure electronic signature**: A signature verified by a certified trust service provider, with higher evidentiary weight.
  - **Digital signature**: Based on public key infrastructure (PKI) with certificate.

#### Formation of Electronic Contracts

- Contracts formed electronically are valid and enforceable.
- An offer and acceptance can be communicated by electronic means.
- An electronic contract is formed when the acceptance reaches the offeror's information system.
- **Click-wrap and browse-wrap agreements**: Legally recognized if the user has clear opportunity to review terms and affirmatively accepts (click-wrap is stronger than browse-wrap).

#### Automated Transactions

- Contracts formed by automated systems (without human review) are valid.
- Relevant for SaaS: Automated subscription sign-ups, payment processing, and service provisioning are legally recognized transactions.

#### Attribution of Electronic Messages

- An electronic message is attributed to the originator if it was sent by the originator, by a person authorized by the originator, or by an automated system programmed by the originator.
- Important for: Automated emails, system notifications, and electronic invoices from SaaS platforms.

#### Record Retention

- Electronic records must be retained in a format that ensures:
  - Integrity of the information.
  - Accessibility for subsequent reference.
  - Retention of information identifying origin, destination, date, and time.
- Retention period: As specified by applicable laws (generally 5 years for commercial records).

### SaaS Implications

| Requirement | Action |
|---|---|
| Valid electronic contracts | Ensure Terms of Service use click-wrap acceptance (checkbox + "I agree") |
| Electronic invoices | Invoices sent electronically are legally valid; ensure they meet VAT invoice requirements |
| Record retention | Store transaction records, communications, and contracts for at least 5 years |
| Automated systems | Document that automated processes (sign-up, billing) are properly configured |
| Digital signatures | For high-value contracts, consider secure electronic signatures via UAE-certified providers |

---

## 2. Federal Law No. 15/2020 -- Consumer Protection

### Overview

This law governs consumer protection across the UAE, applying to all goods and services offered to consumers, including digital services and e-commerce.

### Scope

- Applies to all **suppliers** offering goods or services to **consumers** in the UAE.
- **Supplier**: Any person who provides goods or services in the course of their business.
- **Consumer**: Any person who obtains goods or services for personal use (not for resale or commercial purposes).
- **Important for B2B SaaS**: If your platform serves individual end users (even through a business customer), consumer protection provisions may apply to those end users.

### Key Consumer Rights and Obligations

#### Right to Information

- Consumers have the right to accurate, clear information about goods and services.
- All information must be in **Arabic** (bilingual Arabic + English is common practice; Arabic is mandatory).
- Price information must be clear and include all taxes and fees.

#### Right to Safety

- Products and services must be safe and not pose risks to consumer health or safety.
- For SaaS: Ensure platform does not expose users to security risks, data breaches, or harmful content.

#### Right to Choose

- Consumers must not be forced to purchase additional goods or services as a condition of obtaining the desired product.
- **Anti-bundling**: Do not make essential service access contingent on purchasing unrelated add-ons.

#### Right to Privacy

- Consumer data must be protected. (Cross-reference with PDPL compliance.)
- Consumers must not receive unsolicited communications without consent.

#### Prohibited Practices

The law prohibits:

1. **Deceptive advertising**: False, misleading, or exaggerated claims about products or services.
2. **Bait-and-switch**: Advertising products/services at a price that is not actually available.
3. **Hidden fees**: Failing to disclose all costs before purchase.
4. **Counterfeit goods**: Selling counterfeit or imitation products.
5. **Unfair contract terms**: Terms that are excessively one-sided or that exclude fundamental consumer rights.
6. **Monopolistic practices**: Anti-competitive behavior.
7. **Withholding information**: Failing to provide material information that would affect the purchase decision.

#### Warranty and After-Sale Service

- Suppliers must honor any warranties (express or implied).
- For SaaS: Service level agreements (SLAs) function as a form of warranty. If you promise 99.9% uptime, you must deliver it.
- Defective goods/services: Consumer is entitled to repair, replacement, or refund.

### Penalties

| Violation | Penalty |
|---|---|
| Deceptive advertising | Fine up to AED 2,000,000 + possible imprisonment |
| Hidden fees / price fraud | Fine up to AED 1,000,000 |
| Consumer data misuse | Fine + potential business closure |
| Failure to honor warranty | Fine + compensation to consumer |
| Repeated violations | Doubled penalties + possible license revocation |

### Enforcement

- **Ministry of Economy** and local departments of economic development (DED) enforce consumer protection.
- Consumers can file complaints through the Ministry of Economy app, DED, or consumer protection hotline.

---

## 3. E-Commerce Law No. 1/2006 (Legacy Framework)

### Status

Federal Law No. 1/2006 (Electronic Transactions and Commerce Law) has been largely **superseded** by Federal Decree-Law No. 46/2021. However, some provisions remain relevant as interpretive guidance, and certain implementing regulations issued under the 2006 law may still be in effect.

### Key Legacy Provisions Still Relevant

#### E-Commerce Supplier Obligations

Suppliers engaging in e-commerce must:

1. **Disclose identity**: Full legal name, trade license number, registered address, and contact information.
2. **Provide clear product/service descriptions**: Accurate descriptions of what is being sold.
3. **Display prices clearly**: Including taxes and delivery charges.
4. **Provide terms and conditions**: Before the transaction is completed.
5. **Confirm orders**: Send electronic confirmation of orders and transactions.
6. **Maintain records**: Keep transaction records accessible.

#### Consumer Cooling-Off Period

- Under certain interpretations of the consumer protection framework, consumers may have a right to cancel online purchases within a specified period (typically 5-14 days depending on the product/service type and applicable regulations).
- **SaaS subscriptions**: The cooling-off period is generally applicable to one-time purchases. Subscription cancellation terms should be clearly stated in the Terms of Service.
- **Digital content**: Once digital content is delivered or a service is activated, the cooling-off right may be waived if the consumer was informed and agreed beforehand.

---

## 4. Website Requirements

### Mandatory Disclosures for Online Sellers / SaaS Providers

Every website or application offering goods or services to UAE consumers must display:

#### Company Information

- [ ] Full legal name of the company (as registered)
- [ ] Trade license number
- [ ] Free zone name (e.g., "Registered in IFZA, Dubai")
- [ ] Registered business address
- [ ] Contact email address
- [ ] Contact phone number
- [ ] TRN (Tax Registration Number) if VAT registered

#### Pricing and Payment

- [ ] Clear pricing in AED (UAE Dirhams) -- foreign currency pricing may be shown alongside but AED should be present or easily accessible
- [ ] All prices inclusive of VAT (or clearly state "+ 5% VAT")
- [ ] Total cost displayed before payment confirmation (including any fees, taxes, delivery charges)
- [ ] Accepted payment methods listed
- [ ] Payment security measures disclosed (PCI DSS compliance, SSL/TLS)
- [ ] Subscription pricing clearly stated (monthly/annual, auto-renewal terms)
- [ ] Free trial terms clearly stated (duration, what happens at expiry, payment method requirements)

#### Refunds and Cancellation

- [ ] Refund policy clearly stated and accessible before purchase
- [ ] Cancellation process described (how to cancel, effective date, pro-rata refund if applicable)
- [ ] Subscription auto-renewal cancellation instructions
- [ ] Contact method for refund requests
- [ ] Timeframe for refund processing

#### Product / Service Description

- [ ] Accurate, truthful description of the service
- [ ] Key features and limitations clearly stated
- [ ] Service availability (regions, system requirements)
- [ ] Any restrictions on use

### Advertising and Marketing Requirements

#### Truthful Advertising

- All advertising must be truthful and not misleading.
- Claims must be substantiated (e.g., "fastest platform" requires evidence).
- Testimonials must be genuine and not fabricated.
- Before/after claims must be accurate.

#### Comparative Advertising

- Comparing with competitors is permitted but must be:
  - Objective and verifiable
  - Not misleading
  - Not disparaging to the competitor

#### Digital Advertising Specific

- Sponsored content must be clearly labeled as advertising.
- Influencer marketing must disclose the commercial relationship.
- Email marketing requires opt-in consent (aligned with PDPL).
- Unsubscribe mechanism must be functional and honored promptly.

### Language Requirements

- **Arabic**: Mandatory for consumer-facing content in the UAE. At minimum, key legal documents (terms, privacy policy) should be available in Arabic.
- **English**: Acceptable as a supplementary language.
- **Practical approach**: Bilingual Arabic-English websites are standard practice. If Arabic translation is not yet available, English-only is common for international SaaS targeting global audiences, but adding Arabic is recommended for UAE-focused products and may be required for formal disputes.

---

## 5. Required Disclosures for Online Sellers

### Pre-Transaction Disclosures

Before a consumer completes a purchase, the following must be clearly communicated:

1. **Identity of the seller**: Legal name, license details, address.
2. **Nature of the product/service**: What the consumer is purchasing.
3. **Total price**: Including all taxes and fees, in AED.
4. **Payment terms**: When payment is due, accepted methods.
5. **Delivery/activation terms**: When and how the service will be provided.
6. **Cancellation rights**: Whether and how the consumer can cancel.
7. **Duration**: For subscriptions, the contract duration and renewal terms.
8. **Minimum requirements**: System requirements, prerequisites.

### Post-Transaction Requirements

1. **Order confirmation**: Electronic confirmation with order details, price, payment method.
2. **Receipt/invoice**: VAT-compliant invoice provided electronically.
3. **Access to terms**: Ongoing access to the terms and conditions agreed at purchase.
4. **Support access**: Clear contact method for customer support.
5. **Complaint mechanism**: Process for filing complaints.

### Records to Maintain

| Record | Retention Period |
|---|---|
| Transaction records | 5 years minimum |
| Customer communications | 5 years minimum |
| Invoices and receipts | 5 years (VAT requirement) |
| Contracts and terms accepted | Duration of relationship + 5 years |
| Marketing consent records | Duration of consent + 2 years |
| Complaint records | 5 years |

---

## 6. Digital Services Tax Implications

### Current Tax Landscape

#### VAT (5%)

- Applies to all taxable supplies of goods and services in the UAE.
- SaaS subscriptions sold to UAE customers are subject to 5% VAT.
- See IFZA compliance guide for detailed VAT treatment by scenario.

#### Corporate Tax (9%)

- Federal Decree-Law No. 47/2022 on Taxation of Corporations and Businesses.
- 9% on taxable income exceeding AED 375,000.
- 0% on taxable income up to AED 375,000.
- Free zone companies (including IFZA) may qualify for 0% rate on qualifying income if they meet substance requirements and do not derive income from transactions with mainland UAE entities (specific conditions apply under Qualifying Free Zone Person status).

#### No Withholding Tax

- The UAE does not impose withholding tax on payments to non-residents (dividends, interest, royalties) at the federal level. This is advantageous for SaaS companies making payments to foreign service providers.

#### No Personal Income Tax

- The UAE does not levy personal income tax. Relevant for founders and employees.

#### Digital Services Tax (DST)

- As of March 2026, the UAE has **not** implemented a separate digital services tax.
- The UAE has joined the OECD Inclusive Framework on BEPS and has implemented Pillar Two (global minimum tax of 15% for large multinationals with consolidated revenue above EUR 750M). This is unlikely to affect most SaaS startups.
- Monitor developments: The UAE may implement additional digital economy taxation measures in the future.

#### Customs Duty

- Digital services and software delivered electronically are not subject to customs duty.
- Physical goods imported into the UAE are subject to 5% customs duty (not applicable to most SaaS).

### Tax Compliance Summary for SaaS

| Tax | Applies? | Rate | Threshold |
|---|---|---|---|
| VAT | Yes | 5% | AED 375,000 taxable supplies |
| Corporate Tax | Yes | 9% (0% possible for QFZP) | AED 375,000 taxable income |
| Withholding Tax | No | N/A | N/A |
| Personal Income Tax | No | N/A | N/A |
| Digital Services Tax | No (as of 2026) | N/A | N/A |
| Customs Duty | No (for digital delivery) | N/A | N/A |
| Excise Tax | No (not applicable to SaaS) | N/A | N/A |

---

## 7. Dispute Resolution

### Consumer Complaints

1. **Direct resolution**: Attempt to resolve with the supplier first.
2. **Ministry of Economy**: File complaint through the consumer protection department.
3. **Local DED**: File complaint with the relevant emirate's Department of Economic Development.
4. **Courts**: Civil courts for contractual disputes.

### E-Commerce Dispute Considerations

- **Jurisdiction clause**: Include in Terms of Service. For IFZA companies, UAE courts (or DIAC/DIFC Courts if agreed) have jurisdiction.
- **Arbitration**: Consider including an arbitration clause (DIAC, DIFC-LCIA, or other recognized arbitration center).
- **Governing law**: Specify UAE federal law as governing law in contracts.
- **Online dispute resolution (ODR)**: The UAE has been developing ODR mechanisms. Smart Dubai and other initiatives may provide electronic dispute resolution platforms.

### SaaS Terms of Service Recommendations

1. Clearly state the governing law (UAE Federal Law).
2. Specify dispute resolution mechanism (courts, arbitration, or mediation).
3. Include a jurisdiction clause (e.g., courts of Dubai).
4. Provide a clear complaints process.
5. Set a limitation period for claims if permitted.
6. Ensure the dispute resolution clause is not unfairly one-sided (may be challenged as unfair contract term).

---

## Compliance Checklist Summary

### For Launch

- [ ] Company information displayed on website (name, license, address, contact, TRN)
- [ ] Terms of Service published with click-wrap acceptance
- [ ] Privacy Policy published (PDPL compliant)
- [ ] Cookie consent banner implemented
- [ ] Pricing displayed in AED, inclusive of or clearly showing VAT
- [ ] Refund and cancellation policy published
- [ ] Order confirmation system in place
- [ ] VAT-compliant invoicing system configured
- [ ] Arabic language content available (at minimum for legal documents)
- [ ] Payment security measures in place (SSL/TLS, PCI DSS)

### Ongoing

- [ ] Marketing communications use opt-in consent
- [ ] Advertising is truthful and substantiated
- [ ] Consumer complaints are tracked and resolved
- [ ] Transaction records retained for 5+ years
- [ ] VAT returns filed quarterly
- [ ] Corporate tax returns filed annually
- [ ] Regulatory changes monitored
