# Batch Calculator FAQ

> As of **2026-09-16**. If features or limits change, the [batch calculator page](https://invoicetariff.com/en/batch) is authoritative.
> 其他语言：[中文](../zh/batch-calculation-faq.md)

The [SKU Batch Calculator](https://invoicetariff.com/en/batch) is built for "recalculate the whole catalog / settle landed cost" scenarios: upload an XLSX/CSV, price every row, and export the results with duties and fees. The most common questions are answered below.

## Basic usage

**Q: How many rows can I calculate at once?**
Up to **200 rows per file** — extra rows are not parsed (split the file and retry); up to **5 files per day** (counted in your browser only — clearing site data resets it). Need more? [Join the waitlist](https://invoicetariff.com/en/api-waitlist) for higher limits.

**Q: What columns does the template use?**
Template columns: **SKU, Description, HTS, Value USD, Net weight kg, Qty, Freight share USD**. Download the CSV / XLSX template from the page, fill it in, and upload.

**Q: Which destination and transport mode does it use?**
Batch runs under the **U.S. full regime** (destination = United States). The transport mode (ocean/air) is set once for the whole shipment and controls whether HMF applies.

**Q: Is my data uploaded to a server?**
No. Parsing and math run **entirely in your browser — data never leaves your machine**. That is a design principle of the product, and the reason you can safely drop a full price list in. Only minor preferences are kept in your browser's localStorage.

## Scope and results

**Q: What does "shipment scope" mean?**
MPF/HMF are charged per entry, so the two scopes give different results:

- **All SKUs on one entry**: MPF/HMF charged once, on the total value (consolidation is cheaper);
- **Each SKU entered separately**: fees per row, each with the $33.58 MPF minimum.

The results page states the selected scope, with fees shown as a separate total line.

**Q: Why does a row say "HTS not found in local library"?**
That 8/10-digit code is not in the local tariff library. Verify the code in the [HTS code lookup](https://invoicetariff.com/en/hts), fix the sheet, and re-upload.

**Q: Why does a row require net weight?**
The code's MFN rate is a **specific or compound rate** (priced per kilogram) — net weight is required to compute it. Fill in the weight column.

**Q: What do the results represent?**
Results are **estimates**, returned with the ruleset version; rows with issues are flagged inline and can be fixed and recalculated on the spot. Batch results are for reference and are **not a customs opinion** — final entry figures belong to your broker.

**Q: How do I export results?**
After calculating, **export the XLSX results** with per-row duties and per-unit landed cost, ready for costing and pricing.

## Typical scenarios

- **Recalculating a whole catalog after a policy change**: e.g. after the [De Minimis suspension](../../policy/en/02-de-minimis-suspension.md) or the [global Section 301 tiers](../../policy/en/05-global-section-301.md), run every SKU through once, then decide on pricing and re-sourcing.
- **Comparing sourcing countries**: run the same sheet once with China and once with Vietnam as origin to see the effective-rate gap (background: [China 301](../../policy/en/04-section-301-china.md), [global 301](../../policy/en/05-global-section-301.md)).
- **Consolidated vs. separate entries**: switch the shipment scope, run both ways, and compare the MPF/HMF savings.

---

**Go straight to**: [SKU Batch Calculator](https://invoicetariff.com/en/batch) · [Tariff Calculator](https://invoicetariff.com/en) · [HTS Code Lookup](https://invoicetariff.com/en/hts) · [Higher limits / API waitlist](https://invoicetariff.com/en/api-waitlist) · [Subscribe to change alerts](https://invoicetariff.com/en/radar)

> This document describes product features and general policy context — it is not customs or legal advice.
