# AI Content Disclosure Requirements for SaaS Platforms

## Overview

As AI becomes embedded in SaaS products -- powering chatbots, generating marketing content, grading student work, creating testimonials -- a growing body of legislation mandates disclosure of AI involvement. This reference covers the major frameworks requiring AI transparency, with practical guidance for SaaS and education platforms.

---

## European Union -- EU AI Act

### Key Provisions

The EU AI Act (Regulation (EU) 2024/1689) is the world's first comprehensive AI regulation. It takes a risk-based approach, with different requirements depending on the AI system's risk classification.

### Article 50 -- Transparency Obligations

Article 50 imposes disclosure requirements regardless of risk level for certain AI applications:

1. **Chatbot disclosure (Article 50(1))**: AI systems designed to interact directly with natural persons must be designed so that the person is informed they are interacting with an AI system, unless this is obvious from the circumstances. This applies to:
   - Customer support chatbots
   - AI tutors in education platforms
   - Any conversational AI interface
   - **Practical requirement**: Display a clear notice such as "You are chatting with an AI assistant" before or at the start of the interaction.

2. **Generative AI content marking (Article 50(2))**: Providers of AI systems that generate synthetic audio, image, video, or text content must ensure the output is marked in a machine-readable format as artificially generated or manipulated. This includes:
   - AI-generated blog posts, marketing copy, emails
   - AI-generated images used on websites or in ads
   - AI-generated audio or video content
   - **Practical requirement**: Embed metadata (e.g., C2PA provenance data) indicating AI generation. For text, implement technical marking solutions.

3. **Deepfake labeling (Article 50(4))**: Users of AI systems that generate or manipulate image, audio, or video content constituting a "deep fake" must disclose that the content has been artificially generated or manipulated. The disclosure must be clearly visible.

### Education as High-Risk (Annex III)

**Education and vocational training** is listed in Annex III of the EU AI Act as a high-risk category. Specifically:

- AI systems intended for use in determining access to, admission to, or assignment of persons to educational and vocational training institutions
- AI systems intended for evaluating learning outcomes, including systems used to steer the learning process
- AI systems intended for assessing the appropriate level of education for an individual
- AI systems used for monitoring and detecting prohibited behavior of students during tests

**Requirements for high-risk AI in education**:
- Risk management system (Article 9)
- Data governance and quality requirements (Article 10)
- Technical documentation (Article 11)
- Record-keeping and logging (Article 12)
- Transparency and information to users (Article 13)
- Human oversight provisions (Article 14)
- Accuracy, robustness, and cybersecurity (Article 15)
- Registration in the EU database before placing on the market
- Conformity assessment (self-assessment for education AI, typically)

### Penalties

- **Non-compliance with transparency obligations**: Up to EUR 15,000,000 or 3% of total worldwide annual turnover, whichever is higher.
- **Non-compliance with high-risk requirements**: Up to EUR 15,000,000 or 3% of total worldwide annual turnover.
- **Prohibited AI practices**: Up to EUR 35,000,000 or 7% of total worldwide annual turnover.
- **Supplying incorrect information to authorities**: Up to EUR 7,500,000 or 1% of turnover.

### Timeline

| Date | Milestone |
|------|-----------|
| August 1, 2024 | AI Act entered into force |
| February 2, 2025 | Prohibitions on unacceptable-risk AI apply |
| August 2, 2025 | Obligations for GPAI (general-purpose AI) models apply |
| **August 2, 2026** | **Transparency obligations (Article 50) apply** |
| August 2, 2026 | High-risk AI obligations for systems in Annex III apply |
| August 2, 2027 | High-risk AI obligations for systems embedded in regulated products apply |

**Key date for SaaS**: August 2, 2026 is when chatbot disclosure, generative content marking, and education AI compliance become enforceable.

---

## California

### AB 2013 -- Training Data Transparency (Effective January 1, 2026)

- **Requires** developers of generative AI systems to publicly disclose information about the datasets used to train their models.
- **Disclosures must include**:
  - A high-level summary of the training datasets
  - Whether the datasets include personal information
  - Whether the datasets include copyrighted material
  - The sources of the data (categories, not specific URLs)
  - How the data was collected
  - The time period the data covers
- **Applies to**: Any developer that makes a generative AI system available to Californians.
- **Practical impact**: If your SaaS uses a custom-trained AI model (not just API calls to a third-party model like GPT-4), you may need to publish training data disclosures. If you use a third-party API, the model provider (OpenAI, Anthropic, etc.) bears this obligation for the underlying model.

### CAITA -- California AI Transparency Act (Effective August 1, 2026)

- **Provenance marking**: AI systems that generate content (text, image, audio, video) must embed provenance information using industry standards (e.g., C2PA).
- **Disclosure at point of generation**: When a user generates content using an AI tool, the system must inform the user that the content is AI-generated.
- **Detection tools**: Providers must offer free detection tools to help users identify AI-generated content.
- **Penalties**: $5,000 per violation per day. Enforced by the California Attorney General.
- **Applies to**: Developers and providers of generative AI systems with significant operations in California or significant user bases in California.

### California Bot Disclosure Law (SB 1001, effective July 1, 2019)

- **Prohibits** the use of a bot to communicate with a person in California to incentivize a sale or influence a vote without disclosing that the communication is from a bot.
- **Applies to**: Any automated online account that communicates with California residents for commercial or political purposes.
- **Practical requirement**: If you have an AI chatbot that helps sell your product, it must disclose its non-human nature.
- **Penalties**: Enforced under California's Unfair Competition Law (UCL). No specific per-violation fine, but injunctive relief and restitution are available.

---

## Colorado -- AI Act (SB 24-205)

### Key Provisions

- **Effective**: June 1, 2026 (originally February 1, 2026, extended by amendment).
- **Scope**: Applies to "developers" and "deployers" of "high-risk AI systems" -- those that make consequential decisions about consumers in education, employment, financial services, government services, healthcare, housing, insurance, and legal services.
- **Disclosure requirements for deployers**:
  - Inform consumers that an AI system is being used to make a consequential decision about them
  - Provide a description of the AI system and its purpose
  - Provide contact information for the deployer
  - Describe the nature of the consequential decision and the role the AI system plays
  - Offer an opportunity for the consumer to correct incorrect data used by the AI
  - Offer an opportunity to appeal an adverse decision (with human review)
- **Disclosure requirements for developers**:
  - Provide documentation to deployers about the AI system's capabilities, limitations, intended uses, and known risks of bias
  - Disclose known risks of algorithmic discrimination
  - Publish on their website a summary of the types of high-risk AI systems they develop

### Education Relevance

- AI systems used for **admission decisions**, **grading**, **scholarship allocation**, or **student performance assessment** are likely "high-risk" under this law.
- If your SaaS platform uses AI to make or assist consequential decisions in education, you must comply.

### Penalties

- Enforced by the Colorado Attorney General under the Colorado Consumer Protection Act.
- No specific per-violation fine amount specified in the statute; standard CPA remedies apply (injunctive relief, penalties up to $20,000 per violation under the CPA).

---

## Other US States with AI Disclosure Laws

### Maine

- **LD 1946** (proposed/advancing): Would require AI transparency in government decision-making and certain commercial contexts.

### New York

- **NYC Local Law 144** (effective July 5, 2023): Requires bias audits and disclosure for automated employment decision tools (AEDT) used in hiring and promotion.
  - Annual independent bias audit required
  - Published results of audit on employer's website
  - Notice to candidates that AEDT is being used, at least 10 business days before use
  - **Relevance**: If your SaaS is used as an AEDT (e.g., AI-powered hiring tools, resume screeners), this applies.

### Utah

- **Utah AI Policy Act (SB 149)** (effective May 1, 2024):
  - Requires disclosure when a person interacts with generative AI in certain regulated contexts (particularly in regulated occupations like law, medicine, etc.)
  - Creates a regulatory sandbox for AI development
  - **AI Learning Lab** and **Office of AI Policy** for guidance

### New Jersey

- **Various proposals** advancing AI transparency requirements in employment, consumer protection, and education contexts. Monitor for enacted legislation.

---

## Russia

### Current State

- **No comprehensive AI disclosure law** as of early 2026.
- Russia has adopted a **National AI Development Strategy** (2019) and an **AI Federal Law concept**, but neither imposes specific disclosure requirements comparable to the EU AI Act.
- **Draft bill expected**: A comprehensive AI regulation bill is expected to be introduced to the State Duma by approximately **September 2027**. Early drafts suggest it will apply to AI systems with more than **500,000 daily active users**, focusing on:
  - Transparency of AI-generated content
  - Labeling requirements for AI chatbots
  - Obligations for large-scale AI platforms

### Current Applicable Rules

- **Consumer protection law**: Article 10 of the Law on Protection of Consumer Rights requires providing consumers with "necessary and reliable information" about goods and services. If AI materially affects the service quality, non-disclosure could theoretically be challenged.
- **Advertising law (38-ФЗ)**: AI-generated advertising content is subject to the same rules as human-created content (see testimonials-advertising.md for details on ОРД marking).
- **Personal data law (152-ФЗ)**: If AI processes personal data, standard consent and disclosure requirements under 152-ФЗ apply.

---

## United States Federal -- FTC Enforcement

### Section 5 -- Deceptive Practices

The FTC uses its broad Section 5 authority (prohibiting "unfair or deceptive acts or practices") to police AI-related deception.

### Key Enforcement Principles

1. **AI-generated content presented as human-created is deceptive**: If consumers would reasonably believe content was created by a human, and it was actually AI-generated, this can be a Section 5 violation.
2. **AI-powered interactions must not deceive**: Using AI chatbots that impersonate humans in a commercial context without disclosure may violate Section 5.
3. **AI claims must be substantiated**: Claims about what an AI system can do must be truthful and substantiated.
4. **AI-generated reviews are illegal**: The FTC has explicitly stated that AI-generated fake reviews violate the FTC Act.

### Rytr Enforcement Action (2024)

- **Case**: FTC v. Rytr (AI writing tool)
- **Issue**: Rytr marketed itself as a tool for generating product reviews, and the FTC alleged it was being used to create fake reviews.
- **Outcome**: FTC banned Rytr from generating consumer reviews entirely. This was the first FTC enforcement action specifically targeting AI-generated reviews.
- **Key takeaway**: **AI-generated product reviews are per se deceptive** under FTC guidance. Do not allow your AI tools to generate fake reviews, and do not use AI to generate reviews for your own products.

### FTC Guidance Documents

- **"Keep Your AI Claims in Check"** (February 2023): Companies must not exaggerate what their AI can do, must not deceive consumers about whether they are interacting with AI, and must ensure AI-driven decisions are not discriminatory.
- **"Chatbots, deepfakes, and voice clones"** (March 2023): Using AI to impersonate people or deceive consumers is illegal.

---

## When to Disclose AI Use -- Practical Guide

### Always Disclose

| Scenario | Disclosure Required | Authority |
|----------|-------------------|-----------|
| **AI chatbot** interacting with customers | "You are chatting with an AI" | EU AI Act Art. 50, CA Bot Law, FTC |
| **AI-generated marketing content** (blog posts, emails, social posts) | Mark as AI-generated (metadata + visible label where required) | EU AI Act Art. 50, CAITA |
| **AI grading or assessment** in education | Inform students AI is used; provide appeal mechanism | EU AI Act Annex III, Colorado AI Act |
| **AI-generated testimonials** or reviews | Never use AI to generate fake reviews; disclose AI involvement | FTC Consumer Reviews Rule, EU Omnibus |
| **AI-generated images** in marketing | Embed provenance metadata (C2PA) | EU AI Act Art. 50, CAITA |
| **AI-powered recommendations** affecting consequential decisions | Disclose AI involvement and provide opt-out/appeal | Colorado AI Act, NYC LL 144 |
| **AI customer service** where human expected | Disclose AI; offer human escalation | EU AI Act Art. 50, FTC Section 5 |

### Gray Areas (Disclose Out of Caution)

- AI-assisted (not fully generated) content where AI contribution is significant
- AI spell-checking or grammar correction in user-submitted content
- AI-powered search or content curation within your platform
- AI used for internal analytics that indirectly affects user-facing decisions

---

## Practical Compliance Checklist for SaaS/Education Platforms

### Inventory

- [ ] List all places in your product where AI is used (chatbots, content generation, grading, recommendations, search, analytics)
- [ ] Classify each use case by risk level (prohibited, high-risk, limited-risk, minimal-risk) under the EU AI Act
- [ ] Determine which jurisdictions your users are in

### Chatbot Disclosure

- [ ] Add a clear, persistent notice to all AI chat interfaces: "You are chatting with an AI assistant"
- [ ] Ensure the notice appears before or at the very start of the conversation
- [ ] Offer an option to request a human agent where applicable

### Content Marking

- [ ] Implement C2PA provenance metadata for all AI-generated images, audio, and video
- [ ] For AI-generated text content, add visible labels ("Generated with AI assistance") and/or metadata
- [ ] For AI-generated marketing emails, include disclosure in the email footer

### Education-Specific (High-Risk)

- [ ] Document the AI system's purpose, capabilities, and limitations (technical documentation per Article 11)
- [ ] Implement human oversight for AI-driven grading and assessment decisions
- [ ] Provide students with the right to appeal AI-made decisions and request human review
- [ ] Conduct and document a conformity assessment before deploying AI grading systems to EU users
- [ ] Maintain logging of AI system inputs and outputs for traceability
- [ ] Register the AI system in the EU AI database (when the registration portal is available for Annex III systems)

### Training Data Transparency (California AB 2013)

- [ ] If you train custom AI models, prepare and publish a training data summary
- [ ] If you use third-party AI APIs, verify the provider has published their training data disclosures
- [ ] Include a link to training data disclosures in your privacy policy or a dedicated AI transparency page

### Reviews and Testimonials

- [ ] Never use AI to generate fake reviews of your product
- [ ] If your product enables users to generate reviews using AI, implement safeguards (or block this feature, following the Rytr precedent)
- [ ] Clearly label AI-generated or AI-assisted testimonials

### Monitoring and Updates

- [ ] Set calendar reminders for key compliance dates:
  - January 1, 2026: California AB 2013 effective
  - June 1, 2026: Colorado AI Act effective
  - August 1, 2026: CAITA effective
  - August 2, 2026: EU AI Act transparency obligations effective
- [ ] Monitor legislative developments in Russia (expected draft bill September 2027)
- [ ] Review and update AI disclosure practices quarterly
- [ ] Designate an internal owner for AI compliance
