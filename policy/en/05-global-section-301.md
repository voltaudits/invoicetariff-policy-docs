# The Global Section 301 Program (Effective 2026-07-24): Country Tiers

> As of **2026-10-05**. Tariff policy changes frequently — see the [Tariff Radar (change log + email alerts)](https://invoicetariff.com/en/radar) for the latest.
> 其他语言：[中文](../zh/05-global-section-301.md)

## What this new program is

Under **FR 2026-15181 (91 FR 47318)**, USTR established a *separate* Section 301 program based on **forced-labor findings**, effective **2026-07-24** (goods loaded before that date kept prior treatment through 2026-07-28). It is not an amendment to the China 301 — it is a **global, tiered regime covering roughly 60 economies**, reported at entry through Chapter 99 like any other 301 layer.

Note: the program **is under litigation** — a consolidated challenge by 25 state attorneys general (*Oregon et al. v. Trump*, filed 2026-08-03) and by several businesses is pending at the Court of International Trade (CIT), which **held oral argument on 2026-09-30**; no ruling had issued as of 2026-10-05. Challengers argue the program is forced-labor relief in name only — a way to keep the Supreme Court-struck IEEPA global tariffs alive through Section 301. **CBP is collecting the duty in the meantime**, so plan cash flow on the assumption it applies — if it is later struck down, refunds along the IEEPA precedent become possible (see the [IEEPA refund guide](03-ieepa-tariffs-and-refunds.md)).

## The country tiers

| Tier | Economies | Effect |
|---|---|---|
| **Flat 10%** | 17 — incl. Canada, Mexico, India, Indonesia, Malaysia, UK | 10% on customs value; USMCA-qualifying goods exempt for Canada/Mexico |
| **Combined cap 10%** | European Union, Taiwan | MFN + 301 together cannot exceed 10% of value |
| **Flat 12.5%** | 38 — incl. **China**, Vietnam, Thailand, Singapore, Brazil, Hong Kong | 12.5% on customs value |
| **Combined cap 12.5%** | Japan, South Korea, Switzerland | MFN + 301 together capped at 12.5% |

Three things matter most for your supply chain:

- **China = two layers of 301.** Chinese-origin goods pay the legacy China lists (Lists 1–4A) *and* the 12.5% global tier, each on the same customs value. See the [China 301 guide](04-section-301-china.md).
- **Exemptions.** Goods already covered by a Section 232 order, USMCA-qualifying goods, and products on the program's Annex I/II exemption lists are excluded from the global tier.
- **Origin sets the tier, not the ship-from port.** "Made in Vietnam" pays the 12.5% tier; the difference vs. China is only the missing Lists 1–4A layer — transshipment does not change origin, and CBP is actively pursuing transshipment cases.

## Worked example: same shirt, two origins

Same HTS **6109.10.00** (knitted cotton T-shirt), $10,000 value, formal ocean entry, 1,000 units:

- **From China**: MFN + List 4A (7.5%) + global tier (12.5%) + MPF/HMF;
- **From Vietnam**: MFN + global tier (12.5%) + MPF/HMF.

The China version carries one extra layer — the 7.5% List 4A duty — which on $10,000 is **$750 more duty per entry**. Everything else is identical. That single layer is why "move production to Vietnam" only saves money if the transformation is real: customs origin follows where the goods were made or last substantially transformed.

Enter your code, origin and date in the [tariff calculator](https://invoicetariff.com/en) — every duty row links to the Federal Register notice behind it. For whole catalogs, use the [batch calculator](https://invoicetariff.com/en/batch).

## How the tier stacks with everything else

The global 301 tier **adds** to all other layers and never compounds (see [how U.S. tariffs are calculated](01-us-tariff-calculation.md)):

```text
Duty owed = Customs value × (MFN + China 301 (if applicable) + global 301 tier + Section 232 (if applicable) + …)
```

Exceptions:

- Goods already covered by **Section 232** do not enter the global tier;
- **USMCA-qualifying** Canadian/Mexican goods do not enter the global tier;
- **Combined-cap** economies (EU, Taiwan, Japan, South Korea, Switzerland) are capped at "MFN + 301 ≤ cap";
- The program's own **Annex I/II** product exemption lists apply across all covered economies (the engine has keyed in the text-based entries; items published only as picture attachments are still being transcribed — code pages flag what is verified and what is not).

## Quick path: "what does my country pay now?"

1. Pick the origin country on the [tariffs-by-country topic](https://invoicetariff.com/en/tariffs-by-country) to see its tier;
2. Confirm the product code and every layer with the [HTS code lookup](https://invoicetariff.com/en/hts);
3. Price the full stack for your entry date in the [tariff calculator](https://invoicetariff.com/en).

Tiers and exemption lists move with the Federal Register — the [Tariff Radar](https://invoicetariff.com/en/radar) logs every change, and you can [subscribe to email alerts](https://invoicetariff.com/en/radar).

---

**Related articles**: [Section 301 on China](04-section-301-china.md) · [How U.S. tariffs are calculated](01-us-tariff-calculation.md) · [De Minimis suspension](02-de-minimis-suspension.md)

**Related tools**: [Tariffs by Country topic](https://invoicetariff.com/en/tariffs-by-country) · [Tariff Calculator](https://invoicetariff.com/en) · [SKU Batch Calculator](https://invoicetariff.com/en/batch) · [HTS Code Lookup](https://invoicetariff.com/en/hts)

> This article is a general policy explainer for reference only — not customs or legal advice. Entry decisions should be based on the HTSUS, Federal Register notices and CBP guidance.
