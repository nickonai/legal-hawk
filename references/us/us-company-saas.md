# US Company for SaaS — Draft Reference

> **Статус:** Черновик. Требует проверки с реальным US CPA/attorney.
> **Последнее обновление:** 2026-03-31

---

## 1. Выбор типа компании

| Тип | Для кого | Налогообложение | Плюсы | Минусы |
|-----|----------|----------------|-------|--------|
| **C-Corp (Delaware)** | Стартапы с инвесторами | Двойное: корпоративный налог 21% + дивиденды | Инвесторы предпочитают, неограниченные акционеры, stock options | Двойное налогообложение |
| **LLC (Wyoming/Delaware)** | Соло-фаундеры, малый бизнес | Pass-through (доход на уровне владельца) | Гибкость, проще управление, один уровень налога | Сложнее привлекать инвестиции |
| **S-Corp** | Малый бизнес с US-резидентами | Pass-through | Экономия на self-employment tax | Только US-резиденты, макс. 100 акционеров |

**Рекомендация для SaaS:**
- Если планируешь привлекать инвестиции → **Delaware C-Corp**
- Если соло/бутстрап → **Wyoming LLC** (нет state income tax, $100/год)

---

## 2. Регистрация и первоначальные шаги

### Delaware C-Corp:
1. Зарегистрировать через registered agent (Stripe Atlas, Firstbase, Clerky)
2. Получить EIN (Employer Identification Number) от IRS
3. Открыть банковский счёт (Mercury, Relay, Brex)
4. Выпустить акции основателям (83(b) election — подать в IRS в течение 30 дней!)
5. Принять bylaws, назначить directors/officers
6. Зарегистрироваться для foreign qualification в штатах с nexus

### Wyoming LLC:
1. Зарегистрировать через registered agent
2. Получить EIN
3. Operating Agreement (даже для single-member)
4. Открыть банковский счёт
5. Определить tax election (default pass-through или elect S-Corp/C-Corp)

---

## 3. Federal Tax Obligations (IRS)

| Форма | Кто | Когда | Штраф за пропуск |
|-------|-----|-------|-----------------|
| **Form 1120** | C-Corp | 15 апреля (или 15-е число 4-го месяца после конца fiscal year) | $250/мес за каждого акционера, макс. $50K |
| **Form 1120-S** | S-Corp | 15 марта | $250/мес за каждого акционера |
| **Form 1065** | LLC (multi-member) | 15 марта | $250/мес за каждого партнёра |
| **Form 1040 + Schedule C** | LLC (single-member) | 15 апреля | Failure-to-file penalty: 5%/мес, макс. 25% |
| **Form 5472** | C-Corp с иностранным владельцем (>25%) | С Form 1120 | **$25,000** за каждую непредставленную форму! |
| **Form 1120-W** | C-Corp (estimated tax) | 15.04, 15.06, 15.09, 15.12 | Underpayment penalty |
| **Form 1042 / 1042-S** | Платежи иностранцам (withholding) | 15 марта | $280/форма, макс. $3.4M |
| **Form 1099-NEC** | Платежи US-контракторам >$600 | 31 января | $310/форма |
| **Payroll: 941** | Если есть сотрудники | Ежеквартально | 2-15% от неуплаченного налога |
| **Payroll: 940 (FUTA)** | Если есть сотрудники | 31 января | Penalty + interest |

### Критично для иностранных владельцев:
- **Form 5472** — штраф **$25,000** за КАЖДУЮ непредставленную форму. Если вы иностранный владелец US C-Corp — это самая дорогая ошибка.
- **FBAR (FinCEN 114)** — если есть иностранные банковские счета >$10K суммарно. Штраф: $10K-$100K+ за умышленное непредставление.
- **BOI Report (Beneficial Ownership)** — требуется для всех компаний с 2024. Сроки и enforcement меняются — проверь актуальный статус.

---

## 4. State Tax Obligations

### Delaware (если зарегистрирован, но нет nexus):
- **Franchise Tax**: $400/год (minimum) для C-Corp, $300/год для LLC
- **Annual Report**: с Franchise Tax, до 1 марта (C-Corp) / 1 июня (LLC)
- **Нет state income tax** на доход из-за пределов Delaware

### Штаты с economic nexus (если продаёшь туда):
- Каждый штат с $100K-$500K продаж может требовать:
  - State income tax filing
  - Sales tax collection и filing (если SaaS облагается в этом штате)
  - Foreign qualification registration

### Sales Tax для SaaS (основные штаты):

| Штат | SaaS облагается? | Ставка |
|------|------------------|--------|
| **New York** | Да | ~8.5% |
| **Texas** | Да (80%) | ~8.2% |
| **Washington** | Да + B&O tax | ~9.4% |
| **Pennsylvania** | Да | ~6.3% |
| **California** | Нет (если не bundled) | ~8.9% |
| **Florida** | Нет | — |
| **Oregon** | Нет sales tax | — |

**Решение:** Использовать Stripe Tax или MoR (Paddle/Lemon Squeezy) для автоматического расчёта.

---

## 5. Privacy & Data Protection (US)

### Federal:
- **Нет единого федерального закона о приватности** (в отличие от GDPR)
- **FTC Act Section 5** — запрет на unfair/deceptive practices (включая данные)
- **COPPA** — если пользователи <13 лет
- **CAN-SPAM** — email маркетинг (opt-out, не opt-in)
- **TCPA** — SMS/звонки (требует prior express consent)

### Штаты:
| Закон | Штат | Порог | Ключевые требования |
|-------|------|-------|-------------------|
| **CCPA/CPRA** | California | $25M revenue / 100K consumers / 50% data revenue | Privacy policy, opt-out "Do Not Sell", data access/deletion |
| **CPA** | Colorado | 100K consumers / 25K+ with revenue from data | Opt-out, DPA, universal opt-out mechanism |
| **CTDPA** | Connecticut | 100K consumers / 25K+ with 25% revenue | Similar to Colorado |
| **VCDPA** | Virginia | 100K consumers / 25K+ with 50% revenue | Opt-out, consent for sensitive data |
| **TDPSA** | Texas | Conducts business in TX, no revenue threshold | Broad applicability |

**Что нужно на сайте:**
- Privacy Policy (обязательно если собираешь данные)
- "Do Not Sell or Share" ссылка (если CCPA applies)
- Cookie banner (best practice, обязательно для CA)
- Terms of Service

---

## 6. Employment & Contractors

### US Employees:
- **Payroll tax**: Social Security (6.2%) + Medicare (1.45%) = 7.65% employer share
- **FUTA**: 6% на первые $7K (effective 0.6% с кредитом)
- **State unemployment tax** (SUTA): varies
- **Workers' compensation insurance**: required in most states
- **I-9 verification**: для каждого сотрудника
- **W-2**: до 31 января

### US Contractors:
- **1099-NEC**: для платежей >$600/год
- **W-9**: собрать до первого платежа
- **Misclassification risk**: штрафы IRS + state penalties + back taxes

### Иностранные контракторы:
- **W-8BEN**: собрать до первого платежа
- **Form 1042-S**: отчёт по платежам
- **30% withholding** по умолчанию (если нет tax treaty)
- Tax treaties: UK 0%, Russia suspended, UAE 0%, India 15%

---

## 7. Stripe / Payment Compliance (US-specific)

- **1099-K**: Stripe выдаёт автоматически для US sellers с >$600/год
- **Sales tax**: Stripe Tax рассчитывает автоматически, но вы remit сами
- **Prohibited businesses**: get-rich-quick, predatory coaching = Stripe ban risk
- **Chargeback**: держать <0.75%

---

## 8. Intellectual Property

- **Trademark**: зарегистрировать в USPTO ($250-$350 per class)
- **Copyright**: автоматически, но регистрация ($65) даёт statutory damages
- **Patents**: provisional patent application ($320 для small entity)
- **Trade secrets**: NDA с контрактерами и сотрудниками

---

## 9. Compliance Calendar (US C-Corp, Delaware, Foreign Owner)

| Месяц | Дедлайн | Действие |
|-------|---------|----------|
| Январь | 31.01 | W-2 сотрудникам, 1099-NEC контракторам |
| Март | 01.03 | Delaware Annual Report + Franchise Tax |
| Март | 15.03 | Form 1042/1042-S (если платежи иностранцам) |
| Апрель | 15.04 | Form 1120 + Form 5472 (или extension) |
| Апрель | 15.04 | BOI Report (проверить актуальный дедлайн) |
| Апрель | 15.04 | Estimated tax Q1 (Form 1120-W) |
| Апрель | 15.04 | FBAR (или extension до 15.10) |
| Июнь | 15.06 | Estimated tax Q2 |
| Сентябрь | 15.09 | Estimated tax Q3 |
| Октябрь | 15.10 | Form 1120 (с extension) |
| Декабрь | 15.12 | Estimated tax Q4 |

### Ежеквартально (если есть сотрудники):
- Form 941 (payroll tax) — до конца месяца после квартала
- State payroll filings

### По мере необходимости:
- Sales tax filing (ежемесячно/квартально/ежегодно — зависит от штата)
- Foreign qualification renewals в штатах с nexus

---

## 10. Типичные ошибки иностранных основателей US-компаний

1. **Не подал Form 5472** → штраф $25,000 за форму
2. **Не подал 83(b) election** в течение 30 дней → огромный налог при vesting
3. **Смешал личные и бизнес-финансы** → piercing corporate veil
4. **Не собирает sales tax** в штатах с nexus → back taxes + penalties
5. **Платит иностранным контракторам без W-8BEN и withholding** → IRS penalties
6. **Не ведёт corporate minutes** → risk of losing corporate protection
7. **Забыл Delaware Franchise Tax** → $200 late fee + 1.5%/мес interest
8. **Не зарегистрировался в штате где есть сотрудники** → state penalties
9. **FBAR не подан** → $10K-$100K+ штраф
10. **Transfer pricing не документирован** → IRS audit + penalties

---

> **ВАЖНО:** Это черновик-справочник. US-налоговое право чрезвычайно сложное и зависит от множества факторов. ОБЯЗАТЕЛЬНО привлеките US CPA для конкретных решений. Этот документ — отправная точка для понимания ландшафта, а не замена профессиональной консультации.
