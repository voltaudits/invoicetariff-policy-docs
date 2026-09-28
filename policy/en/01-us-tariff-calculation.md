# How U.S. Import Tariffs Are Calculated

> As of **2026-09-28**. Tariff policy changes frequently — see the [Tariff Radar (change log + email alerts)](https://invoicetariff.com/en/radar) for the latest.
> 其他语言：[中文](../zh/01-us-tariff-calculation.md)

## The formula

Every layer of U.S. import duty is an *ad valorem* percentage applied to the **same customs value**. The layers are **added** to each other; no layer compounds on another:

```text
Total duty  = Customs value × (MFN rate + Section 301 rate + Section 232 rate + …)
Fees        = MPF (0.3464% of value; per-entry min/max $33.58 / $651.50
              through 2026-09-30, $34.58 / $670.86 from 2026-10-01 — 91 FR 48398)
            + HMF (0.125% of value, ocean only)
Owed to CBP = Total duty + Fees
```

Three things follow:

- **Rates add, they do not multiply.** 16.5% + 7.5% + 12.5% is a 36.5% duty, not 1.165 × 1.075 × 1.125 ≈ 40.9%.
- **International freight is not in the base.** Unlike the EU or Canada, which value goods CIF, the United States uses transaction value, excluding international freight and insurance when shown separately.
- **Fees are not duties.** The Merchandise Processing Fee (MPF) and Harbor Maintenance Fee (HMF) are user fees under a different statute, charged per entry and not refundable under trade programs that refund duties.

## What "customs value" means

U.S. customs value is the **transaction value** defined in 19 U.S.C. § 1401a: the price actually paid or payable for the goods when sold for export to the United States, plus certain additions if not already in the price:

| Included in customs value | Not included (if separately identified) |
|---|---|
| Price paid or payable to the seller | International freight and insurance |
| Packing costs | U.S. inland freight after import |
| Selling commissions paid by the buyer | Customs duties and fees themselves |
| **Assists** — tooling, molds, materials, design work the buyer supplies free or at reduced cost | Buying commissions |
| Royalties the buyer must pay as a condition of the sale | Post-import services (installation, training) |
| Proceeds of resale that accrue to the seller | |

In practice, for most e-commerce and wholesale shipments the customs value is the **FOB / EXW invoice price**. If you quote DDP, you still declare the goods value — not the DDP price — and the duty you pay is your cost.

## The layers a single shipment can hit

| Layer | Legal basis | Applies to | How it is set |
|---|---|---|---|
| **MFN base rate** (HTSUS column 1, "General") | Tariff Act of 1930; HTSUS column 1 | Every country with normal trade relations | Fixed per 8/10-digit HTS code by the USITC: "Free", a percentage, or a specific / compound rate |
| **China Section 301** (Lists 1–4A + four-year-review increases) | Trade Act of 1974 § 301 (USTR) | Goods of Chinese origin only | 25% on Lists 1–3, 7.5% on List 4A; higher review rates on targeted products (e.g. solar cells 50%) |
| **Global Section 301 program** | Trade Act of 1974 § 301 (USTR, effective 2026-07-24) | Country-specific tiers — 12.5% for China, 10% for the UK, etc., with combined caps for some partners | Set per economy in FR 2026-15181; product exclusions published separately |
| **Section 232** | Trade Expansion Act of 1962 § 232 (Presidential proclamations) | Specific sectors regardless of origin: steel & aluminum 50%, copper 50%, autos & parts 25%, timber 10%, furniture 25%, semiconductors 25%, pharmaceuticals (general tier 20% from 2026-09-29) | By HTS scope listed in each proclamation annex; some derivatives on metal content only |
| **Section 338** | Tariff Act of 1930 § 338 (19 U.S.C. § 1338, Presidential proclamations) | Goods of countries found to discriminate against U.S. commerce — currently Canadian motor vehicles, dairy and alcoholic beverages (50%, since 2026-08-22) | Up to 50% by proclamation; stacks on other layers but not on goods already under Section 232 |
| **AD / CVD** | Tariff Act of 1930 Title VII (Commerce / ITC) | Named producers or countries in a specific case | Case-by-case rates, often very high; deposited at entry, finalized later |
| **MPF + HMF** | 19 U.S.C. § 58c (MPF); 26 U.S.C. § 4461 (HMF) | Every formal entry (HMF: ocean only) | MPF 0.3464% of value with per-entry floor and cap; HMF 0.125% |

Two programs still referenced in older material **no longer apply to new entries**:

- **IEEPA "reciprocal" and fentanyl tariffs** (Chapter 99 headings 9903.01 / 9903.02): struck down on 2026-02-24. Duties paid between 2025-02-04 and 2026-02-24 are refundable through the CBP CAPE process — see the [IEEPA refund guide](03-ieepa-tariffs-and-refunds.md).
- **The $800 De Minimis exemption**: suspended for all countries since 2025-08-29; low-value shipments now pay the same duty stack — see the [De Minimis guide](02-de-minimis-suspension.md).

## Specific and compound rates

Not every MFN rate is a percentage. The HTSUS also uses:

- **Specific rates** — a fixed amount per unit of quantity, e.g. rice at *2.1¢/kg*. You need the net weight (or count) of the entry, not just the value.
- **Compound rates** — a percentage plus a specific rate, e.g. steel bolts at *9% + 0.5¢/kg*.

Even when the MFN base is specific or compound, Section 301 and 232 layers remain ad valorem on the customs value. The calculator shows the ad valorem layers and asks for net weight where a specific component applies; results without weight are labeled a partial estimate.

## Worked example: cotton T-shirts from China

Take HTS **6109.10.00** (knitted cotton T-shirts), $10,000 of goods, formal ocean entry, 1,000 units: the MFN rate, the China Section 301 rate and the global Section 301 tier are each multiplied by the same $10,000 and added. MPF and HMF are charged on that same $10,000 — not on value plus duty. Divide the total by the unit count and you have the per-unit duty for your landed cost.

Change any one input — origin country, HTS code, entry date, ocean vs air — and the stack changes. "The tariff on China" is never a single number: it is the sum of whichever layers the specific code triggers on the specific date.

## Statutory rate ≠ effective rate

- **Statutory rate**: what one program charges, e.g. "25% under Section 301".
- **Effective rate**: (all duties + fees) ÷ customs value.

In the example above the effective rate is roughly 37% even though no single program charges 37%. Compare suppliers across countries, or decide how much cost to pass through, using the effective rate.

## What changes the answer

- **Entry date.** Rates are time-bound: the global Section 301 program started 2026-07-24; MPF minimum and maximum rise on 2026-10-01 (FY2027 — $34.58 / $670.86, 91 FR 48398); Section 232 pharmaceutical tariffs begin 2026-09-29. The engine keys every rate to its effective window, and the [Tariff Radar](https://invoicetariff.com/en/radar) logs each change with its Federal Register source.
- **Country of origin** — where the goods were made or last substantially transformed, not where they shipped from. Transshipping through a third country does not change origin.
- **Entry type.** Formal entries pay ad valorem MPF; postal informal entries (≤ $2,500) pay a flat fee instead. HMF applies only to ocean arrivals.
- **AD/CVD orders** on the product-country pair, which sit on top of everything above.
- **Preferential programs** such as USMCA can zero out the MFN layer; they generally do not remove Section 232 or 301 layers.

## Check your own tariff stack

1. **Fix the exact code first**: start from the [HTS code lookup](https://invoicetariff.com/en/hts) and confirm the 8/10-digit code against USITC or a customs ruling.
2. **Read the code page**: each code page (e.g. [/en/hts/61091000](https://invoicetariff.com/en/hts/61091000)) lists every applicable layer (MFN, China 301, global 301, 232) with rate, effective window, verification status and Federal Register source.
3. **Run the entry date**: the [U.S. tariff calculator](https://invoicetariff.com/en) prices the stack for a specific date, origin and transport mode.
4. **Whole catalogs**: for more than a handful of SKUs, the [SKU batch calculator](https://invoicetariff.com/en/batch) prices an entire XLSX/CSV sheet and returns the ruleset version with the results.

---

**Related tools**: [Tariff Calculator](https://invoicetariff.com/en) · [Landed Cost Calculator](https://invoicetariff.com/en/landed-cost-calculator) · [SKU Batch Calculator](https://invoicetariff.com/en/batch) · [HTS Code Lookup](https://invoicetariff.com/en/hts) · [Subscribe to tariff change alerts](https://invoicetariff.com/en/radar)

> This article is a general policy explainer for reference only — not customs or legal advice. Entry decisions should be based on the HTSUS, Federal Register notices and CBP guidance.
