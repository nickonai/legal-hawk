# Карта базы знаний

> Часть навыка `legal-hawk`, вынесена из `SKILL.md` без изменения формулировок. Предупреждение о датах, Evidence Gate (Шаг 6 в `SKILL.md`) и дисклеймер в конце ответа действуют и здесь.

## Карта базы знаний (`references/`)

Это ПОЛНЫЙ список справочных файлов. Читай только релевантные для задачи — не загружай всё подряд.

**Россия (`references/russia/`):**
- `152-fz-personal-data.md` — персональные данные, локализация, Роскомнадзор, согласия
- `54-fz-online-kassa.md` — онлайн-кассы, чеки, ККТ
- `consumer-protection.md` — ЗоЗПП, возвраты, права потребителей
- `education-licensing.md` — образовательная лицензия (273-ФЗ)
- `ooo-requirements.md` — корпоративные требования к ООО
- `recurring-payments.md` — подписки, автосписания, 376-ФЗ
- `website-checklist.md` — полный чеклист сайта для РФ

**UAE (`references/uae/`):**
- `pdpl-data-protection.md` — PDPL (Decree-Law 45/2021)
- `ecommerce-law.md` — E-Commerce Law, онлайн-продажи
- `ifza-compliance.md` — требования IFZA FZCO, лицензия, отчётность
- `website-checklist.md` — полный чеклист сайта для UAE

**US (`references/us/`):**
- `us-company-saas.md` — US LLC / C-Corp для SaaS
- `childrens-data-biometrics.md` — COPPA-2025, Illinois BIPA, биометрия, дети (+ GDPR-дети/UAE)
- `ip-trademark-ugc.md` — товарные знаки и авторские права в UGC / AI-генерации / print-on-demand: чужие персонажи и логотипы по запросу пользователя, миф «пользователь попросил» и «один экземпляр для личного пользования», nominative fair use и Rogers vs. Jack Daniel's (2023), de minimis, statutory damages (§504(c), §1117(c)), прецеденты POD (SunFrog $19.2M, Zazzle, Redbubble), indemnity типографии (Lulu §3/§16), Schedule A TRO с заморозкой Stripe/PayPal, right of publicity
- `negative-option-ftc.md` — FTC Act §5(a), ROSCA 15 U.S.C. §§8401-8405, негативный опцион, "quiz funnel" мошенничество, «clearly and conspicuously» 8-part test, Visa/Mastercard схемные правила, прецеденты (Genesis Tech $106M, Amazon $2.5B, Vonage $100M, ABCmouse $10M)

**EU (`references/eu/`):**
- `consumer-rights.md` — Consumer Rights Directive 2011/83/EU (14-дневный отзыв, кнопка оплаты, пре-контрактная информация), Digital Content Directive 2019/770, Omnibus Directive 2019/2161 (fake discounts, fake reviews, персонализированные цены), UCP Directive 2005/29/EC (черный список запрещённых практик, fake urgency, bait & switch)
- `enforcement-precedents.md` — Крупнейшие EU/GDPR штрафы с прецедентами: Meta €1.2B (SCCs), Amazon €746M (таргетинг), TikTok €345M (дети), Google €150M (cookie dark patterns), Facebook €60M (cookie banner). Таблица "это уже штрафовали" для аргументации
- `website-checklist.md` — Полный EU website compliance checklist: cookies, GDPR, Consumer Rights, UCP/dark patterns, AI Act Art. 50, EAA 2025, DSA, international transfers

**International (`references/international/`):**
- `gdpr.md` — GDPR основы (Art. 5-7, Art. 13-14, Art. 30 ROPA, Art. 32-36, Art. 37-39 DPO, Art. 83 штрафы)
- `eprivacy-cookies.md` — cookie consent, ePrivacy Directive, CMPs, страновые различия (CNIL/DSK/Garante)
- `uk-gdpr.md` — UK GDPR, PECR, ICO
- `ccpa-cpra.md` — Калифорния (если есть US-клиенты)
- `cross-border-transfers.md` — трансграничная передача данных (SCCs, адекватность, EU-US DPF)
- `accessibility.md` — WCAG 2.1/2.2, EAA + EN 301 549, ADA Title III, **US state law (CA Unruh $4K/violation, NY HRL)**, **accessibility-оверлеи как liability (FTC v. accessiBe $1M)**, **драфтинг Accessibility Statement (overpromise trap, defensive vs. audited pattern)**, playbook по demand letter
- `ai-disclosure.md` — EU AI Act (Art. 50 disclosure, High-Risk Annex III образование), раскрытие AI
- `dark-patterns.md` — манипулятивные UI-паттерны
- `non-obvious-traps.md` — неочевидные ловушки (trial→paid, geoblocking, COPPA и др.)
- `platform-compliance.md` — требования Stripe / Google Ads / рекламы в соцсетях / Visa/Mastercard
- `tax-compliance.md` — VAT/НДС, EU OSS, Merchant of Record
- `testimonials-marketing.md` — отзывы, income claims, FTC, ОРД-маркировка

**Шаблоны (`references/templates/`):**
- `audit-report.md` — шаблон отчёта аудита (режим AUDIT)
- `document-templates.md` — структуры юридических документов (режим GENERATE)
